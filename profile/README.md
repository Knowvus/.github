## Welcome to the team 🙌

🙋‍♀️ **INTRODUCTION**

*Problem*: Documenting learnings and planning projects is inefficent due to data silos.
*Solution*: Knowvus synthesizes org-wide data and deliveres relevant insights in real-time.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Deployment](#deployment)
- [Infrastructure](#infrastructure)
- 
## How to CLI Deploy to a DigitalOcean Droplet

This guide explains how to use the provided CLI commands to deploy your application to a DigitalOcean Droplet.

### Prerequisites

1. **DigitalOcean Droplet**: Ensure you have a running Droplet.
2. **SSH Key**: Generate an SSH key pair and add the public key to your Droplet's `~/.ssh/authorized_keys`.
3. **Docker Hub Account**: Ensure your Docker image is pushed to Docker Hub.
4. **Infisical Account**: Ensure you have an Infisical account and project token.

### [Setup]

1. **Generate SSH Key**:
```
   ssh-keygen -t ed25519 -C "your_email@example.com"
```

2. Add the public key to your DigitalOcean Droplet:
```
cat ~/.ssh/id_ed25519.pub | ssh root@<DROPLET_IP> 'cat >> ~/.ssh/authorized_keys'
```

4. Test the SSH connection:
```
ssh -i ~/.ssh/id_ed25519 root@<DROPLET_IP>
```

5. Encode the private key in base64:
```
base64 -w 0 ~/.ssh/id_ed25519 > key_base64.txt
```

6. Set up Infisical:
- Install Infisical CLI:
```
npm install -g infisical
- Authenticate with Infisical:
```
infisical login --token <YOUR_INFISICAL_PROJECT_TOKEN>```

6. Store the SSH Key in Infisical:
- Add the base64 encoded SSH private key to Infisical:
```
infisical secret set DROPLET_SSH_BASE64 --value "$(cat key_base64.txt)"
```

7. Store the Known Hosts in Infiscal
-  Fetch the known hosts and add them to Infisical:
```
ssh-keyscan <DROPLET_IP> > known_hosts.txt
infisical secret set KNOWN_HOSTS --value "$(cat known_hosts.txt)"
```

8. Store the Droplet IP in Infiscal
- Add the Droplet IP to Infisical:
```
infiscal secret set DROPLET_IP --value "<DROPLET_IP>"
```

### Deployment

1. Fetch secrets from Infisical:
```
infisical pull --env production
```

3. Set up SSH key:
```
echo "$DROPLET_SSH_BASE64" | base64 --decode > key.pem
chmod 600 key.pem
```

4. Add known hosts:
```
mkdir -p ~/.ssh
echo "$KNOWN_HOSTS" > ~/.ssh/known_hosts
```

5. Deploy to DigitalOcean Droplet:
```
ssh -i key.pem -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no root@$DROPLET_IP << 'EOF'
  set -e
  docker pull your-dockerhub-username/your-app:latest
  docker stop your-container-name || true
  docker rm your-container-name || true
  docker run -d -p 8000:8000 --name your-container-name your-dockerhub-username/your-app:latest
EOF
```










---
## Infrastructure

1. Duke
- IP: 10.116.0.2
Kerrigan
- IP: 10.17.0.5


**MILESTONES**

Feature: Launch CLI Server-DB Interface
1) Duke       [Server]
- [ ] **Initialize Server**
- [ ] **Endpoints**
  - [ ] /create-user
    -  [ ] _Data Validation: Check for Duplicates_
  - [ ] /create-task
- [ ]  **Logging**
  - [ ] Initialization
  - [ ] Endpoints
    - [ ] Logging Payload
    - [ ]  User_IP
    - [ ]  User_Email
    - [ ]  Datetime_Stamp
    - [ ]  Service_Name
        
3) Artanis    [Observability]
4)   
5) Kerrigan   [Postgres]



## OVERVIEW

[Resources](#RESOURCES)

[Components](#COMPONENTS) 

[Architectural Decision Review](#ADR) 

👩‍💻 **RESOURCES**

- [Lucid](https://lucid.app/lucidchart/27a4f1ab-1925-4b57-b286-d59169d5385b/edit?invitationId=inv_c172e4c8-e0a9-4258-a836-6ee22863362c&page=qAbGdBw9_a6I#) - Master Architecture Diagram

  (+) [Eraser](https://app.eraser.io/workspace/QFzM4xawEp5SQTKiSW56) - Diagram Accelerator (Reduce Cycle Time via AI for Pareto Start)
- [Digital Ocean](https://DigitalOcean.com)       -  Infrastructure-as-a-Service           (Compute, Storage [RAM, SSD, CPU, GPU, NPU])
- [Cloud Flare](https://Cloudflare.com)           -  Hosting
- [Github](https://Github.com/Knowvus.com)        -  Codebase + CI/CD
- [Docker](https://Docker.com)                    -  Containerization  Deployment

## COMPONENTS

| Category       | Component | Description | Server Details | Cost |
|----------------|-----------|-------------|----------------|------|
| Infrastructure | [Duke](https://github.com/Knowvus/Duke) | Server | Container - Droplet: 1vCPU / 512MB / 10 GB Disk / 0.5 TB / Ubuntu 24.04 (LTS) x64 | $4/mo + $0.018/hr |
| Features       | [Tassadar](https://github.com/Knowvus/Tassadar) | Knowledge Framework | N/A | N/A |
| Features       | [Fenix](https://github.com/Knowvus/Fenix) | Frame Processing, Semantic Process & Vector Embedding | N/A | N/A |
| Features       | [Overmind](https://github.com/Knowvus/Overmind) | Modal Recorder | N/A | N/A |
| Storage        | [Kerrigan](https://github.com/Knowvus/Kerrigan) | Postgres | Container - Droplet: 1vCPU / 2GB / 50 GB Disk / 2 TB / Ubuntu 24.04 (LTS) x64 | $12/mo + $0.018/hr |
| Observability  | [Artanis](https://github.com/Knowvus/Artanis) | Observability | N/A | N/A |
| Platform Tools | [Duran](https://github.com/Knowvus/Duran) | CICD Automation | N/A | N/A |

## [ADR](https://github.com/Knowvus/.github-private/blob/main/documentation/ARD-%7BTemplate%7D.md)

We use Architectural Decision Reviews to document and communicate significant architectural decisions to ensure clarity, consistency, and informed decision-making across the organization.

- **Context**: Background information and the rationale behind the decision.
- **Decision**: A clear statement of the chosen architectural decision.
- **Consequences**: Positive and negative outcomes of the decision.
- **Implementation Details**: Specifics on how the decision will be implemented.
- **Recommended Libraries**: Tools and libraries to be used.
- **Metrics for Performance**: Key metrics to monitor for assessing performance.
- **Best Practices**: Guidelines and practices to ensure quality and consistency.
- **Key Stakeholders**: Individuals responsible for and affected by the decision.

## MONTHLY COST TO OPERATE
**FIXED**
```
Duke-COST:               $   4.00
Kerrigan-COST:           $  12.00
Duke-TRANSFER-LIMIT:          0.5 TB
Kerrigan-TRANSFER-LIMIT:      2.0 TB
```
**VARIABLE**
```
Duke-RATE-HR:            $  0.018
Kerrigan-RATE-HR:        $  0.018
Duke-VOLUME:                  1.0 TB <VALIDATE>
Kerrigan-VOLUME:              1.0 TB <VALIDATE>
Duke-COST:               $ 500.00    <VALIDATE>
Kerrigan-COST:           $ 100.00    <VALIDATE> 
```
**TOTAL**
```
Fixed:                   $  20
Variable:                $ 600
Total:                   $ 620
```

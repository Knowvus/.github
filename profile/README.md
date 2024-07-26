## Welcome to the team 🙌

🙋‍♀️ **INTRODUCTION**

Knowvus synthesizes org-wide data and deliveres relevant insights in real-time. 

👩‍💻 **RESOURCES**

- [Lucid](https://lucid.app/lucidchart/27a4f1ab-1925-4b57-b286-d59169d5385b/edit?invitationId=inv_c172e4c8-e0a9-4258-a836-6ee22863362c&page=qAbGdBw9_a6I#) - Architecture Diagrams
- [Digital Ocean](https://DigitalOcean.com)       -  Infrastructure-as-a-Service (Compute, Storage [RAM, SSD, CPU, GPU, NPU]
- [Cloud Flare](https://Cloudflare.com)           -  Hosting
- [Github](https://Github.com/Knowvus.com)        -  Codebase + CI/CD
- [Docker](https://Docker.com)                    -  Containerization  Deployment

## COMPONENTS

**INFRASTRUCTURE**
- [Duke](https://github.com/Knowvus/Duke)         -   Server - Container - Droplet: 1vCPU / 512MB / 10 GB Disk / 0.5 TB / ubuntu 24.04 (LTS) x64 - $4/mo + $0.018/hr

**FEATURES**
- [Tassadar](https://github.com/Knowvus/Tassadar) -   Knowledge Framework
- [Fenix](https://github.com/Knowvus/Fenix)       -   Frame Processing, Semantic Process & Vector Embedding
- [Overmind](https://github.com/Knowvus/Overmind) -   Modal Recorder

**STORAGE**
- [Kerrigan](https://github.com/Knowvus/Kerrigan) -   Postgres   - Container - Droplet: 1vCPU / 2GB / 50 GB Disk / 2 TB / ubuntu 24.04 (LTS) x64 - $12/mo + $0.018/hr

**OBSERVABILITY**
- [Artanis](https://github.com/Knowvus/Artanis)   -   Observability

**Platform Tools**
- [Duran](https://github.com/Knowvus/Duran)       -   CICD Automation

## [Architectural Decision Record](https://github.com/Knowvus/.github-private/blob/main/documentation/ARD-%7BTemplate%7D.md)

We use ADRs to document and communicate significant architectural decisions to ensure clarity, consistency, and informed decision-making across the organization.

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

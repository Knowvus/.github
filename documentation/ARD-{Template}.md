# Architectural Decision Record (ADR)

## ADR: Deployment Log Observability System

**Status**: Approved

**Date**: 2024-07-26

## Context

To ensure robust observability for our deployment processes, we need a system that can effectively record, view, and filter deployment logs for our Duke and Kerrigan services. This system will help us monitor, troubleshoot, and optimize our deployments, ultimately leading to improved performance and reliability.

## Decision

We will implement an observability platform, Artanis, which will:

1. **Record Logs**: Capture logs for each deployment of Duke and Kerrigan to GitHub.
2. **View Logs**: Provide capabilities to view logs in both tabular and graphical formats.
3. **Filter Logs**: Implement filters for logs by service, branch, and time period.

### Key Components

- **Logging Infrastructure**:
  - Utilize Knowvus (or a similar service) for log aggregation and storage.
  - Logs will be pushed to a central repository upon each deployment.

- **Frontend**:
  - Build a user interface to display logs in both tabular and graphical formats.
  - Implement filters for service, branch, and time period.

- **Backend**:
  - Set up APIs using `FastAPI` for log retrieval and filtering.
  - Implement logic for filtering logs based on the selected criteria.

- **Deployment**:
  - Deploy the observability platform on Digital Ocean.
  - Ensure secure and reliable access to the platform.

## Consequences

### Positive Outcomes

- Improved monitoring and troubleshooting capabilities for deployments.
- Enhanced visibility into deployment performance and issues.
- Ability to analyze logs in multiple formats (tabular and graphical) and filter them based on various criteria.

### Negative/Neutral Outcomes

- Additional complexity in maintaining the observability platform.
- Potential need for increased storage and computing resources to handle log aggregation and processing.

## Implementation

### Recommended Libraries

- **Logging**:
  - `loguru` (Python): Simplifies logging setup and configuration.
  - `winston` (Node.js): Versatile logging library for Node.js.

- **APIs**:
  - `FastAPI` (Python): High-performance web framework for building APIs.
  - `Express.js` (Node.js): Fast, unopinionated, minimalist web framework for Node.js.

- **Data Visualization**:
  - `Plotly` (Python, JavaScript): Interactive graphing library.
  - `D3.js` (JavaScript): Powerful library for producing dynamic and interactive data visualizations in web browsers.

- **Testing**:
  - `pytest` (Python): Framework makes it easy to write small tests, yet scales to support complex functional testing.
  - `Jest` (JavaScript): Delightful JavaScript Testing Framework with a focus on simplicity.

### Metrics to Observe for Performance

- **API Response Time**: Measure the time it takes for your APIs to respond.
- **Log Throughput**: The number of logs processed per second.
- **Error Rate**: The frequency of errors encountered during log processing.
- **System Load**: Monitor CPU and memory usage to ensure the system can handle the logging load.
- **Data Latency**: Time taken for logs to be available for querying after being generated.
- **Storage Utilization**: Monitor the amount of storage being used by the logging infrastructure.

### Best Practices

- **Use Structured Logging**: Ensure that logs are in a structured format (e.g., JSON) to make them easier to parse and analyze.
- **Centralize Logs**: Aggregate logs from all services and deployments into a single location for easy access and analysis.
- **Implement Log Rotation and Retention Policies**: To manage disk space usage, implement policies to rotate and delete old logs.
- **Ensure Security and Compliance**: Protect log data by ensuring it is encrypted in transit and at rest. Ensure that log management practices comply with relevant regulations and standards.
- **Automate Deployment and Monitoring**: Use CI/CD pipelines to automate the deployment of the logging infrastructure and setup automated monitoring and alerting for key metrics.
- **Regularly Review Logs**: Periodically review logs to ensure that logging is working correctly and to identify any potential issues or areas for improvement.

## Decision Makers

- **Author**: [Your Name]
- **Approvers**: [Approver Names]

## Links

- [Project Repository](https://github.com/your-repo/Artanis)
- [Knowvus Documentation](https://github.com/Knowvus/documentation)

---

This ADR should be reviewed and updated as the project evolves and new information becomes available.

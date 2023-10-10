# Write-up

## Analyze, Choose, and Justify the Appropriate Resource Option for Deploying the App.

### Appropriate Solution
I choose Azure App Service to deploy this exercise.

### Why I Chose App Service
- Azure App Service simplifies deployment. I don't need to worry about the underlying infrastructure, security, or networking. This allows me to focus solely on my application code and not worry about server management tasks.
- Deploying Flask applications to Azure App Service is straightforward. I can deploy directly from a Git repository, simplifying the deployment process and reducing downtime.
- Azure App Service integrates with various managed services like Azure SQL Database, simplifying database management.

### Why Not Virtual Machines
- Setting up and configuring VMs is complex, especially for those without expertise in server administration. You need to handle network configurations, security settings, and software installations.
- Unlike Azure App Service, VMs take more time to manage the entire infrastructure stack, resulting in slower application deployment.

### Justification Based on Cost, Scalability, Availability, and Workflow:

- Cost: With Azure App Service, you only pay for the resources you consume. It can be more cost-effective than running and managing VMs, especially for smaller to moderately sized applications like this Flask app.

- Scalability: Azure App Service makes it easy to scale the application vertically by adjusting the number of instances or horizontally using auto-scaling based on demand. This ensures that my Flask web app can handle varying levels of traffic without manual intervention.

- Availability: Azure App Service automatically load-balances incoming traffic across multiple instances, providing high availability and improved reliability.

- Workflow: Azure App Service supports automated deployments from GitHub, Azure DevOps, or any Git repository. With GitHub Actions for Azure web apps, developers can create workflows in GitHub repositories to build, test, package, release, and deploy to Azure.

# Write-up

## Analyze, choose, and justify the appropriate resource option for deploying the app.

### Appropriate solution
I choose Azure App Service to deploy this excercise.

### Why I choose App service
- Azure App service has a built-in infrastructure maintenance, security patching, and scaling.
- Azure App service Support multiple languages, such as .NET, .NET Core, Java,  PHP, Python,...
- Azure app service allows me to quickly build, deploy, and scale my web app

### Why not Virtual Machines
- I don't want to control the underlying Operating System or install a software on the server.
- Using App service I can quickly deploy my web application setup environment and right now i not enought knowleague to do all that.

### Justification based on cost, scalability, avaliability and workflow:

- Cost: Azure App service is less expensive than Virtual Machines. It provide different plans options such as Free and Shared (preview) plans to test or deploy an app

- Scalability: Azure provides developer with the possibility to easily scale his apps either horizontally or vertically. vertical scaling automatically increases or decreases resources allocated to our App Service, such as the amount of vCPUs or RAM, by changing the App Service pricing tier. Horizontal scaling increases or decreases the number of Virtual Machine instances our App Service is running.

- Availability: Global scale with high availability. Using App service I can host my app anywhere in Microsoft's global datacenter infrastructure, and the App Service SLA promises high availability.

- Workflow: Azure App service support automated deployments from GitHub, Azure DevOps, or any Git repository. With GitHub Actions for Azure web app, developer can create workflows in github repository to build, test, package, release and deploy to Azure. 


### Assess app changes that would change your decision.

- Azure app service has a hardware limitations. Also is not an appropriate solution for apps which have scope to expand for future. Instead, VMs are preferred. If this app grows to a larger scale, when we have vast increase in the number of users or when more features are added to the app, I would choose a Virtual Machine.

- For advanced scaling (auto) and traffic management features, I would go for VM.

- Using App service, I have limited access to the host server, if I want to control the underlying OS or install a software on the server, I have to choose Virtual Machine.
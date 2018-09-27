# Demo for integrated IaaS, PaaS, CaaS deployment options

This deploys a lot of infrastructure options to do proof of concepts on deploying workloads to different scenarios.

- Front Tier
- Backend Tier
- Microservice Tier
- Azure SQL
- Function Apps
- Web Apps
- API Gateway
- API Management

 ## Infrastructure Architecture

![[0]][0]


Single Region Deployment:  All resources deployed using a single region.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fdanielscholl%2Fazure-ipc-arch%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fdanielscholl%2Fazure-ipc-arch%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

 ### Manual Installation

__Setup Environment Variables__

Export environment variables required to use the install script.

>A great tool to do this automatically with is [direnv](https://direnv.net/).

```bash
export AZURE_SUBSCRIPTION="YOUR_SUBSCRIPTION_ID"
export AZURE_LOCATION="YOUR_REGION"
```

__Execute the Install__

```bash
install.sh
```



[0]: ./diagrams/architecture.png "Architecture Diagram"
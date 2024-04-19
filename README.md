# azure-containers-at-a-glance

| [App Service](appservice.md) | [Container Instances](containerinstancesmd)  | [Container Apps](containerapps.md) | [Spring Apps](springapps.md) | [Kubernetes Service](aks.md) | 
| --- | --- | --- | --- | --- |
| Fully managed hosting focused on web applications | Single pod of Hyper-V isolated containers on demand |Optimized for microservice containers | Spring Goodies | Full container orchestration management solution |
| Compute can either be multitenant (shared), single tenant (dedicated) or ASE | Compute is isolated by hypervisor isolation | The ACA Environment is the compute isolation boundary | Each Spring App Service is isolated compute | Compute is based on VMSS Clusters |
| App Service Plan can be scaled as a whole | Single pod, no scaling beyond defined sizing | Min/max replicas can be specified per pod | [Manual or Autoscale per App](https://learn.microsoft.com/en-us/azure/spring-apps/how-to-setup-autoscale) | Clusters and Pods can all scale individually |
| {::nomarkdown}<ul><li>Consumption/shared: no</li><li>Dedicated (basic, standard, premium): optional</li><li>ASEv3: deploys into VNet, (required)</li></ul>{:/} | Running on a defined Vnet only supported on Linux containers | The ACA Environment can have a Vnet associated with it | ASA can have a vnet associated with it | Cluster resides on a Vnet and can be run with either Kubenet or Azure CNI |
| Supports Windows and Linux Containers | Supports Windows and Linux Containers | Supports Linux Containers | Supports JARs or Linux Containers | Supports Windows and Linux Containers | 
| Zone Redundancy is available | Zone Redundancy available with Public networking | Zone Redundancy with VNet Integration | [Zone Redundancy with Standard or Enterprise SKU](https://learn.microsoft.com/en-us/azure/spring-apps/how-to-enable-redundancy-and-disaster-recovery?tabs=azure-cli) | Cluster nodes can be deployed to multiple Availability Zones |
| [SLA: 99.95%](https://azure.microsoft.com/en-us/support/legal/sla/app-service/v1_5/) | [SLA: 99.9%](https://azure.microsoft.com/en-us/support/legal/sla/container-instances/v1_0/) | [SLA: 99.95%](https://azure.microsoft.com/en-us/support/legal/sla/container-apps/v1_0/) | [SLA 99.9%](https://azure.microsoft.com/en-us/support/legal/sla/spring-apps/v1_0/) | [SLA: 99.95% if in AZ](https://azure.microsoft.com/en-us/support/legal/sla/kubernetes-service/v1_1/) |  
| [Architecture](https://github.com/Azure/appservice-landing-zone-accelerator) | Architecture Coming Soon | [Architecture](https://github.com/Azure/ACA-Landing-Zone-Accelerator) | [Architecture](https://github.com/Azure/azure-spring-apps-landing-zone-accelerator) | [Architecture](https://github.com/Azure/AKS-Landing-Zone-Accelerator/tree/main/Scenarios/AKS-Secure-Baseline-PrivateCluster) | 

***
Github Pages: https://scallighan.github.io/azure-containers-at-a-glance/

# azure-containers-at-a-glance

| [App Service](appservice.md) | [Container Instances](containerinstances.md)  | [Container Apps](containerapps.md) | [Kubernetes Service](aks.md) | 
| --- | --- | --- | --- |
| Fully managed hosting focused on web applications | Single pod of Hyper-V isolated containers on demand |Optimized for microservice containers | Full container orchestration management solution |
| Compute can either be multitenant (shared), single tenant (dedicated) or ASE | Compute is isolated by hypervisor isolation | The ACA Environment is the compute isolation boundary | Compute is based on VMSS Clusters |
| App Service Plan can be scaled as a whole | Single pod, no scaling beyond defined sizing | Min/max replicas can be specified per pod | Clusters and Pods can all scale individually |
| > **Consumption/shared:** no > **Dedicated (basic, standard, premium):** optional > **ASEv3:** deploys into VNet, (required) | Running on a defined Vnet only supported on Linux containers | The ACA Environment can have a Vnet associated with it | Cluster resides on a Vnet and can be run with either Kubenet or Azure CNI |
| Supports Windows and Linux Containers | Supports Windows and Linux Containers | Supports Linux Containers | Supports Windows and Linux Containers | 
| Zone Redundancy is available | Zone Redundancy available with Public networking | No Zone Redundancy at this time | Cluster nodes can be deployed to multiple Availability Zones |
| [SLA: 99.95%](https://azure.microsoft.com/en-us/support/legal/sla/app-service/v1_5/) | [SLA: 99.9%](https://azure.microsoft.com/en-us/support/legal/sla/container-instances/v1_0/) | [SLA: 99.95%](https://azure.microsoft.com/en-us/support/legal/sla/container-apps/v1_0/) | [SLA: 99.95% if in AZ](https://azure.microsoft.com/en-us/support/legal/sla/kubernetes-service/v1_1/) |  
| Architecture Coming Soon | Architecture Coming Soon | Architecture Coming Soon | [Architecture](https://github.com/Azure/AKS-Landing-Zone-Accelerator/tree/main/Scenarios/AKS-Secure-Baseline-PrivateCluster) | 

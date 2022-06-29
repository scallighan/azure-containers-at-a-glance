# azure-containers-at-a-glance

| App Service | Container Instances  | Container Apps | Kubernetes Service | 
| --- | --- | --- | --- |
| Fully managed hosting focused on web applications | Single pod of Hyper-V isolated containers on demand |Optimized for microservice containers | Full container orchestration management solution |
| Compute can either be multitenant (shared), single tenant (dedicated) or ASE | Compute is isolated by hypervisor isolation | The ACA Environment is the compute isolation boundary | Compute is based on VMSS Clusters |
| App Service Plan can be scaled as a whole | Single pod, no scaling beyond defined sizing | Min/max replicas can be specified per pod | Clusters and Pods can all scale individually |
| <ul><li>Consumption/shared: no</li><li>Dedicated (basic, standard, premium): optional</li><li>ASEv3: deploys into VNet, (required</li></ul> | Running on a defined Vnet only supported on Linux containers | The ACA Environment can have a Vnet associated with it | Cluster resides on a Vnet and can be run with either Kubenet or Azure CNI |


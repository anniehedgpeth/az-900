


# AZ-900 (updated June 2022)

# Describe Cloud Concepts (20 - 25%)

## Describe the benefits and considerations of using cloud services

| Term | description |
|---|---|
| [High availability](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/benefits-of-cloud-computing) | Occurs when multiple resources are deployed so that a system is available 99.99% of the time. For example, Azure creates availability sets for VMs to ensure that workloads are available almost all of the time. |
| [Scalability](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/benefits-of-cloud-computing) | Occurs when you can increase the number of VMs as more inbound requests arrives. This represents manual horizontal scaling. |
| [Elasticity](https://azure.microsoft.com/en-us/overview/what-is-elastic-computing/) | Elastic computing is the ability to quickly expand or decrease computer processing, memory, and storage resources to meet changing demands without worrying about capacity planning and engineering for peak usage. |
| [Agility](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/benefits-of-cloud-computing) | The ability to rapidly develop, test and launch software applications that drive business growth. Cloud Agility allows them to focus on other issues such as security, monitoring and analysis, instead of provisioning and maintaining the resources. |
| [Fault tolerance](https://docs.microsoft.com/en-us/learn/modules/cmu-disaster-recovery-backup/1-failures-fault-tolerance) | Occurs when a state-wide power outage in a region does not affect the ability of users to access data that was deployed to a datacenter in that state. Redundancy is built into the Azure architecture so that if a region fails, a paired region at least 300 miles away takes over. |
| [Disaster recovery](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/benefits-of-cloud-computing) | Occurs when you are able to retrieve data after it was lost due to some type of event. |
| [Economies of scale](https://en.wikipedia.org/wiki/Economies_of_scale) | Economies of scale is the ability to do things more efficiently or at a lower-cost per unit when operating at a larger scale (e.g. the ability to acquire hardware at a lower cost than if a single user or smaller business were purchasing it, cloud providers can also make deals with local governments and utilities to get tax savings, lower pricing on power, cooling, and high-speed network connectivity between sites). |

---

| term | description |
|---|---|
| [Capital Expenditure (CapEx)](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/benefits-of-cloud-computing) | CapEx is the spending of money on physical infrastructure up front, and then deducting that expense from your tax bill over time. CapEx is an upfront cost, which has a value that reduces over time.|
| [Operational Expenditure (OpEx)](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/benefits-of-cloud-computing) | OpEx is spending money on services or products now and being billed for them now. You can deduct this expense from your tax bill in the same year. |

* _understand the consumption-based model_ - With OpEx, there is no upfront cost, you pay for a service or product as you use it.

## Shared responsibility model in the cloud
 * As you consider and evaluate public cloud services, it’s critical to understand the [shared responsibility model](https://docs.microsoft.com/en-us/azure/security/fundamentals/shared-responsibility) and which security tasks are handled by the cloud provider and which tasks are handled by you. The workload responsibilities vary depending on whether the workload is hosted on Software as a Service (SaaS), Platform as a Service (PaaS), Infrastructure as a Service (IaaS), or in an on-premises datacenter
* In an on-premises datacenter, you own the whole stack. As you move to the cloud some responsibilities transfer to Microsoft. The following diagram illustrates the areas of responsibility between you and Microsoft, according to the type of deployment of your stack.

![Diagram showing responsibility zones.](https://docs.microsoft.com/en-us/azure/security/fundamentals/media/shared-responsibility/shared-responsibility.svg)
Regardless of the type of deployment, the following responsibilities are always retained by you:
* Data
* Endpoints
* Account
* Access management

## Describe the differences between Infrastructure-as-a-Service (IaaS), Platform-as-a-Service (PaaS) and Software-as-a-Service (SaaS)

* _[Infrastructure-as-a-Service (IaaS)](https://azure.microsoft.com/en-us/overview/what-is-iaas/)_ - IaaS quickly scales up and down with demand, letting you pay only for what you use. It helps you avoid the expense and complexity of buying and managing your own physical servers and other datacenter infrastructure. Each resource is offered as a separate service component, and you only need to rent a particular one for as long as you need it. A cloud computing service provider, such as Azure, manages the infrastructure, while you purchase, install, configure, and manage your own software—operating systems, middleware, and applications.
* _[Platform-as-a-Service (PaaS)](https://azure.microsoft.com/en-us/overview/what-is-paas/#overview)_ - PaaS is designed to support the complete web application lifecycle: building, testing, deploying, managing, and updating. PaaS allows you to avoid the expense and complexity of buying and managing software licenses, the underlying application infrastructure and middleware, container orchestrators such as Kubernetes, or the development tools and other resources. You manage the applications and services you develop, and the cloud service provider typically manages everything else.
* _[Software-as-a-Service (SaaS](https://azure.microsoft.com/en-us/overview/what-is-saas/#overview))_ - Software as a service (SaaS) allows users to connect to and use cloud-based apps over the Internet. Common examples are email, calendaring, and office tools (such as Microsoft Office 365). SaaS provides a complete software solution that you purchase on a pay-as-you-go basis from a cloud service provider. You rent the use of an app for your organization, and your users connect to it over the Internet, usually with a web browser. All of the underlying infrastructure, middleware, app software, and app data are located in the service provider’s data center. The service provider manages the hardware and software, and with the appropriate service agreement, will ensure the availability and the security of the app and your data as well. SaaS allows your organization to get quickly up and running with an app at minimal upfront cost.

## Serverless computing

| Term | Description |
|---|---|
| [Azure Functions](https://docs.microsoft.com/en-us/azure/azure-functions/functions-overview) | Provides a solution for building highly reliable and secure serverless apps suppporting multiple programming languages. You can build apps using simple serverless functions with the ability to scale as needed to meet demand. It enables you to focus on building apps without the concerns for server resources.|
| [Logic Apps](https://docs.microsoft.com/en-us/azure/logic-apps/logic-apps-overview) | A low-code/no-code GUI based cloud service designed to help you automate and orchestrate tasks, workflows, and business processes. Logic Apps is a serverless solution that lets you connect and coordinate systems and applications.| 
| [Event Grid](https://azure.microsoft.com/en-us/services/event-grid/) | Allows you to easily build applications with event-based architectures. It's a fully-managed, intelligent event routing service that uses a publish-subscribe model for uniform event consumption. |

---

## Describe the differences between public, private and hybrid cloud models
* [_Cloud computing_](https://azure.microsoft.com/en-us/overview/what-is-cloud-computing/) - Simply put, cloud computing is the delivery of computing services—including servers, storage, databases, networking, software, analytics, and intelligence—over the Internet (“the cloud”) to offer faster innovation, flexible resources, and economies of scale.
* [_Public cloud_](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/types-of-cloud-computing) - The solution is managed by a provider. MOst solutions are based on a multi-tenant model with the solution run in a shared environment with customer data partitioned to provide data security. MSFT Azure is an example of a public cloud.
* [_Private cloud_](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/types-of-cloud-computing) - An organization builds and maintains its own solution, either in its datacenter or hosted as dedicated resources by a solution provider. Services and infrastructure are hosted on a private network dedicated to that organization only. Government agencies and financial institutions often use the private cloud model. A private cloud requires access to be limited to one tenant A private cloud's services and infrastructure are maintained on a private network. A company can implement its own private cloud, but it is more common to subscribe to a private cloud hosted and managed by a third-party provider.
* [_Hybrid cloud_](https://docs.microsoft.com/en-us/learn/modules/fundamental-azure-concepts/types-of-cloud-computing) - This combines features of public and private clouds. This provides a way to save costs by sharing less-secure solutions needs in a public cloud and keeping high-risk, high-value resources internal to the network. A hybrid cloud provides support for a feature known as cloud bursting, where internal resources meet most needs but cloud-based resources can be added to help support peak use times.
* _compare and contrast the three different cloud models_

---

| | Advantages | Disadvantages |
|---|---|---|
| Public | + High Scalability/Agility <br/>+ PAYG (No CapEx, OpEx model)<br/>+ Minimal technical knowledge required<br/>+ Lower costs — no need to purchase hardware or software, and you pay only for the service you use.<br/>+ No maintenance — your service provider provides the maintenance.<br/>+ Near-unlimited scalability — on-demand resources are available to meet your business needs.<br/>+ High reliability — a vast network of servers ensures against failure.| - May not be able to meet specific security requirements | - May not be able to meet specific compliance requirements<br/>- You don't own the hardware and may not be able to manage them as you wish |
| Private | + You have complete control<br/>+ Can meet strict security and compliance requirements <br/>+ More flexibility — your organization can customize its cloud environment to meet specific business needs.<br/>+ Improved security — resources are not shared with others, so higher levels of control and security are possible.<br/>+ High scalability — private clouds still afford the scalability and efficiency of a public cloud.| - Upfront CapEx costs<br/>- Owning equipment limits agility to scale<br/>- Requires high technical knowledge |
| Hybrid | + Advantages of both Public and Private<br/>+ Control — your organization can maintain a private infrastructure for sensitive assets.<br/>+ Flexibility — you can take advantage of additional resources in the public cloud when you need them.<br/>+ Cost-effectiveness — with the ability to scale to the public cloud, you pay for extra computing power only when needed.<br/>+ Ease — transitioning to the cloud doesn’t have to be overwhelming because you can migrate gradually — phasing in workloads over time.| - Can be more expensive than selecting one deployment model<br/>- Can be more complicated to set up and manage|

# Describe Core Azure Services (15 - 20%)

## Describe the core Azure architectural components
| term | description |
|---|---|
| [Regions](https://docs.microsoft.com/en-us/azure/availability-zones/az-overview) | A region is a geographical area on the planet containing at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network.|
| [Regions Pairs](https://docs.microsoft.com/en-us/azure/best-practices-availability-paired-regions) | A region pair Each Azure region is paired with another region within the same geography (such as US, Europe, or Asia). Each Azure Region within a pair is physically / geographically located at least 300 miles apart where possible. |
| [Availability Zones](https://docs.microsoft.com/en-us/azure/availability-zones/az-overview) | Availability Zone is an isolated location inside of an Azure Region that has its own independent power source, network, and cooling. The physical and logical separation of Availability Zones within an Azure region protects applications and data from zone-level failures. Availability Zone data transfer pricing is based on Availability Zones. Azure availability zones are connected by a high-performance network with a round-trip latency of less than 2 ms|
|[Availability sets](https://docs.microsoft.com/en-us/azure/virtual-machines/availability-set-overview)|An availability set is a logical grouping of VMs that allows Azure to understand how your application is built to provide for redundancy and availability. We recommended that two or more VMs are created within an availability set to provide for a highly available application and to meet the 99.95% Azure SLA. There is no cost for the Availability Set itself, you only pay for each VM instance that you create.|
| [Resource Groups](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview#resource-groups) | Resource groups are a fundamental element of the Azure platform. A resource group is a logical container for resources deployed on Azure. |
| [Subscriptions](https://docs.microsoft.com/en-us/microsoft-365/enterprise/subscriptions-licenses-accounts-and-tenants-for-microsoft-cloud-offerings) | A subscription is an agreement with Microsoft to use one or more Microsoft cloud platforms or services, for which charges accrue based on either a per-user license fee or on cloud-based resource consumption. (Examples: Free trial, Student, Pay as you go, MSDN, etc..)|
| [Management Groups](https://docs.microsoft.com/en-us/azure/governance/management-groups/overview) | If your organization has many subscriptions, you may need a way to efficiently manage access, policies, and compliance for those subscriptions. Azure management groups provide a level of scope above subscriptions. You organize subscriptions into containers called "management groups" and apply your governance conditions to the management groups. All subscriptions within a management group automatically inherit the conditions applied to the management group. Management groups give you enterprise-grade management at a large scale no matter what type of subscriptions you might have. All subscriptions within a single management group must trust the same Azure Active Directory tenant. <br/><br/> Management levels and hierarchy <br/><br/> Azure provides four levels of management: management groups, subscriptions, resource groups, and resources. The following image shows the relationship between these levels. <br/><br/>![https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-setup-guide/media/organize-resources/scope-levels.png](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-setup-guide/media/organize-resources/scope-levels.png) <br/><br/> Each directory is given a single top-level management group called the root management group. The root management group is built into the hierarchy to have all management groups and subscriptions fold up to it. This root management group allows for global policies and Azure role assignments to be applied at the directory level. No one is given default access to the root management group. Azure AD Global Administrators are the only users that can elevate themselves to gain access. Once they have access to the root management group, the global administrators can assign any Azure role to other users to manage it. Any assignment of user access or policy on the root management group applies to all resources within the directory.<br/><br/> ![https://docs.microsoft.com/en-us/azure/governance/management-groups/media/tree.png](https://docs.microsoft.com/en-us/azure/governance/management-groups/media/tree.png) |
| [Azure Resource Manager](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview) | Azure Resource Manager is the interface for managing and organizing cloud resources. Think of Resource Manager as a way to deploy cloud resources.|
| [Azure resources](https://azure.microsoft.com/en-us/resources/) | Resources are any manageable item that is available through Azure. Virtual machines, storage accounts, web apps, databases, and virtual networks are examples of resources |

## Describe core resources available in Azure

| Compute resources | Description |
|---|---|
| [Virtual Machines](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/overview) | Windows or Linux virtual machines (VMs) hosted in Azure |
| [Virtual Machine Scale Sets](https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview) | Scaling for Windows or Linux VMs hosted in Azure |
|  [Azure App Service](https://docs.microsoft.com/en-us/azure/app-service/overview) | PaaS offerings to build, deploy, and scale enterprise-grade web, mobile, and API apps. |
| [Azure Container Instances (ACI)](https://docs.microsoft.com/en-us/azure/container-instances/container-instances-overview) | Run Docker containers on-demand in a managed, serverless Azure environment |
| [Azure Kubernetes Service (AKS)](https://docs.microsoft.com/en-us/azure/container-instances/container-instances-overview) | deploying a managed Kubernetes cluster in Azure by offloading the operational overhead to Azure. |
| [Azure Virtual Desktop](https://docs.microsoft.com/en-us/azure/virtual-desktop/overview) | Azure Virtual Desktop is a desktop and app virtualization service that runs on the cloud.|
||
---
| Networking resources | Description |
|---|---|
| [Virtual Network](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-networks-overview) | Connects VMs to incoming Virtual Private Network (VPN) connections |
|[Virtual Network peering](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-network-peering-overview) | Virtual network peering enables you to seamlessly connect two or more in Azure Virtual Networks. The virtual networks appear as one for connectivity purposes. The traffic between virtual machines in peered virtual networks uses the Microsoft backbone infrastructure. Like traffic between virtual machines in the same network, traffic is routed through Microsoft's _private_ network only.|
| [VPN Gateway](https://docs.microsoft.com/en-us/azure/vpn-gateway/vpn-gateway-about-vpngateways) | Accesses Azure Virtual Networks through high-performance VPN gateways. Azure VPN Gateway enables you to establish secure, cross-premises connectivity between your virtual network within Azure and on-premises IT infrastructure. |
|[ExpressRoute](https://docs.microsoft.com/en-us/azure/expressroute/expressroute-introduction) | ExpressRoute lets you extend your on-premises networks into the Microsoft cloud over a private connection with the help of a connectivity provider. With ExpressRoute, you can establish connections to Microsoft cloud services, such as Microsoft Azure and Microsoft 365. 
 
---
| Resource | Description | When to use |
|---|---|---|
| [Azure Blobs](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-overview) | Designed for storing very large quantities of unstructured data. Outside access to application data is supported, but data is stored and accessed as block blobs. Provides client libraries and a REST interface that allows unstructured data to be stored and accessed at a massive scale in block blobs. Also supports Azure Data Lake Storage Gen2 for enterprise big data analytics solutions. | You want your application to support streaming and random access scenarios. You want to be able to access application data from anywhere. You want to build an enterprise data lake on Azure and perform big data analytics.|
| [Disk Storage](https://docs.microsoft.com/en-us/azure/virtual-machines/managed-disks-overview) | Stores data as a virtual hard disk (VHD) that is available to the VM to which the disk is attached. This storage product does not provide any outside access. Provides client libraries and a REST interface that allows data to be persistently stored and accessed from an attached virtual hard disk. | You want to lift and shift applications that use native file system APIs to read and write data to persistent disks. You want to store data that is not required to be accessed from outside the virtual machine to which the disk is attached. |
| [File Storage](https://docs.microsoft.com/en-us/azure/storage/files/storage-files-introduction) | Access is provided to other VMs, as well as on-prem, through use of the Server Message Block (SMB) protocol, REST, and native client libraries. Provides an SMB interface, client libraries, and a REST interface that allows access from anywhere to stored files. | You want to "lift and shift" an application to the cloud which already uses the native file system APIs to share data between it and other applications running in Azure. You want to store development and debugging tools that need to be accessed from many virtual machines. |
|[Hot, Cool and Archive Access Storage Tier For Blob Data](https://docs.microsoft.com/en-us/azure/storage/blobs/access-tiers-overview)|**Hot tier:** An online tier optimized for storing data that is accessed or modified frequently. The Hot tier has the highest storage costs, but the lowest access costs. <br/><br/> **Cool tier:** An online tier optimized for storing data that is infrequently accessed or modified. Data in the Cool tier should be stored for a minimum of 30 days. The Cool tier has lower storage costs and higher access costs compared to the Hot tier. <br/><br/> **Archive tier:** An offline tier optimized for storing data that is rarely accessed, and that has flexible latency requirements, on the order of hours. Data in the Archive tier should be stored for a minimum of 180 days. This is provided as a low-cost storage option for data that is rarely accessed. You want to store logs that you don't need quick access to.|
---
| Database resources | Description |
|---|---|
| [CosmosDB](https://docs.microsoft.com/en-us/azure/cosmos-db/introduction) | Globally distributed database that supports NoSQL options |
| [Azure SQL Database](https://docs.microsoft.com/en-us/azure/azure-sql/database/sql-database-paas-overview) | PaaS offering that is fully managed relational database with auto-scale, integral intelligence, and robust security |
| [Azure Database for MySQL](https://docs.microsoft.com/en-us/azure/mysql/overview) | A relational database service powered by the MySQL community edition. It's a fully managed database as a service offering that can handle mission-critical workloads with predictable performance and dynamic scalability. |
| [Azure Database for PostgreSQL](https://docs.microsoft.com/en-us/azure/postgresql/overview) | A relational database service based on the open-source Postgres database engine. It's a fully managed database-as-a-service offering that can handle mission-critical workloads with predictable performance, security, high availability, and dynamic scalability. It's available in two deployment options, as a single server and as a Hyperscale (Citus) cluster. The Hyperscale (Citus) option horizontally scales queries across multiple machines using sharding, and serves applications that require greater scale and performance. |
|[SQL Managed Instance](https://docs.microsoft.com/en-us/azure/azure-sql/managed-instance/sql-managed-instance-paas-overview)| Microsoft managed PaaS offering that provides near 100% compatibility with the latest Microsoft SQL Server (Enterprise Edition) database engine, supports native VNet implementations that addresses common security concerns, and allow existing SQL Server customers to lift and shift their on-premises applications to the cloud with minimal application and database changes.|
---
| Marketplace resources | Description |
|---|---|
| [Azure Marketplace](https://docs.microsoft.com/en-us/marketplace/azure-marketplace-overview) | The Marketplace allows customers to find, try, purchase, and provision applications and services from thousands of leading service providers, all certified to run on Azure. Azure Marketplace is a service on Azure that helps connect end users with Microsoft partners, independent software vendors (ISVs), and start-ups that are offering their solutions and services, which are optimized to run on Azure. The catalog includes solutions for different industries and technical areas, free trials, and also consulting services from Microsoft partners.|
---
# Describe core solutions and management tools on Azure (10 - 15%)
### Internet of Things (IoT)

| Core Solution| Description |
|---|---|
| [IoT Hub](https://docs.microsoft.com/en-us/azure/iot-hub/iot-concepts-and-iot-hub) | A PaaS solution that requires you to write code to connect to IoT devices.|
| [IoT Central](https://docs.microsoft.com/en-us/azure/iot-central/core/overview-iot-central) | A global IoT SaaS solution which provides the means to connect to, monitor, and manage IoT resources. IoT Central is a SaaS solution that does not require any development experience. An application is completely hosted by MSFT, which eliminates the need for you to manage an IoT application.|
| [Azure Sphere](https://docs.microsoft.com/en-us/azure-sphere/product-overview/what-is-azure-sphere) | Azure Sphere is a high-level application platform used to securely monitor and manage IoT connected devices running the Azure Sphere OS.|

### Big Data and Analytics
| Core Solution| Description |
|---|---|
| [Azure Synapse Analytics](https://docs.microsoft.com/en-us/azure/synapse-analytics/overview-what-is) | Analytics service (using either serverless or dedicated options at scale) that brings together data integration, enterprise data warehousing, and big data analytics in unified experience to ingest, explore, prepare, transform, manage, and serve data for immediate business intelligence and machine learning needs. (This service was formerly known as Azure SQL Data Warehouse) |
|[HDInsight](https://docs.microsoft.com/en-us/azure/hdinsight/hdinsight-overview)| An open-source enterprise-level analytics service that provides for fast and cost-effective processing of massive amounts of data and supports a multitude of open-source analytic frameworks (Hadoop, Apache Spark, Apache Hive, LLAP, Apache Kafka, Apache Storm, R, etc). HDInsight can be used to analyze streaming or historic data. Scenarios for using HDInsight include extract, transform, and load (ETL) batch processing, interactive queries on data warehouses, machine learning, and processing streams of Internet of Things (IOT) data.|
|[Databricks](https://docs.microsoft.com/en-us/azure/databricks/scenarios/what-is-azure-databricks)|An Apache Spark-based analytics platform. You can think of it as "Spark as a service." It's the easiest way to use Spark on the Azure platform. It manages the Spark cluster for you. Azure Databricks is comprised of three environments (Databricks SQL, Databricks Data Science & Engineering, and Databricks Machine Learning) for developing data intensive applications.|
---
### Artificial Intelligence (AI) and automation
| Core Solution| Description |
|---|---|
| [Azure Machine Learning Service](https://docs.microsoft.com/en-us/azure/machine-learning/overview-what-is-azure-machine-learning) | A data science solution that enables computers to predict outcomes and trends without being explicitly programmed. It is a cloud service to train, deploy, automate, and manage machine learning models. It is designed to let you start training on a local computer and then scale out to the cloud. Machine learning models created in Machine Learning Studio cannot be deployed or managed by Azure Machine Learning Service.|
|[Cognitive Services](https://docs.microsoft.com/en-us/azure/cognitive-services/what-are-cognitive-services)| Cloud-based services with REST APIs and client library SDKs that allow developers to add cognitive features (see, hear, speak, understand, and even make decisions) within applications without having artificial intelligence (AI) or data science skills.|
|[Azure Bot Service](https://docs.microsoft.com/en-us/azure/bot-service/?view=azure-bot-service-4.0)| Provides an integrated environment for the development of bots.|
| [Azure Functions](https://docs.microsoft.com/en-us/azure/azure-functions/functions-overview) | An event-driven, serverless compute service |
|[Azure Logic Apps](https://docs.microsoft.com/en-us/azure/logic-apps/logic-apps-overview)|Allows for the creation and running or automated workflows that integrate your apps, data, services, and systems. Azure Logic Apps simplifies the way that you connect legacy, modern, and cutting-edge systems across cloud, on premises, and hybrid environments.|
---
### DevOps solutions
| Core Solution| Description |
|---|---|
| [Azure DevOps](https://docs.microsoft.com/en-us/devops/what-is-devops) | Provides version control, reporting, requirements management, project management, automated builds, lab management, testing and release management capabilities. It covers the entire application lifecycle, and enables DevOps capabilities. |
|[GitHub](https://docs.github.com/en)| Provides Internet hosting for distributed source code version control and source code management (SCM) functionality using Git. It also provides access control to Git resources and several collaboration features including bug tracking, feature requests, task management, continuous integration and wikis for projects.|
| [GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions)| Supplements continuous integration / continuous deployment (CI/CD) by allowing users to automate, customize, and execute software development actions within their pipelines from within Github repositories. *(For example, you can run a workflow to automatically add the appropriate labels whenever someone creates a new issue in your repository.)*|
| [Azure DevTest Labs](https://docs.microsoft.com/en-us/azure/devtest-labs/devtest-lab-overview) | Creates labs consisting of pre-configured bases or Azure Resource Manager templates. These have all the necessary tools and software that you can use to create environments. You can create environments in a few minutes, as opposed to hours or days. |
---
## Describe Azure management tools
| Management Tool| Description |
|---|---|
| [Azure Portal](https://docs.microsoft.com/en-us/azure/azure-portal/azure-portal-overview) | Azure CLI is a cross-platform command-line program that connects to Azure and executes administrative commands on Azure resources. Cross-platform means that it can be run on Windows, Linux, or macOS. |
| [Azure Powershell](https://docs.microsoft.com/en-us/powershell/azure/what-is-azure-powershell) | Azure PowerShell is a module that you add to Windows PowerShell or PowerShell Core that enables you to connect to your Azure subscription and manage resources. <br/> Example command: Connect-AzAccount |
| [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/what-is-azure-cli) | The Azure command-line interface (CLI) is Microsoft's cross-platform command-line experience for managing Azure resources. The Azure CLI is designed to be easy to learn and get started with, but powerful enough to be a great tool for building custom automation to use Azure resources.  <br/> Example command: az account show
| [Cloud Shell](https://docs.microsoft.com/en-us/azure/cloud-shell/overview) | Azure Cloud Shell is an interactive, authenticated, browser-accessible shell for managing Azure resources. It provides the flexibility of choosing the shell experience that best suits the way you work, either Bash or PowerShell. <br/> Example command: az account show |
| [Azure Mobile App](https://azure.microsoft.com/en-us/get-started/azure-portal/mobile-app/)| An iOS / Android mobile app that allows users to monitor, manage and recieve alerts for Azure resources. It also provides the ability to perform tasks via the Azure Cloud Shell as well as Azure CLI.|
| [Azure Advisor](https://docs.microsoft.com/en-us/azure/advisor/advisor-overview)| Azure Advisor provides you with a consistent, consolidated view of recommendations for all your Azure resources. It integrates with Azure Security Center to bring you security recommendations. You can get security recommendations from the Security tab on the Advisor dashboard. Security Center helps you prevent, detect, and respond to threats with increased visibility into and control over the security of your Azure resources. It periodically analyzes the security state of your Azure resources. When Security Center identifies potential security vulnerabilities, it creates recommendations. The recommendations guide you through the process of configuring the controls you need.|
| [Azure Resource Manager (ARM) templates](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview) | Azure Resource Manager templates are JSON files that define the infrastructure and configuration for your project.|
| [Azure Monitor](https://docs.microsoft.com/en-us/azure/azure-monitor/overview)| Azure Monitor maximizes the availability and performance of your applications and services by delivering a comprehensive solution for collecting, analyzing, and acting on telemetry from your cloud and on-premises environments. It helps you understand how your applications are performing and proactively identifies issues affecting them and the resources they depend on. <br/><br/>Just a few examples of what you can do with Azure Monitor include:<br/> * Detect and diagnose issues across applications and dependencies with Application Insights.<br/> * Correlate infrastructure issues with Azure Monitor for VMs and Azure Monitor for Containers.<br/> * Drill into your monitoring data with Log Analytics for troubleshooting and deep diagnostics.<br/> * Support operations at scale with smart alerts and automated actions. <br/> * Create visualizations with Azure dashboards and workbooks.
|[Azure Service Health](https://docs.microsoft.com/en-us/azure/service-health/overview)|Azure Service Health is a suite of experiences that provide personalized guidance and support when issues in Azure services are or may affect you in the future. Azure Service Health is composed of Azure status, the service health service, and Resource Health.<br/> <br/>Azure Service Health is a combination of three separate smaller services:<br/>1. [Azure status](https://docs.microsoft.com/en-us/azure/service-health/azure-status-overview) informs you of service outages in Azure on the [Azure Status page](https://status.azure.com) <br/>2. [Service health](https://docs.microsoft.com/en-us/azure/service-health/service-health-overview) provides a personalized view of the health of the Azure services and regions you're using.<br/>3. [Resource health](https://docs.microsoft.com/en-us/azure/service-health/resource-health-overview) provides information about the health of your individual cloud resources such as a specific virtual machine instance.

# Describe general security and network security features (10 - 15%)
| Security Feature| Description |
|---|---|
| [Defender for Cloud](https://docs.microsoft.com/en-us/azure/defender-for-cloud/defender-for-cloud-introduction) | Defender for Cloud (formerly called Azure Security Center) is a monitoring service tool that provides threat protection across all of your services both in Azure, and on-premises and in other clouds due to integration with  [Azure Defender](https://aka.ms/azuredefender). Available in two tiers, Free (limited to assessments and recommendations only); Standard (full suite of security-related services including continious monitoring, threat detection and just-in-time access control)<br/>_Usage scenarios:_<br/>&bull; Incident Response (Detect, Assess, Diagnose)<br/>&bull; Implement Recommendations <br/><br/> **Key features include:**<br/>&bull; **Compliance dashboard** - Compares the configuration of your resources against requirements outlined within in industry standards, [regulations](https://docs.microsoft.com/en-us/azure/defender-for-cloud/update-regulatory-compliance-packages), and [benchmarks](https://docs.microsoft.com/en-us/security/benchmark/azure/overview).   <br/>&bull; **Security alerts** - When Defender for Cloud detects a threat in any area of your environment, it generates a security alert. These alerts describe details of the affected resources, suggested remediation steps, and in some cases an option to trigger a logic app in response.  <br/>&bull; **Secure score** - A single score so that you can tell, at a glance, your current security situation (the higher the score, the lower the identified risk level). You can view your overall Secure score across your subscriptions or management groups, depending on the scope you select. The score is calculated based on the ratio between your healthy resources and your total resources and will vary based on subscription selected and the active recommendations on these subscriptions. <br/> &bull; **Resource security hygiene** - Most prevalent recommendations and highest impact recommendations.|
| [Key Vault](https://docs.microsoft.com/en-us/azure/key-vault/general/overview) | Azure Key Vault is a secret store: a centralized cloud service for key management, secret management, certificate management, and storing secrets supported by hardware models. Key Vault helps you control your applications’ secrets by keeping them in a single central location and providing secure access, permissions control, and access logging.
|[Azure Sentinel](https://docs.microsoft.com/en-us/azure/sentinel/overview)|Microsoft Sentinel is a scalable, cloud-native, security information event management (SIEM) and security orchestration automated response (SOAR) solution. Microsoft Sentinel delivers intelligent security analytics and threat intelligence across the enterprise, providing a single solution for alert detection, threat visibility, proactive hunting, and threat response.<br/><br/>  **Key features include:** <br/> &bull;  **Collect data at cloud scale** across all users, devices, applications, and infrastructure, both on-premises and in multiple clouds. <br/> &bull;  **Detect previously undetected threats**, and minimize false positives using Microsoft's analytics and unparalleled threat intelligence. <br/> &bull; **Investigate threats with artificial intelligence**, and hunt for suspicious activities at scale, tapping into years of cyber security work at Microsoft. <br/> &bull; **Respond to incidents rapidly** with built-in orchestration and automation of common tasks.|
|[Azure Dedicated Hosts](https://docs.microsoft.com/en-us/azure/virtual-machines/dedicated-hosts)|Azure Dedicated Host is a service that provides physical servers - able to host one or more virtual machines - dedicated to one Azure subscription. Dedicated hosts are the same physical servers used in our data centers, provided as a resource. You can provision dedicated hosts within a region, availability zone, and fault domain. Then, you can place VMs directly into your provisioned hosts, in whatever configuration best meets your needs. <br/><br/>Reserving the entire host provides the following benefits:<br/> &bull;  Hardware isolation at the physical server level. No other VMs will be placed on your hosts. Dedicated hosts are deployed in the same data centers and share the same network and underlying storage infrastructure as other, non-isolated hosts. <br/> &bull; Control over maintenance events initiated by the Azure platform. While the majority of maintenance events have little to no impact on your virtual machines, there are some sensitive workloads where each second of pause can have an impact. With dedicated hosts, you can opt-in to a maintenance window to reduce the impact to your service. <br/> &bull; With the Azure hybrid benefit, you can bring your own licenses for Windows and SQL to Azure. Using the hybrid benefits provides you with additional benefits.|
---
| Network Security Feature| Description |
|---|---|
| [Defense in Depth](https://docs.microsoft.com/en-us/learn/modules/azure-well-architected-security/2-defense-in-depth)| Defense in depth is a strategy that employs a series of mechanisms to slow the advance of an attack that's aimed at acquiring unauthorized access to information. Each layer provides protection so that if one layer is breached, a subsequent layer is already in place to prevent further exposure.|
| [Network Security Groups (NSG)](https://docs.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview) | NSGs operate at layers 3 & 4, and provide a list of allowed and denied communication to and from network interfaces and subnets. NSGs are fully customizable, and give you the ability to fully lock down network communication to and from your virtual machines. By using NSGs, you can isolate applications between environments, tiers, and services. ***Note: NSGs uses static IP addresses and as your network scales this may become difficult to maintain.*** |
| [Application Security Groups (ASG)](https://docs.microsoft.com/en-us/azure/virtual-network/application-security-groups)|Application Security Groups (ASG) are a feature within Azure that helps simplify the management of Network Security Group (NSG) rules. Application security groups enable you to configure network security as a natural extension of an application's structure, ***allowing you to group virtual machines and define network security policies based on those groups***. You can reuse your security policy at scale without manual maintenance of explicit IP addresses.|
| [Azure Firewall](https://docs.microsoft.com/en-us/azure/firewall/overview) | Azure Firewall is a managed, cloud-based, network security service that protects your Azure Virtual Network resources. It is a fully stateful firewall as a service with built-in high availability and unrestricted cloud scalability. Azure Firewall provides inbound protection for non-HTTP/S protocols. Examples of non-HTTP/S protocols include: Remote Desktop Protocol (RDP), Secure Shell (SSH), and File Transfer Protocol (FTP). It also provides outbound, network-level protection for all ports and protocols, and application-level protection for outbound HTTP/S. |
| [Azure DDoS Protection](https://docs.microsoft.com/en-us/azure/ddos-protection/ddos-protection-overview) | DDoS Protection leverages the scale and elasticity of Microsoft’s global network to bring DDoS mitigation capacity to every Azure region. The Azure DDoS Protection service protects your Azure applications by scrubbing traffic at the Azure network edge before it can impact your service's availability. Within a few minutes of attack detection, you are notified using Azure Monitor metrics.<br/><br/> Comes in two versions: <br/> Azure DDoS Protection Basic (*Free*)<br/> Azure DDoS Protection Standard (*provides SLAs for Application and Cost Protection*) <br/><br/> Every property in Azure is protected by Azure's infrastructure DDoS (Basic) Protection at no additional cost and requires no user configuration or application changes. <br/> ![](https://docs.microsoft.com/en-us/azure/ddos-protection/media/ddos-protection-overview/ddos-comparison.png)|
---
# Describe identity, governance, privacy, and compliance features (15 - 20%)
## Describe core Azure identity services
| Azure identity services | Description |
|---|---|
| [Authentication](https://docs.microsoft.com/en-us/azure/active-directory/develop/authentication-vs-authorization) (Who are you?) | The process of establishing the identity of a person or service looking to access a resource. It involves the act of challenging a party for legitimate credentials, and provides the basis for creating a security principal for identity and access control use. It establishes if they are who they say they are. |
| [Authorization](https://docs.microsoft.com/en-us/azure/active-directory/develop/authentication-vs-authorization) (What are you allowed to do?) | The process of establishing what level of access an authenticated person or service has. It specifies what data they're allowed to access and what they can do with it. |
| [Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-whatis) | Azure AD is a cloud-based identity service. It has built in support for synchronizing with your existing on-premises Active Directory or can be used stand-alone. This means that all your applications, whether on-premises, in the cloud (including Office 365), or even mobile can share the same credentials. Administrators and developers can control access to internal and external data and applications using centralized rules and policies configured in Azure AD. To manage resources in Azure AD, such as users, groups, and domains, there are several Azure AD administrator roles. |
| [Conditional Access](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) | Allows access to a resources based on meeting one or more predefined criteria|
| [Azure Multi-Factor Authentication](https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks) | Multi-factor authentication (MFA) provides additional security for your identities by requiring two or more elements for full authentication. These elements fall into three categories: <br/>  - Something you know<br/>  - Something you possess<br/>  - Something you are |
| [Single Sign-On (SSO)](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/what-is-single-sign-on) | Single sign-on is an authentication method that allows users to sign in using one set of credentials to multiple independent software systems. Choosing an SSO method depends on how the application is configured for authentication. Cloud applications can use federation-based options, such as OpenID Connect, OAuth, and SAML. The application can also use password-based SSO, linked-based SSO, or SSO can be disabled.|

| Authentication type | Supports MFA | Supports SSPR |
|---|---|---|
| Password | yes | yes |
| SMS |  yes | yes |
| Voice Call | yes | yes |
| App Passwords | sometimes | no |
| MSFT Authenticator | yes | yes |
| OATH Hardware token | Public Preview | yes |
| Security Questions | no | yes |
| Email address | no | yes |

## Describe Azure governance features
| Governance feature | Description |
|---|---|
| [Azure Role-Based Access Control (RBAC](https://docs.microsoft.com/en-us/azure/role-based-access-control/overview)) | Azure RBAC is a newer authorization system that provides fine-grained access management to Azure resources. RBAC includes many built-in roles, can be assigned at different scopes, and allows you to create your own custom roles. The way you control access to resources using RBAC is to create role assignments. This is a key concept to understand – it’s how permissions are enforced. A role assignment consists of three elements: security principal, role definition, and scope.
| [Resource locks](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/lock-resources) | As an administrator, you can lock a subscription, resource group, or resource to prevent other users in your organization from accidentally deleting or modifying critical resources. The lock overrides any permissions the user might have. <br/> <br/> You can set the lock level to **CanNotDelete** or **ReadOnly**. *In the portal, the locks are called **Delete** and **Read-only** respectively.* <br/>  &bull; **CanNotDelete** means authorized users can still read and modify a resource, but they can't delete the resource.  <br/> &bull; **ReadOnly** means authorized users can read a resource, but they can't delete or update the resource. Applying this lock is similar to restricting all authorized users to the permissions granted by the **Reader** role.|
| [Tags](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/tag-resources)| You apply tags to your Azure resources, resource groups, and subscriptions to logically organize them into a taxonomy. Each tag consists of a name and a value pair. For example, you can apply the name _Environment_ and the value _Production_ to all the resources in production.| 
| [Azure Policy](https://docs.microsoft.com/en-us/azure/governance/policy/overview) | Used to enforce tagging rules and conventions. By creating a policy, you avoid the scenario of resources being deployed to your subscription that don't have the expected tags for your organization. Instead of manually applying tags or searching for resources that aren't compliant, you create a policy that automatically applies the needed tags during deployment.| 
| [Azure Policy Initiative](https://docs.microsoft.com/en-us/azure/governance/policy/overview?WT.mc_id=itopstalk-blog-phschmit)|An initiative definition is a collection of policy definitions that are tailored toward achieving a singular overarching goal. Initiative definitions simplify managing and assigning policy definitions. They simplify by grouping a set of policies as one single item.|
| [Azure Blueprints](https://docs.microsoft.com/en-us/azure/governance/blueprints/overview)| Enables cloud architects and central information technology groups to define a repeatable set of Azure resources that implements and adheres to an organization's standards, patterns, and requirements. Azure Blueprints makes it possible for development teams to rapidly build and stand up new environments with trust they're building within organizational compliance with a set of built-in components, such as networking, to speed up development and delivery.<br/> <br/>  Blueprints are a declarative way to orchestrate the deployment of various resource templates and other artifacts such as:<br/> &bull;  Role Assignments <br/> &bull; Policy Assignments <br/> &bull;  Azure Resource Manager templates (ARM templates) <br/> &bull; Resource Groups| <br/> &bull;
| [Cloud Adoption Framework for Azure](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/overview) | The Microsoft Cloud Adoption Framework (CAF) for Azure is guidance that's designed to help you create and implement business and technology strategies for the cloud based on best practices, documentation, and tools.|

## Describe privacy and compliance resources
| Privacy and Compliance Resources | Description |
|---|---|
| Describe the Microsoft core tenets of Security, Privacy, and Compliance |[Watch this YouTube video](https://www.youtube.com/watch?v=zBzsDYZw98M)|
| [Microsoft Privacy Statement](https://docs.microsoft.com/en-us/learn/modules/examine-privacy-compliance-data-protection-standards/3-access-microsoft-privacy-statement)| Details collection, purpose and usage of personal data for all Microsoft offerings|
| [Online Services Terms (OST)](https://docs.microsoft.com/en-us/learn/modules/examine-privacy-compliance-data-protection-standards/3-access-microsoft-privacy-statement) | Provides license terms (use rights) for Microsoft online products and services.|
| [Data Protection Amendment (DPA)](https://docs.microsoft.com/en-us/learn/modules/examine-privacy-compliance-data-protection-standards/3-access-microsoft-privacy-statement)| Provides in-depth specification on processing and security of personal and customer data as well as obligations of the customer and Microsoft. <br/><br/>The Data Protection Addendum (DPA) further defines the data processing and security terms for online services. These terms include:<br/> &bull; Compliance with laws.<br/> &bull; Disclosure of processed data. <br/> &bull; Data Security, which includes security practices and policies, data encryption, data access, customer responsibilities, and compliance with auditing. <br/> &bull; Data transfer, retention, and deletion.|
| [Trust Center](https://docs.microsoft.com/en-us/learn/modules/examine-privacy-compliance-data-protection-standards/4-explore-trust-center) |A single place for organizations to review security, privacy and compliance of Microsoft online services. [Service Trust Portal](https://servicetrust.microsoft.com/)|
| [Azure compliance documentation](https://docs.microsoft.com/en-us/learn/modules/examine-privacy-compliance-data-protection-standards/5-access-azure-compliance-documentation) | The Azure compliance documentation provides you with detailed documentation about legal and regulatory standards and compliance on Azure. These compliance documents relate to the following: <br/> &bull; Global <br/> &bull; US government <br/> &bull; Financial services <br/> &bull; Health <br/> &bull; Media and manufacturing <br/> &bull; Regional|
| Azure Sovereign Regions | Provides Azure services in markets with very strick regulatory requirements (e.g. Azure (US) Government Cloud and China)|
---

# Describe Azure cost management and Service Level Agreements (10 - 15%)

### Describe methods for planning and managing costs
## Identify factors that affecting costs:
* **Resource Type:** Costs are resource-specific, so the usage that a meter tracks and the number of meters associated with a resource depend on the resource type.
  * **Service:** Azure usage rates and billing periods can differ between Enterprise, Web Direct, and Cloud Solution Provider (CSP) customers. Some subscription types also include usage allowances, which affect costs.
  * **Location:** Azure has datacenters all over the world. Usage costs vary between locations that offer particular Azure products, services, and resources based on popularity, demand, and local infrastructure costs.
  * **Ingress and egress traffic -**
    * Following Availability Zone data transfer is charged:
      * Data transfer, ingress and egress, from a VNet resource deployed in an Availability Zone to another resource in different Availability Zone in the same VNET
    * Following Availability Zone data transfer is NOT charged:
      * Data transfer between VNet resources located in same Availability Zone
      * Data transfer between a VNet resource and a Public IP address in the same Azure Region
      * Data transfer between VNet resources located in peered VNets across Availability Zones. This data transfer will be charges as per VNet peering rates.
* **Zones for billing** - A zone is a geographical grouping of Azure regions used to determine billing based on data transfers. Billing applies to both incoming and outgoing data and varies by zone.  Data transfers between zones and regions in a zone are billed. Data transfers between zones in the same region are not charged. Zones do not impact any other billing factors.

## Identify factors that reduce costs:
  * ***[Azure reservations](https://docs.microsoft.com/en-us/azure/cost-management-billing/reservations/save-compute-costs-reservations)*** - Reserved instances are pre-purchased in **one-year or three-year terms**, with payment required for the full term up front. After it's purchased, Microsoft matches up the reservation to running instances and decrements the hours from your reservation. Reservations can be purchased through the Azure portal. And because reserved instances are a compute discount, they are available for both Windows and Linux VMs.
  * ***[Reserved capacity](https://azure.microsoft.com/en-us/pricing/reserved-capacity/)*** - Pre-purchased Azure capacity resources that do not require (but support) one-year or three-year terms. 
  * ***[Azure hybrid use benefit](https://azure.microsoft.com/en-us/pricing/hybrid-benefit/)*** - Azure Hybrid Benefit is a licensing benefit that helps you to significantly reduce the costs of running your workloads in the cloud. It works by letting you use your on-premises Software Assurance-enabled Windows Server and SQL Server licenses on Azure. And now, this benefit applies to RedHat and SUSE Linux subscriptions, too.
  * ***[Azure Spot Virtual Machines](https://azure.microsoft.com/en-us/services/virtual-machines/spot/)*** - Use Spot Virtual Machines to buy unused compute capacity at significant cost savings. Deploy workloads that can handle interruptions and don't need to be completed within a specific period of time at a very low cost.
----
* **_Function and use of the [Pricing calculator](https://azure.microsoft.com/en-us/pricing/)_** - The Azure pricing calculator is a free web-based tool that allows you to input Azure services and modify properties and options of the services. It outputs the costs per service and total cost for the full estimate.
* **_Function and use of the [Total Cost of Ownership (TCO) Calculator](https://azure.microsoft.com/en-us/pricing/tco/calculator/)_** - If you are starting to migrate to the cloud, a useful tool you can use to predict your cost savings is the Total Cost of Ownership (TCO) calculator. TCO helps you estimate cost savings realized by mirating to Azure.
* **_Best practices for minimizing Azure costs_:**
  * *[Performing cost analysis](https://docs.microsoft.com/en-us/azure/cost-management-billing/costs/cost-analysis-common-uses)* -
  * *[Creating spending limits and quotas](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/azure-subscription-service-limits)* - Spending limit in Azure exists to prevent spending over your credit amount. All new customers who sign up for the trial or offers that includes credits over multiple months have the spending limit turned on by default. The spending limit is $0. It can’t be changed. The spending limit isn’t available for subscription types such as Pay-As-You-Go subscriptions and commitment plans.
  * *Using tags to identify cost owners* - You can use tags to group your billing data. For example, if you're running multiple VMs for different organizations, use the tags to group usage by cost center. You can also use tags to categorize costs by runtime environment, such as the billing usage for VMs running in the production environment. When exporting billing data or accessing it through billing APIs, tags are included in that data and can be used to further slice your data from a cost perspective.
* **_Function and use of the [Azure Cost Management](https://docs.microsoft.com/en-us/azure/cost-management-billing/cost-management-billing-overview)_** - Azure Cost Management is another free, built-in Azure tool that can be used to gain greater insights into where your cloud money is going. You can see historical breakdowns of what services you are spending your money on and how it is tracking against budgets that you have set. You can set budgets, schedule reports, and analyze your cost areas.
---
## Describe Azure Service Level Agreements (SLAs) and service lifecycles
* **_Purpose of an [Azure Service Level Agreement (SLA)](https://azure.microsoft.com/en-us/support/legal/sla/summary/)_** - Formal documents called Service-Level Agreements (SLAs) capture the specific terms that define the performance standards that apply to Azure. SLAs describe Microsoft's commitment to providing Azure customers with specific performance standards. There are SLAs for individual Azure products and services. SLAs also specify what happens if a service or product fails to perform to a governing SLA's specification. Note: Azure does not provide SLAs for most services under the Free or Shared tiers.
 * [YouTube: Identify actions that can impact an SLA (i.e. Availability Zones)](https://www.youtube.com/watch?v=WuzpcMZ1UxI) 
* **_Composite SLAs_** - When combining SLAs across different service offerings, the resultant SLA is a called a Composite SLA. The resulting composite SLA can provide higher or lower uptime values, depending on your application architecture.
* **_How to determine an appropriate SLA for an application_** - There are three key characteristics of SLAs for Azure products and services:
  * Performance Targets
  * Uptime and Connectivity Guarantees
  * Service credits (percentage of the applicable monthly service fees credited to you if a service fails to meet uptime guarantee)

| SLA % | Downtime per year |
|---|---|
| 99.99 | 52m 35s (about 1 hour) |
| 99.95 | 4h 22m 58s (about 4.5 hours)|
| 99 | 3d 15h 39m 29s (about 3.5 days)|

## Understand service lifecycle in Azure

| Term | Description |
|---|---|
| Public | This means that an Azure feature is available to all Azure customers for evaluation purposes. These previews can be turned on through the preview features page as detailed below.|
| Private | This means that an Azure feature is available to *specific* Azure customers for evaluation purposes. This is typically by invite only and issued directly by the product team responsible for the feature or service.|
| General Availability (GA) | Once a feature has been evaluated and tested successfully, it might be released to customers as part of Azure's default product set. This release is referred to as General Availability (GA). |

* _To monitor feature updates and product changes_ - The Azure portal "What's New" link on the ? help menu provides a list of recent updates you can periodically check to see what's changed in Azure. Alternatively, you can use the Azure Updates page (https://azure.microsoft.com/updates/).
---
# Extra stuff I saw on practice exams

## Understand Azure subscriptions

* _describe an Azure subscription_ - An Azure subscription is a logical container used to provision resources in Microsoft Azure. It holds the details of all your resources like virtual machines, databases, etc.
* _understand the uses and options with Azure subscriptions such access control and offer types_ - Azure offers free and paid subscription options to suit different needs and requirements. The most commonly used subscriptions are:
  * Free: An Azure free subscription includes a $200 credit to spend on any service for the first **30 days**, free access to the most popular Azure products for 12 months, and access to more than 25 products that are always free.
  * Pay-As-You-Go: A Pay-As-You-Go (PAYG) subscription charges you monthly for the services you used in that billing period. This subscription type is appropriate for a wide range of users, from individuals to small businesses, and many large organizations as well.
  * Enterprise Agreement: An Enterprise Agreement (EA) provides flexibility to buy cloud services and software licenses under one agreement, with discounts for new licenses and Software Assurance. It's targeted at enterprise-scale organizations.
  * Student: An Azure for Students subscription includes $100 in Azure credits to be used within the first 12 months plus select free services without requiring a credit card at sign-up. You must verify your student status through your organizational email address.

  * Every Azure Subscription Includes
    * Free access to billing and subscription support
    * Azure products and services documentation
    * Online self-help documentation
    * Community support forums

  * Purchasing Options for Azure Products and Services
    * Enterprise: Enterprise customers sign an Enterprise Agreement (EA) with Azure that commits them to spend a negotiated amount on Azure services, which they typically pay annually. Enterprise customers also have access to customized Azure pricing.
    * Web direct: Direct Web customers pay general public prices for Azure resources, and their monthly billing and payments occur through the Azure website.
    * Cloud Solution Provider: Cloud Solution Provider (CSP) typically are Microsoft partner companies that a customer hires to build solutions on top of Azure. Payment and billing for Azure usage occur through the customer's CSP.
---
### Supplemental material that I found useful

**John Savill's** - How to prep for the AZ-900 Exam (Watch only the first 20 minutes)
https://www.youtube.com/watch?v=0sHvssrWytM

Download the exams skills outline PDF on this page in the "Skills measured" section. 
https://docs.microsoft.com/en-us/learn/certifications/exams/az-900

**Adam Marczak** - AZ-900 training (*This course is one of most comprehensive and easy to understand AZ-900 training courses that I found. I highly recommend watching all of these videos once, and then re-watching videos associated with content listed in the "Skills measured".*)
https://marczak.io/az-900/

**Tim Warner** - AZ-900 Playlist (*This guy has some great material but is geared towards folks with less IT experience*.)
https://www.youtube.com/watch?v=HfZ1kgHlrfg&list=PLYGZ9Q0oTOHfsI-3IAhvyc09ssPDfoePv

[Microsoft Learning -  Microsoft Certified Trainer (MCT) lab for AZ-900](https://microsoftlearning.github.io/AZ-900T0x-MicrosoftAzureFundamentals/)

[Microsoft Learning - Microsoft Certified Trainer (MCT) labs for all exams](https://github.com/MicrosoftLearning/)



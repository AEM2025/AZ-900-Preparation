# AZ-900-Preparation
Resources to be prepared for Microsoft Azure Fundamentals Exam (AZ-900)


Exam includes three knowledge domain areas:

|AZ-900 Domain Area	| Weight |
--------------------------|-------|
|Describe cloud concepts  |	25-30%|
|Describe Azure architecture and services |	35-40%|
|Describe Azure management and governance	|30-35%|

## Resources
- [My Notes](https://github.com/AEM2025/AZ-900-Preparation#my-notes)
- [Youtube Videos](https://github.com/AEM2025/AZ-900-Preparation#youtube-videos)
- [Microsoft Learn path](https://github.com/AEM2025/AZ-900-Preparation#microsoft-learn)
- [Coursera Specialization](https://github.com/AEM2025/AZ-900-Preparation#coursera-specialization)
- [Practice Questions from Microsoft](https://learn.microsoft.com/en-us/certifications/exams/az-900/practice/assessment?assessment-type=practice&assessmentId=23)
- [Examtopics - Dumb1](https://www.examtopics.com/exams/microsoft/az-900/)

## My Notes:

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/Azure_Services%20.png" align="center" >

### 1 - Describe cloud concepts:<br><br>
#### 1.1 - Describe cloud computing:

<ul>
<li>Cloud models:
  <ol type="1">
    <li>Private cloud: on-premises data center.</li>
    <li>Public cloud: third party cloud provider who manage everything.</li>
    <li>Hybrid cloud: use both public and private.</li>
    <li>Multi-cloud: you're working with many cloud providers.</li>
    <li>Azure Arc: a set of technologies that helps manage your cloud environment (public, private, hybrid, multi cloud).</li>
    <li>Azure VMware Solution: lets you run your VMware workloads in Azure with seamless integration and scalability.</li>
  </ol>
</li>

<li>Consumption-based model has many benefits:
  <ol type="1">
    <li>No upfront costs.</li>
    <li>No need to purchase and manage costly infrastructure that users might not use to its fullest potential.</li>
    <li>The ability to pay for more resources when they're needed.</li>
    <li>The ability to stop paying for resources that are no longer needed.</li>
  </ol>
</li>
</ul>

#### 1.2 - Describe the benefits of using cloud services:
<ul>
  <li> High availability: 
    <ul> 
      <li>SLAs (service-level agreements): uptime guarantees.</li>
    </ul>
  </li>
  
  <li>Scalability:
    <ul>
      <li>Vertical scaling: add more CPU and memory. Scaling up and scaling down.</li>
      <li>Horizontal scaling: add more vms containers to custmize your solution. Scaling out and scaling in.</li>
    </ul>
  </li>

  <li>Reliability: The ability of a system to recover from failures and continue to function.</li>
  <li>Predictability: in the cloud lets you move forward with confidence.</li>
  <li>Performance predictability: focuses on predicting the resources needed to deliver a positive experience for your customers.</li>
  <li>Cost predictability: is focused on predicting or forecasting the cost of the cloud spend. </li>
  
  <li>Management in the cloud:
    <ol type="1">
      <li>Through a web portal.</li>
      <li>Using a command line interface.</li>
      <li>Using APIs.</li>
      <li>Using PowerShell.</li>
    </ol>
  </li>
</ul> 

#### 1.3 - Describe cloud service types:

<ul>
  <li>Infrastructure as a Service (IaaS): is most suited to a lift and shift migration from an on-premises datacenter to a cloud deployment.</li>
  <li>Software as a Service (SaaS): Finance and Expense tracking solution typically be in.</li>
</ul>

### 2 - Describe Azure architecture and services:<br><br>
#### 2.1 - Describe the core architectural components of Azure:
Components of Azure may be broken down into two main groupings: 
##### 1 - Physical infrastructure:

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/2.1%20-%20Region%20pairs.png" align="center" alt="Region pairs" width="700" height="400" >
<ul>
<li>Regions: is a geographical area on the planet that contains at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network. 
</li>

<li> Availability Zones:  are physically separate datacenters within an Azure region. Each availability zone is made up of one or more datacenters equipped with independent power, cooling, and networking.</li>

<li>Azure services that support availability zones fall into three categories:
  <ol type="1">
    <li>Zonal services: You pin the resource to a specific zone (for example, VMs, managed disks, IP addresses).</li>
    <li>Zone-redundant services: The platform replicates automatically across zones (for example, zone-redundant storage, SQL Database).</li>
    <li>Non-regional services: Services are always available from Azure geographies and are resilient to zone-wide outages as well as region-wide outages.</li>
  </ol>
</li>

<li> Region pairs: regions are paired with another region within the same geography (such as US, Europe, or Asia) at least 300 miles away. </li>

<li> Sovereign Regions: are instances of Azure that are isolated from the main instance of Azure. You may need to use a sovereign region for compliance or legal purposes. </li>

<li>Azure sovereign regions include:
  <ul>
    <li> US DoD Central, US Gov Virginia, US Gov Iowa and more: These regions are physical and logical network-isolated instances of Azure for U.S. government agencies         and partners. These datacenters are operated by screened U.S. personnel and include additional compliance certifications. </li>
    <li> China East, China North, and more: These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft doesn't directly           maintain the datacenters. </li>
  </ul>
</li>

</ul>


##### 2 - Management infrastructure

<ol type="1">

<li> Azure resources: Anything you create, provision, deploy, etc. is a resource. Virtual Machines (VMs), virtual networks, databases, cognitive services, etc. are all considered resources within Azure. 

Azure resource groups: Resource groups are simply groupings of resources. 

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/2.1%20-%20Resource%20Group%20.png" align="center" alt="Region pairs" width="700" height="400" >

</li>

<li> Azure subscriptions: A subscription provides you with authenticated and authorized access to Azure products and services. 
There are two types of subscription boundaries that you can use:
  <ul>
    <li> Billing boundary: This subscription type determines how an Azure account is billed for using Azure. You can create multiple subscriptions for different types          of billing requirements. Azure generates separate billing reports and invoices for each subscription so that you can organize and manage costs.
    </li>
    <li> Access control boundary: Azure applies access-management policies at the subscription level, and you can create separate subscriptions to reflect different organizational structures. 
    </li>
  </ul>
  
  <img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/2.2%20-%20Subscriptions%20.png" align="center" alt="Region pairs" width="700" height="400" >
  
</li>

<li> Azure management groups: Resources are gathered into resource groups, and resource groups are gathered into subscriptions. If you’re just starting in Azure that might seem like enough hierarchy to keep things organized. But imagine if you’re dealing with multiple applications, multiple development teams, in multiple geographies.

Azure management groups provide a level of scope above subscriptions. 

  <img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/2.3%20-%20Management-groups-subscriptions%20.png" align="center" alt="Region pairs" width="700" height="400" >

</li>
</ol>

#### 2.2 - Describe Azure compute and networking services:

<ul>
<li>
Azure VM: VMs provide infrastructure as a service (IaaS) in the form of a virtualized server and can be used in many ways.
</li>
  <li>VMs are an ideal choice when you need:
    <ul>
      <li> Total control over the operating system (OS).</li>
      <li> The ability to run custom software.</li>
      <li> To use custom hosting configurations.</li>
    </ul>
  </li>


<li>Virtual machine scale sets: let you create and manage a group of identical, load-balanced VMs. If you simply created multiple VMs with the same purpose, you’d need to ensure they were all configured identically and then set up network routing parameters to ensure efficiency. You’d also have to monitor the utilization to determine if you need to increase or decrease the number of VMs.</li>

<li>Scale sets allow you to centrally manage, configure, and update a large number of VMs in minutes.</li>



<li>Virtual machine availability sets: are another tool to help you build a more resilient, highly available environment. Availability sets are designed to ensure that VMs stagger updates and have varied power and network connectivity, preventing you from losing all your VMs with a single network or power failure.</li>


<li>Availability sets do this by grouping VMs in two ways: 
  <ol type="1">
    <li>Update domain: The update domain groups VMs that can be rebooted at the same time.</li>
    <li>Fault domain: The fault domain groups your VMs by common power source and network switch. By default, an availability set will split your VMs across up to three fault domains.</li>
  </ol>
</li>


<li>Some common examples or use cases for virtual machines include:
  <ul>
    <li> During testing and development.</li>
    <li> When running applications in the cloud. </li>
    <li> When extending your datacenter to the cloud.</li>
    <li> During disaster recovery.</li>
  </ul>
</li>

<li>VM Resources:
  <ul>
    <li> Size (purpose, number of processor cores, and amount of RAM)</li>
    <li> Storage disks (hard disk drives, solid state drives, etc.)</li>
    <li> Networking (virtual network, public IP address, and port configuration)</li>
  </ul>
</li>


<li>Azure Virtual Desktop: is a desktop and application virtualization service that runs on the cloud. It enables you to use a cloud-hosted version of Windows from any location. Azure Virtual Desktop works across devices and operating systems, and works with apps that you can use to access remote desktops or most modern browsers.</li>


<li>Azure Containers: Containers are a virtualization environment.</li>

<li>Azure Container Instances: offer the fastest and simplest way to run a container in Azure; without having to manage any virtual machines or adopt any additional services. Azure Container Instances are a platform as a service (PaaS).</li>

**Note: VM virtualize the hardware. containers virtualize the OS.**

<li>Azure Functions: is an event-driven, serverless compute option that doesn’t require maintaining virtual machines or containers. If you build an app using VMs or containers, those resources have to be "running" in order for your app to function. With Azure Functions, an event wakes the function, alleviating the need to keep resources provisioned when there are no events.</li>



<li>Azure App Service: enables you to build and host web apps, background jobs, mobile back-ends, and RESTful APIs in the programming language of your choice without managing infrastructure. It offers automatic scaling and high availability. App Service supports Windows and Linux. It enables automated deployments from GitHub, Azure DevOps, or any Git repo to support a continuous deployment model.</li>

<li>Azure App Service is a robust hosting option that you can use to host your apps in Azure. Azure App Service lets you focus on building and maintaining your app, and Azure focuses on keeping the environment up and running.</li>

<li>Azure App Service is an HTTP-based service for hosting web applications, REST APIs, and mobile back ends. It supports multiple languages, including .NET, .NET Core, Java, Ruby, Node.js, PHP, or Python. It also supports both Windows and Linux environments.</li>

<li>Types of app services:
  <ul>
    <li> Web apps
    <li> API apps
    <li> WebJobs
    <li> Mobile apps
  </ul>
</li>

<li>Azure Virtual Private Networks (VPN):  uses an encrypted tunnel within another network. VPNs are typically deployed to connect two or more trusted private networks to one another over an untrusted network (typically the public internet). Traffic is encrypted while traveling over the untrusted network to prevent eavesdropping or other attacks. VPNs can enable networks to safely and securely share sensitive information.</li>


<li>VPN gateway:  is a type of virtual network gateway. </li>

<li>It enables the following connectivity:
  <ul>
    <li> Connect on-premises datacenters to virtual networks through a site-to-site connection.</li>
    <li> Connect individual devices to virtual networks through a point-to-site connection.</li>
    <li> Connect virtual networks to other virtual networks through a network-to-network connection.</li>
  </ul>
</li>

<li>Azure ExpressRoute: lets you extend your on-premises networks into the Microsoft cloud over a private connection, with the help of a connectivity provider. This connection is called an ExpressRoute Circuit. With ExpressRoute, you can establish connections to Microsoft cloud services, such as Microsoft Azure and Microsoft 365. This allows you to connect offices, datacenters, or other facilities to the Microsoft cloud. Each location would have its own ExpressRoute circuit.</li>


<li>Azure DNS:  is a hosting service for DNS domains that provides name resolution by using Microsoft Azure infrastructure. By hosting your domains in Azure, you can manage your DNS records using the same credentials, APIs, tools, and billing as your other Azure services.</li>

</ul>

#### 2.3 - Describe Azure storage services:

list of redundancy options:

- Locally redundant storage (LRS): replicates your data three times within a single data center in the primary region. LRS provides at least 11 nines of durability (99.999999999%) of objects over a given year.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.1%20-%20locally-redundant-storage.png" align="center" width="500" height="300" >

- Zone-redundant storage (ZRS): replicates your Azure Storage data synchronously across three Azure availability zones in the primary region. ZRS offers durability for Azure Storage data objects of at least 12 nines (99.9999999999%) over a given year.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.1%20-%20zone-redundant-storage.png" align="center" width="500" height="300" >

- Geo-redundant storage (GRS): offers durability for Azure Storage data objects of at least 16 nines (99.99999999999999%) over a given year. geo-redundant storage (GRS) and geo-zone-redundant storage (GZRS). GRS is similar to running LRS in two regions, and GZRS is similar to running ZRS in the primary region and LRS in the secondary region.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.1%20-%20geo-redundant-storage.png" align="center" width="500" height="300" >

- Geo-zone-redundant storage (GZRS)
<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.1%20-%20geo-zone-redundant-storage-138ab5af.png" align="center" width="500" height="300" >

- Read-access geo-redundant storage (RA-GRS)
- Read-access geo-zone-redundant storage (RA-GZRS)

| Type | Supported services| 	Redundancy Options	| Usage|
|------|-------------------|-----------------------|------|
| Standard general-purpose v2 |	Blob Storage (including Data Lake Storage), Queue Storage, Table Storage, and Azure Files |	LRS, GRS, RA-GRS, ZRS, GZRS, RA-GZRS |	Standard storage account type for blobs, file shares, queues, and tables. Recommended for most scenarios using Azure Storage. If you want support for network file system (NFS) in Azure Files, use the premium file shares account type.|
| Premium block blobs	| Blob Storage (including Data Lake Storage) |	LRS, ZRS |	Premium storage account type for block blobs and append blobs. Recommended for scenarios with high transaction rates or that use smaller objects or require consistently low storage latency. |
| Premium file shares |	Azure Files	| LRS, ZRS | Premium storage account type for file shares only. Recommended for enterprise or high-performance scale applications. Use this account type if you want a storage account that supports both Server Message Block (SMB) and NFS file shares. |
| Premium page blobs |	Page blobs only |	LRS |	Premium storage account type for page blobs only. |

Azure storage services:
- Azure Blobs: A massively scalable object store for text and binary data. Also includes support for big data analytics through Data Lake Storage Gen2.
- Blob storage is ideal for:
  - Serving images or documents directly to a browser.
  - Storing files for distributed access.
  - Streaming video and audio.
  - Storing data for backup and restore, disaster recovery, and archiving.
  - Storing data for analysis by an on-premises or Azure-hosted service.

- Blob storage tiers:
  - Hot access tier: Optimized for storing data that is accessed frequently (for example, images for your website).
  - Cool access tier: Optimized for data that is infrequently accessed and stored for at least 30 days (for example, invoices for your customers).
  - Archive access tier: Appropriate for data that is rarely accessed and stored for at least 180 days, with flexible latency requirements (for example, long-term backups).


- Azure Files: Managed file shares for cloud or on-premises deployments. offers fully managed file shares in the cloud that are accessible via the industry standard Server Message Block (SMB) or Network File System (NFS) protocols.
- Azure Queues: A messaging store for reliable messaging between application components.
- Azure Disks: Block-level storage volumes for Azure VMs.

- Azure Migrate: is a service that helps you migrate from an on-premises environment to the cloud. Azure Migrate functions as a hub to help you manage the assessment and migration of your on-premises datacenter to Azure.

- Azure Migrate hub also includes the following tools to help with migration:
  - Azure Migrate: Discovery and assessment. Discover and assess on-premises servers running on VMware, Hyper-V, and physical servers in preparation for migration to Azure.
  - Azure Migrate: Server Migration. Migrate VMware VMs, Hyper-V VMs, physical servers, other virtualized servers, and public cloud VMs to Azure.
  - Data Migration Assistant. Data Migration Assistant is a stand-alone tool to assess SQL Servers. It helps pinpoint potential problems blocking migration. It identifies unsupported features, new features that can benefit you after migration, and the right path for database migration.
  - Azure Database Migration Service. Migrate on-premises databases to Azure VMs running SQL Server, Azure SQL Database, or SQL Managed Instances.
  - Web app migration assistant. Azure App Service Migration Assistant is a standalone tool to assess on-premises websites for migration to Azure App Service. Use Migration Assistant to migrate .NET and PHP web apps to Azure.
  - Azure Data Box. Use Azure Data Box products to move large amounts of offline data to Azure.

- Azure file movement options:
  - AzCopy is a command-line utility that you can use to copy blobs or files to or from your storage account. With AzCopy, you can upload files, download files, copy files between storage accounts, and even synchronize files. AzCopy can even be configured to work with other cloud providers to help move files back and forth between clouds.
  - Azure Storage Explorer is a standalone app that provides a graphical interface to manage files and blobs in your Azure Storage Account. It works on Windows, macOS, and Linux operating systems and uses AzCopy on the backend to perform all of the file and blob management tasks. With Storage Explorer, you can upload to Azure, download from Azure, or move between storage accounts.
  - Azure File Sync: is a tool that lets you centralize your file shares in Azure Files and keep the flexibility, performance, and compatibility of a Windows file server. 

#### 2.4 - Describe Azure identity, access, and security:

- Azure Active Directory (Azure AD) is a directory service that enables you to sign in and access both Microsoft cloud applications and cloud applications that you develop. Azure AD can also help you maintain your on-premises Active Directory deployment.

- Azure AD provides services such as:
  - Authentication: This includes verifying identity to access applications and resources.
  - Single sign-on: Single sign-on (SSO) enables you to remember only one username and one password to access multiple applications.
  - Application management: You can manage your cloud and on-premises apps by using Azure AD.
  - Device management: Along with accounts for individual people, Azure AD supports the registration of devices.

- Azure AD Connect: enables you to connect your on premises AD to Azure AD.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.2%20-%20azure-active-directory-sync-topology%20.png" align="center" width="700" height="300" >

- Azure Active Directory Domain Services (Azure AD DS) is a service that provides managed domain services such as domain join, group policy, lightweight directory access protocol (LDAP), and Kerberos/NTLM authentication.

- Multifactor authentication: is the process of prompting a user for an extra form (or factor) of identification during the sign-in process.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.2%20-%20passwordless-convenience-security.png" align="center" width="500" height="300" >

- Conditional Access: is a tool that Azure Active Directory uses to allow (or deny) access to resources based on identity signals. These signals include who the user is, where the user is, and what device the user is requesting access from.

- Conditional Access helps IT administrators:
  - Empower users to be productive wherever and whenever.
  - Protect the organization's assets.

During sign-in, Conditional Access collects signals from the user, makes decisions based on those signals, and then enforces that decision by allowing or denying the access request or challenging for a multifactor authentication response.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.2%20-%20conditional-access%20.png" align="center" width="700" height="300" >

- Azure role-based access control: is applied to a scope, which is a resource or set of resources that this access applies to. So, if you hire a new engineer and add them to the Azure RBAC group for engineers, they automatically get the same access as the other engineers in the same Azure RBAC group.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.2%20-%20role-based-access-scope%20.png" align="center" width="500" height="300" >

- Scopes include:
  - A management group (a collection of multiple subscriptions).
  - A single subscription.
  - A resource group.
  - A single resource.

- Resource Manager: is a management service that provides a way to organize and secure your cloud resources. You typically access Resource Manager from the Azure portal, Azure Cloud Shell, Azure PowerShell, and the Azure CLI.

- Zero Trust: is a security model that assumes the worst case scenario and protects resources with that expectation. Zero Trust assumes breach at the outset, and then verifies each request as though it originated from an uncontrolled network.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.2%20-%20zero-trust%20.png" align="center" width="500" height="300" >

- The objective of defense-in-depth is to protect information and prevent it from being stolen by those who aren't authorized to access it.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/3.2%20-%20defense-depth%20.png" align="center" width="500" height="300" >

- Here's a brief overview of the role of each layer:
  - The physical security layer is the first line of defense to protect computing hardware in the datacenter.
  - The identity and access layer controls access to infrastructure and change control.
  - The perimeter layer uses distributed denial of service (DDoS) protection to filter large-scale attacks before they can cause a denial of service for users.
  - The network layer limits communication between resources through segmentation and access controls.
  - The compute layer secures access to virtual machines.
  - The application layer helps ensure that applications are secure and free of security vulnerabilities.
  - The data layer controls access to business and customer data that you need to protect.


### 3 - Describe Azure management and governance:<br><br>
#### 3.1 - Describe cost management in Azure:

The pricing calculator and the total cost of ownership (TCO) calculator are two calculators that help you understand potential Azure expenses. Both calculators are accessible from the internet, and both calculators allow you to build out a configuration. However, the two calculators have very different purposes.

- The pricing calculator: is designed to give you an estimated cost for provisioning resources in Azure. 

- The TCO calculator: is designed to help you compare the costs for running an on-premises infrastructure compared to an Azure Cloud infrastructure. 

Cost Management provides the ability to quickly check Azure resource costs, create alerts based on resource spend, and create budgets that can be used to automate management of resources.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/6.1%20-%20cost-analysis%20.png" align="center" >

-Cost alerts provide a single location to quickly check on all of the different alert types that may show up in the Cost Management service. The three types of alerts that may show up are:
  - Budget alerts: notify you when spending, based on usage or cost, reaches or exceeds the amount defined in the alert condition of the budget. Cost Management budgets are created using the Azure portal or the Azure Consumption API.
  - Credit alerts: notify you when your Azure credit monetary commitments are consumed. Monetary commitments are for organizations with Enterprise Agreements (EAs). 
  - Department spending quota alerts: notify you when department spending reaches a fixed threshold of the quota.

#### 3.2 - Describe features and tools in Azure for governance and compliance:

- Azure Blueprints lets you standardize cloud subscription or environment deployments. Instead of having to configure features like Azure Policy for each new subscription, with Azure Blueprints you can define repeatable settings and policies that are applied as new subscriptions are created. Need a new test/dev environment? Azure Blueprints lets you deploy a new Test/Dev environment with security and compliance settings already configured.

- Azure Policy is a service in Azure that enables you to create, assign, and manage policies that control or audit your resources. These policies enforce different rules across your resource configurations so that those configurations stay compliant with corporate standards.

- An Azure Policy initiative is a way of grouping related policies together. The initiative definition contains all of the policy definitions to help track your compliance state for a larger goal.

- A resource lock prevents resources from being accidentally deleted or changed.
- Microsoft Service Trust Portal: is a portal that provides access to various content, tools, and other resources about Microsoft security, privacy, and compliance practices.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/6.1%20-%20service-trust-portal%20.png" align="center"  >

#### 3.3 - Describe features and tools for managing and deploying Azure resources:

- Azure provides multiple tools for managing your environment, including the:
  - Azure portal: is a web-based, unified console that provides an alternative to command-line tools. With the Azure portal, you can manage your Azure subscription by using a graphical user interface. You can:
    - Build, manage, and monitor everything from simple web apps to complex cloud deployments
    - Create custom dashboards for an organized view of resources
    - Configure accessibility options for an optimal experience
  - Azure cloud shell: is a browser-based shell tool that allows you to create, configure, and manage Azure resources using a shell. Azure Cloud Shell support both Azure PowerShell and the Azure Command Line Interface (CLI), which is a Bash shell.

  - Azure PowerShell: is a shell with which developers, DevOps, and IT professionals can run commands called command-lets (cmdlets). These commands call the Azure REST API to perform management tasks in Azure. 
In addition to be available via Azure Cloud Shell, you can install and configure Azure PowerShell on Windows, Linux, and Mac platforms.

  - Azure Command Line Interface (CLI):  is functionally equivalent to Azure PowerShell, with the primary difference being the syntax of commands. While Azure PowerShell uses PowerShell commands, the Azure CLI uses Bash commands.

- Azure arc: lets you extend your Azure compliance and monitoring to your hybrid and multi-cloud configurations. Azure Arc simplifies governance and management by delivering a consistent multi-cloud and on-premises management platform.

- Azure Arc provides a centralized, unified way to:
  - Manage your entire environment together by projecting your existing non-Azure resources into ARM.
  - Manage multi-cloud and hybrid virtual machines, Kubernetes clusters, and databases as if they are running in Azure.
  - Use familiar Azure services and management capabilities, regardless of where they live.
  - Continue using traditional ITOps while introducing DevOps practices to support new cloud and native patterns in your environment.
  - Configure custom locations as an abstraction layer on top of Azure Arc-enabled Kubernetes clusters and cluster extensions.

- Currently, Azure Arc allows you to manage the following resource types hosted outside of Azure:
  - Servers
  - Kubernetes clusters
  - Azure data services
  - SQL Server
  - Virtual machines (preview)

- Azure Resource Manager (ARM): is the deployment and management service for Azure. It provides a management layer that enables you to create, update, and delete resources in your Azure account. Anytime you do anything with your Azure resources, ARM is involved. It's equivelent to Cloudformation in AWS.

- With Azure Resource Manager, you can:
  - Manage your infrastructure through declarative templates rather than scripts. A Resource Manager template is a JSON file that defines what you want to deploy to Azure.
  - Deploy, manage, and monitor all the resources for your solution as a group, rather than handling these resources individually.
  - Re-deploy your solution throughout the development life-cycle and have confidence your resources are deployed in a consistent state.
  - Define the dependencies between resources, so they're deployed in the correct order.
  - Apply access control to all services because RBAC is natively integrated into the management platform.
  - Apply tags to resources to logically organize all the resources in your subscription.
  - Clarify your organization's billing by viewing costs for a group of resources that share the same tag.

#### 3.4 - Describe monitoring tools in Azure:

- Azure Advisor: evaluates your Azure resources and makes recommendations to help improve reliability, security, and performance, achieve operational excellence, and reduce costs. Azure Advisor is designed to help you save time on cloud optimization. The recommendation service includes suggested actions you can take right away, postpone, or dismiss.

- The recommendations are divided into five categories:
  - Reliability is used to ensure and improve the continuity of your business-critical applications.
  - Security is used to detect threats and vulnerabilities that might lead to security breaches.
  - Performance is used to improve the speed of your applications.
  - Operational Excellence is used to help you achieve process and workflow efficiency, resource manageability, and deployment best practices.
  - Cost is used to optimize and reduce your overall Azure spending.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/6.1%20-%20azure-advisor-dashboard.png" align="center" >

- Azure Service Health: helps you keep track of Azure resource, both your specifically deployed resources and the overall status of Azure. Azure service health does this by combining three different Azure services:
  - Azure Status is a broad picture of the status of Azure globally. Azure status informs you of service outages in Azure on the Azure Status page. 
  - Service Health provides a narrower view of Azure services and regions. It focuses on the Azure services and regions you're using. 
  - Resource Health is a tailored view of your actual Azure resources. It provides information about the health of your individual cloud resources, such as a specific virtual machine instance. Using Azure Monitor, you can also configure alerts to notify you of availability changes to your cloud resources.

- Azure Monitor:  is a platform for collecting data on your resources, analyzing that data, visualizing the information, and even acting on the results. Azure Monitor can monitor Azure resources, your on-premises resources, and even multi-cloud resources like virtual machines hosted with a different cloud provider.

<img src="https://github.com/AEM2025/AZ-900-Preparation/blob/master/6.1-azure-monitor-overview-.jpg" align="center" >

- Azure Log Analytics: is the tool in the Azure portal where you’ll write and run log queries on the data gathered by Azure Monitor. Log Analytics is a robust tool that supports both simple, complex queries, and data analysis. 


- Azure Monitor Alerts are an automated way to stay informed when Azure Monitor detects a threshold being crossed. You set the alert conditions, the notification actions, and then Azure Monitor Alerts notifies when an alert is triggered.

- Application Insights, Azure monitor feature, is capable of monitoring applications that are running in Azure, on-premises, or in a different cloud environment.
- There are two ways to configure Application Insights: 
  - Install SDK on your application.
  - Use the Application Insights agent. The Application Insights agent is supported in C#.NET, VB.NET, Java, JavaScript, Node.js, and Python.
  
- Once Application Insights is up and running, you can use it to monitor a broad array of information, such as:
  - Request rates, response times, and failure rates
  - Dependency rates, response times, and failure rates, to show whether external services are slowing down performance
  - Page views and load performance reported by users' browsers
  - AJAX calls from web pages, including rates, response times, and failure rates
  - User and session counts
  - Performance counters from Windows or Linux server machines, such as CPU, memory, and network usage












## Youtube videos:
- [Microsoft Azure Fundamentals Certification Course (AZ-900) - Pass the exam in 3 hours! FreeCodeCamp](https://www.youtube.com/watch?v=NKEFWyqJ5XA&pp=ygUGYXotOTAw)
- [English - Microsoft Azure Fundamentals | AZ-900 By Adam Marczak](https://www.youtube.com/playlist?list=PLGjZwEtPN7j-Q59JYso3L4_yoCjj2syrM)
- [Arabic - Microsoft Azure Fundamentals | AZ-900 By Hmada Glal](https://www.youtube.com/playlist?list=PLCIJjtzQPZJ-CDaKOAlm3JfpL2kddIhRA)
- [Arabic - Microsoft Azure Fundamentals | AZ-900 By Mohamed Zohdy](https://www.youtube.com/playlist?list=PLDxVq3TlR9y3D61tEq4BbRZ8f5bv2_PFt)
- [Arabic - Microsoft Azure Fundamentals | AZ-900 By Sajjad Ghaffoori](https://www.youtube.com/playlist?list=PLAqaqJU4wzYV00PpXhPpaKEBNgsl7TZdK)

## Microsoft learn:
- [Master the basics of Azure: Fundamentals](https://learn.microsoft.com/en-us/users/sandramarin/collections/n6ga8m0jkgrwk)

## Coursera Specialization:
- [Microsoft Azure Fundamentals AZ-900 Exam Prep Specialization](https://www.coursera.org/specializations/microsoft-azure-fundamentals-az-900)

# AZ-900-Preparation
Resources to be prepared for Microsoft Azure Fundamentals Exam (AZ-900)


Exam includes three knowledge domain areas:

|AZ-900 Domain Area	| Weight |
--------------------------|-------|
|Describe cloud concepts  |	25-30%|
|Describe Azure architecture and services |	35-40%|
|Describe Azure management and governance	|30-35%|

## My Notes:
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
#### 2.4 - Describe Azure identity, access, and security:


### 3 - Describe Azure management and governance:<br><br>
#### 3.1 - Describe cost management in Azure:
#### 3.2 - Describe features and tools in Azure for governance and compliance:
#### 3.3 - Describe features and tools for managing and deploying Azure resources:
#### 3.4 - Describe monitoring tools in Azure:

## Youtube videos:
- [Microsoft Azure Fundamentals Certification Course (AZ-900) - Pass the exam in 3 hours! FreeCodeCamp](https://www.youtube.com/watch?v=NKEFWyqJ5XA&pp=ygUGYXotOTAw)
- [Arabic - Microsoft Azure Fundamentals | EXAM AZ-900 By Hmada Glal](https://www.youtube.com/playlist?list=PLCIJjtzQPZJ-CDaKOAlm3JfpL2kddIhRA)
- [Arabic - Microsoft Azure Fundamentals | AZ-900 By Mohamed Zohdy](https://www.youtube.com/playlist?list=PLDxVq3TlR9y3D61tEq4BbRZ8f5bv2_PFt)
- [Arabic - Microsoft Azure Fundamentals | AZ-900 By Sajjad Ghaffoori](https://www.youtube.com/playlist?list=PLAqaqJU4wzYV00PpXhPpaKEBNgsl7TZdK)

## Microsoft learn:
- [Master the basics of Azure: Fundamentals](https://learn.microsoft.com/en-us/users/sandramarin/collections/n6ga8m0jkgrwk)

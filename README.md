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

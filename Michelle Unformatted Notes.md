Cloud Computing
Cloud computing requires virtualization and all these characteristics must be met
Resource Pooling
Broad access
Metered usage
rapid elasticity
self-provisioning

Resource pooling
cloud service provider (CSP) equipment available for cloud tenants
compute, network and storage appears infinite for cloud tenant

Broad access
the use of any type of device (phone, tablet, laptop)

Metered usage
Resource usage is tracked
monthly charges based on usage

Rapid elasticity
More VM's (horizontal scaling)
More storage or Increased vm power (vertical scaling)

Self-provisioning
cloud user deploys & manages resources
CSP techs are not involved
GUI (azure portal), command line (powershell or azure CLI), template (text file with instructions in to deploy or manage 1 or more cloud resources)

Virtualization & the cloud
does not mean cloud
cloud computing requires virtualization

hypervisor is a software solution
Type 1 - Is the OS
runs on physical hardware so called "bare metal" hardware
streamlined to support virtualization hosting
VMware ESXI, Microsoft HyperV
Type 2 - Not OS
Is an app that runs in existing OS (Windows, Linux)
stability and performance of OS affects vm guests
Not designed to run mission-critical virtual workloads
ex- VMware workstation

Dedicates VM hosting
renting use of a physical server running Hyper visor in a datacenter
physical host in datacenter used by single cloud tenant

VM sprawl
quick & easy provisioning of vm
easy to forget abt unused vm's

Azure advisor provides recommendations abt resources that haven't been used or unused vms that are forgotten abt

Cloud computing economies of scale
Resource pooling for use by cloud tenants
csp pool resources (network infrastructure equipment, storage arrays, servers to run Vm's) for use by cloud tenants
cloud tenants pay for their usuage of these resources

Capex for CSP 
Opex for cloud tenant
cloud tenants can use azure pricing calculator to control how much they're paying and what they're paying for

CSP can negotiate better pricing for equipment bulk purchases 
Sale of excess unused capacity (Spot VMs)
Spot VMs used at a discount 

Homogenous data center configurations within and among data centers
Same type of equipment - same type of configuration for that equipment is attempted to be adhered to to streamline the process of making those resources available pooled together for use by cloud customers
Sometimes automated configuration is acquired to configure new hardware. Like hypervisors to a cluster that can run VM guests at datacenter

Network links linking datacenters together for azure cloud
from multiple network providers around the world for redundancy
negotiation with network providers 
long-term commitment for network providers

public clouds
resource pooling
provide broad access
metered usage
rapid elasticity
self-provisioning

available to anyone over internet
usually a free trial

network link speed
physical data center security
CSP security accreditations

reports published from 3rd party audits of physical datacenters and security mechanisms

GDPR general data protection regulation - regional regulations which exists to safeguard the privacy of European native citizen data
all of this is published on azure website

shared responsibility (depends on cloud service)
public clouds are larger target for malicious users

IT service availabity per region
VM instance types
graphic acceleration
dedicated hosts

public cloud require cloud technician skill set - Microsoft azure certified
Vendor lock-in - make sure not selecting a public cloud provider that uses a proprietary formats for file storage. 

Private clouds - owned and used by a single organization
resource pooling owned and acquired by a single organization
broad access is limited - network controlled by local organization
metered usage is tracked
rapid elasticity 
self-provisioning 

on premises virtualization does not constitute a private cloud
virtualization is required 

organization has full configuration control
metered usage for departmental or project chargeback

LAN/WAN bandwidth & isolation (Local area network) (Wide area network)
On-premises security 
responsible for compliance with security and data privacy falls on organization as well as underlying cloud infrastructure
Less of a target than public cloud - not advertised but might not have resources to dedicate securing infrastructure 

Azure stack lets you run azure services without a connection to public cloud
private cloud management can be outsourced

Hybrid cloud
Resource pooling would be applicable for private and public
broad access 
metered usage
rapid elasticity - when private cloud resources have been depleted, you can reach out to public cloud to use resources for additional storage capacity or cloud bursting
self-provisioning

combines private & public clouds
full configuration control (private)
uses virtualization - can't have a cloud without virtualization
Confidential processes and data might have to remain under singular organization control

used for short-term (migration)
or long-term - cloud bursting resources are depleted

IT service/risk outsourced to public cloud provider
combining capex & opex 

Azure stack - run azure services & store data locally via vendor-specific hardware appliances
means that an organization can use familiar azure services without a connection to internet 
services include - azure vms
azure app service
azure active directory - is an identity in access management solution where you can create users and groups and control permissions to azure resources 
azure functions - allow developers to build custom functions using cloud based tools - considered serverless feature because developers don't need to manually deploy a vm to run and host this function. handled automatically

Community cloud designed to serve a special community of clients
Resource pooling
broad access - limited for specific access by organizations that have similar computing needs
metered usage still tracked and customers still pay on usage
rapid elasticity
self-provisioning

Serves specific needs to organizations or govts that have specific requirements - usually security but not just security

Government
Pharmaceutical - could apply to a specific software that can monitors pharmaceutical distribution or compliance with laws and regulations as well as expiry of certain types of pharmaceuticals
financial services

Community clouds and regulatory compliance
Health insurance portability & accountability act (HIPAA) - protect of patient medical insurance and medical information 
General data protection regulation (GDPR) - safeguard sensitive data of European union citizens even if the data is being handled outside of EU.

International based security standards
Payment card industry data security standard (PCI DSS) - security controls to safeguard cc holder information 


Community cloud solutions
Azure US Government cloud - consists of 8 azure regions
US DoD, US Gov, US Secret

These communities do not show up in public cloud regions

Azure Germany - two azure Germany regions (2 public azure regions in Germany also)

Azure China - 4 azure regions in china
Chinese data sovereignty requirements 
data stays in china
cloud workloads stay in china
this region is unavailable when deploying resources using other azure clouds

IaaS - Infrastructure as a Service
cloud service model that supports IT services

All underlying infrastructure hosted in datacenter
Configured by IT sys admins
Deploying and managing:
Network
Network security
Storage 
compute
Service level agreement (SLA)

Azure data center house all the physical equipment that provides infrastures on which azure services run
locations not disclosed for security reasons
one or more data center per availability zone (AZ) - provides redundancy at power level, network level and equipment rack level as well
physical facility security

Shared responsibility - that it's secure, redundant and kept up and running
customer's responsibility to customize and manage vm 
CSP - hypervisor, network equipment & physical storage arrays
Tenant - VM Deployment & management, VNets (Virtual networks), storage provisioning

Azure IaaS examples
Storage accounts
Virtual Network Configurations where we specity IP address range used by subnets to find vnets
subnets are where you actually deploy resources like vms
Manually deployed vms are IaaS not to be confused with vms that are automatic provisioned with other services like azure functions. 
Azure firewall is another example 

IaaS benefits
Accessible from anywhere
Less provisioning time
Shared responsibility

Azure IaaS can be managed with
GUI management (Azure Portal) - web interface
Azure CLI 
Azure PowerShell - issue command 
Programmatic API calls - to control various azure services
Templates

Azure PaaS - Platform as a Service
Underlying infrastructure required to support IT services
Provisioning done by CSP
Referred to as a "Managed Service"
Configured by IT admins or software developers
Service level agreement

CSP responsible for underlying infrastructure, VMs, software and patching
Tenant is responsible for configuration of the solution and data

Azure active directory - (Azure AD) - create user accounts or groups to control user access
No network configuration to deploy or manage
No servers to deploy or manage
No OUs (organizational units) 
Full active directory control - deploy manually as IaaS

Azure SQL Database - managed service
No network configuration to deploy or manage
No servers to deploy or manage
No database software to install
Full SQL database control - deploy manually as IaaS

Windows Virtual desktop
No network configuration to deploy or manage
No client-based vms to deploy or manage
Select a bundle (hardware & software)

Azure PaaS can manage solutions using:
GUI management (Azure portal)
Azure CLI
Azure PowerShell
Programmatic API calls
Templates

Azure SaaS (Software as a service)
End-user applications
Limited configuration options
Isolated from other cloud tenants
"Managed Service"
Software managed by CSP
Service level agreement for each SaaS offering

Azure SaaS
Shared responsibility
CSP: supporting infrastructure, software maintenance/patching, tenant isolation
Tenant: available configuration options, usage, data privacy

SaaS app that has a reliance upon user and group provisioning
User and group permissions instead of individual permissions
Enable Multifactor authentication - function of PaaS 
Single Sign on


Accessible from anywhere using any platform
Normally no software deployment (apps on devices vs. browser-based)
User familiarity with cloud-based applications like outlook web mail

SaaS benefits
Pay only what you use
App accessibility through web browser

SaaS Examples
Microsoft 365
Customized line-of-business apps
Web application

On premises vs. public cloud
public cloud: CSP has many data center around the globe and their responsibility they're all secured and all hardware configured accourdingly 
Private cloud: owned and used by a single organization
on premises gives configuration flexibility which
ensuring data privacy
& regulatory compliance

On premises vs. public cloud hardware
acquisition & shipping
configuration changes 
ongoing management
firmware updates
Decommissioning - data destruction

Software
acquisition & licensing
Configuration
Ongoing management 
software updates or patches
Decommissioning

Cost (capex vs opex)
total cost of ownership (TCO)
Microsoft offers web based TCO

CSP economies of scale

Migrating to the cloud
might include on-premises 
IT systems
data

On-premises migration suitability
Cloud service mapping
security standards

when thinking about migrating to cloud from on-premises
Lift and shift migration
migrating with little to no change

Azure migrate service
Discovery & migration assessment of on-premises IT workloads
Detects on-premises IT system dependencies
Can provide cost estimates 

Azure Migrate Service Discovery
Can discover VM
Virtual desktop Infrastructure (VDI)
Databases
Web applications
Data (Azure Data Box)

Azure Migration Steps
1. Create a project through azure portal
2. On-premises collector VM
3. Gathered data is sent to Azure project
4. Organize discovered VMs into groups
5. View or download assessment

Microsoft Cloud Adoption Framework for Azure??????
Naming convention templates and best practices facilitate migrating to azure
Spot instances are when an extra Microsoft data center compute capacity can be used at a discount for VMs.

Resource pooling
CSP equipment available in data centers for cloud tenant 

Broad access
Wide array of different types of devices - phones, laptops, tablets etc

Rapid elasticity
Add or remove IT services that are running in the cloud
Add or remove VMs
Resize VMs, autoscaling using vertical or horizontal scaling

On-demand self service
Cloud user deploys and manages resources
CSP technicians not involved
Provides more cloud resource control for cloud tenants immediately

Metered Usage
Resource usage is tracked

Virtualization does not mean cloud but cloud computing DOES mean virtualization

Virtualization & the cloud
means OS virtualization requires a hypervisor
Type 1 hypervisor
Type 2  hypervisor
Application virtualization (app streaming)
Application containers - does not have OS - runs on a host that has an installed engine that runs containers. Uses OS running on underlying host
Virtual desktop infrastructure (VDI); Azure virtual desktop
Software-defined networking (SDN)

Type 1 hypervisor - bare metal 
IS the OS
Runs directly on hardware
Streamlined to support virtualization hosting simultaneously like CPU cores, RAM, storage 

VMware ESXI is an ex of type 1 hypervisor

Type 2 Hypervisor
Runs as an app within an existing OS (Windows, Linux)
Stability & Performance of the OS affect vm guests

Dedicated VM hosting - means that a single cloud tenant
physical host in a data center
used by a single cloud tenant
more expensive than shared hosting for vm
legal/regulatory compliance

VM Sprawl
VMs that are not being used but you are still paying for the storage and disks being used or the IP 

Azure Data Centers
Public Cloud - CSP data centers
Private cloud - owned & used by a single organization - some organizations use a 3rd party
Configuration flexibility
Data privacy
Regulatory compliance

On-premises IT hardware Responsibilities:
Acquisition & Shipping of hardware
Configuration
Ongoing management of equipment
Firmware updates
Decommissioning

On-premises IT Software Responsibilities:
Acquisition, licensing
Configuration
Ongoing Management
Decommissioning

On-premises vs Public Cloud
CapEx vs OpEx
Total cost of ownership (TCO) tool 

CSP economies of scale 
CSP security accreditations

The cloud can serve as an alternate site if there's a natural disaster
IT system duplication in the cloud for resiliency
Data replication to the cloud for resiliency

Azure regions
Geographical regions
More than 60 worldwide
Service availability can vary by region

Some configurations require resources to be in the same region
A key vault should be in the same region as storage count using customer managed keys

Azure Availability zones (AZs)
Contained within an azure region - each one has a power, network and cooling configuration
Each region has at least one az
An availability zone is a separate location (data center)
they'll all be linked with high-speed networks

Azure Sovereign Regions
A type of community cloud
Are kept separate or isolated from standard public azure cloud
dedicated to specific entities: azure german cloud, azure government, azure china

Azure Arc - manage IT resources across platforms, clouds, and data centers as if they were running in Azure using Azure management tools
Azure Arc centralized management & governance of on-premises IT services
VMs running in AWS (Amazon web services)
Manage IOT (Internet of things) or edge IT services

It allows for unified management using tools like 
Azure portal
Azure CLI
Azure powershell - it's object oriented
Azure REST API 

Azure Arc - External Services Management
Physical/Virtual servers for Linux & Windows
Kubernetes clusters - is an orchestration in management platform that allows you to manage application containers in a large scale
Manage Microsoft SQL server

Azure Arc-enabled server
azure connected machine agent must be installed
The server is assigned a resource ID, becomes a part of the resource group, and is assigned a managed identity
Server is then treated as a standard Azure resource and can have tags applied, Azure policy allows to check for compliance on the configuration of those servers
Servers can be monitored using a log analytics workspace

Azure Cloud technicians will be interested in Azure Arc when:
they need a centralized compliance (Azure policy)
or centralized server configuration management

Azure Data Centers is a physical facility that house computer equipment
exist in 140 countries

Azure Data center components
HVAC
Equipment Racks
Hypervisor Servers
Storage Arrays
Routers, switches, UPSs, generators

Azure Data Center Security
Fencing, alarms, guards
Mantrap doors, logged entry and exit
Employee background checks
Locked rooms
Locked equipment racks

Azure Regions
Geographical in nature
54 regions in 140 countries
Undisclosed Azure government regions

Availability Zones
Within an Azure region - normally at least 3
One or more data centers

Azure Service Availability
Varies by region
Examples are:
Azure Search - will not be able to use Canada East
G-Series (high end) VMs - not available in Central US

When we go to manage and deploy resources it varies from one region to another

An availability zone (AZ) can have one or more data centers
Useful to spread out services to increase availability
Replicate data between AZs in case of a catastrophe or failure in one AZ

High availability
Fault domains - to spread out our deployed services like VMs if we’ve got a cluster of them across multiple physical data center racks. Where each rack has its own power source, network  switch, own hypervisor etc. In case of a failure in one data center rack, there will still be some VMs that will be in another fault domain. 
Update domains  

Azure Resource Manager (ARM)
Manages related resources as a group - but it doesn’t have to do that. 
Can use arm to deploy or manage a single VM
Use ARM to deploy resources - create new VMs, storage accounts
Use ARM to manage existing resources or remove resources too

Azure Resources are 
Web applications
Databases
Storage Accounts
Virtual Machines

When you deploy a VM one of the things you need to do is deploy into a resource group or create a new resource group

ARM Template looks like java script but it’s json syntax
A template is a file that uses json syntax
You can see VM Name, location, size of RAM etc

You can deploy ARM Templates several ways
You can create a template in Azure portal in editor or import a template

You can also deploy ARM templates through PowerShell

Azure Resource Manager (ARM)

Azure VMs
Can deploy Window images or Linux images

When you deploy a vm , you need to know resource group it’s deployed into. Specify the region it’s going into and VM name. The Image size, (vCPUs, RAM and number of data disks) which can all be monitored and changed over time. Also specify OS credentials (ex. Username and password)

VM can deploy VM extensions - small software agents that can be deployed in a vm that give the VM enhanced capabilities. Like enhanced monitoring capabilities or malware scanner. 
Have to deploy the VM into a subnet in a VNet. and you can determine if you want it to have a public IP address

Public IP address is a separate resource that will be associated with VM. 

You can also get to Azure cloud though a VPN or expressroute if you need to manage VMs directly. You’ll need the private IP. 

You’ll also need to specify the Network security group which is a resource that serves basic packet of filtering firewall that controls into or out of VM network interface card or an entire subnet. 
Can also configure load balancing. 
You can also enable auto-shutdown and backup. 

You’ll need to specify logon credentials
Connect using remote desktop protocol (RDP) to remotely manage your VM
In order to do that you need to make sure firewalls allow RDP - firewalls in Azure cloud and also any firewall software in the OS. 
You can also remotely manage through Azure Bastion service

If you don’t want to use a public IP, you don’t want to VPN and don’t want to use expressroute circuits, you can use Azure Bastion.

FOR LINUX VMs
You can specify username/password credentials
Public key authentication
Connect using secure shell (SSH) - specify username but no password. You’ll need the private key which is password protected. 
Ensure firewalls allows SSH traffic or
Remote manage through Azure Bastion

You can manage Azure VMs with 
Azure portal
Azure CLI
PowerShell
Application programming interfaces (APIs) or ARM templates

You can also configure VM scale set (VMSS) - is used with load balancing
The scale set is autoscaled
Scale out - adding VMs
Scale in - removing VMs

VMs in a scale set need to be identical. 
Same OS image

Spot instances - 

Linux SSH Public Key Authentication
Public key is stored with linux VM 
Private key stored in admin station

The default is SSH public key 
You need a public and private key together - they’re always a pair

It’ll create an IP address

Azure doesn’t store the private key. You want to download the private key and create a resource. Make sure you have a backup file

You can reset configuration if you’re not able to sign in using the public key credentials and you know you’re putting the correct information

The Putty tool is a GUI tool that you can use to make a remote SSH connection to manage SSH devices
SSD - Solid state drive
LUN - logical unit number or lun value
DAG - Desktop application Group

You create a key vault by going to create a resource in azure portal then putting key vault in the search bar then choose key vault.

You can access keys by going to key vault and clicking on keys on the right. 

Azure Virtual Desktop (AVD) is a cloud-based user virtual machine service or Desktop as a Service (DaaS) -aka Virtual desktop infrastructure (VDI)

AVD accesses web browser on windows or linux or install avd client for start menu integration. 

User accounts need to be in azure AD in order to access avd
User maust be assigned to use AVD and apps
Consider enabling MFA (Multi factor authentication)
Consider enabling condiciotna access polices like (specific user IP subnet, or geographic location)

AVD Host Pools is a resource that can be created in Azure
Grouping of identical VMs based on teh same VM image

Two types:
Personal: a user is assigned to a vm
Pooled: VM accepts any authorized user

Host pools is a grouping of VMs that users can connect to

Microsoft defender for cloud provides security related services
Allows protection for resources in Azure
Provide protection for resources in other cloud environment like AWS or google cloud platform
Also inventory on premises resources
Track vulnerabilities and provide recommendations
Can also resolve threats and can classify data you have

SDN (Software Defined Network)
Control plane is the interface
Data Plane is the actual transferring of network traffic

SDN Azure Applicability
NSG (Network Security Group)- is like a firewall that can be applied to vm network interface or can be applied to an entire subnet
NAT Gateway to allow outbound connectivity to the internet
Configure Azure Virtual WAN
Azure VPN Gateway
Azure load balancer

SDN Control plane
The customer doesn’t need to know detailed vendor-specific configuration details
This provides consistencey for cloud customers 

Consists of Azure portal GUI
Manage those things with CLI
Powershell
REST API 

Without SDN techiniicans would have to know how to configure all network infrastructure equipment or delegate to others. 

Azure makes sure that SDN interface is consistent so they create a SDN gateway controller. 
SDN gateway controller is software mechanism between control plane and data plane.  responsible for taking commands and configuring the equipment 

Azure VNets are managed through portal (VUI), CLI or programmatically. 
SDN is used to define VNEts in the azure cloud

Azure VNet Configuration Settings
Region
IPv4/IPv6 address space(s) or both
DDoS (Distributed denial of service) protection
Enable azure firewall

You configure azure VNets to isolate azure resources
VNets DNS settings can be customized
VMs can use private and public IPs
Site to site VPN can link to a Vnet
Vnets can be peered together

Subnets are created within a Vnet and subnet gets assigned an NSG (network security group) which is like a virtual firewall which controls traffic coming in and out of subnet. 
It also gets assigned a route table which is where you can make entries to control traffic flow
Subnet IP range must fallin within Vnet IP range
Subnet IP address range can be changed at any time

Bastion host is a role management point that allows us to get into remotely managed VM in subnet without a public IP. These VMs only have private IP. 

PowerShell has a file extension by default of .ps1

Azure Vnet peering is for better network performance
Vnet resources can connect with eachother via private IPs 

With Vnet peering 2 VMs that are not on the same subnet can connect and perform as if they were on the same subnet. 
Do not have to be on the same IP range

Vnets cna be within or spread among azure subscriptions or regions

Global vnet peering is when vnets from different regions connect with peering

Vnet peering is not transitive meaning if Vnet 1 is peering with Vnet 2 and Vnet 2 is peering with Vnet 3. Vnet 1 is NOT peered to Vnet 3. 

Azure Virtual Network Gateway
Max 1 VPN Gateway per Vnet 
represents a software VPN appliance in Azure
Each VPN gateway can support multiple connections

You need a subnet and it must be named “GatewaySubnet”
Gonna be used to contain 2 VMs which aren’t manageable so they won’t show up in your portal as a VM
They also won’t deploy any resources

Can use Vnet gateway to connect as an expressroute circuit - it’s a direct dedicated network circuit from an on premises network to azure cloud. It’s a dedicated network link to azure instead of going throug internet. 

Point-to-site (P2S) VPN - is used to allow individual device establish a vpn tunnel with an azure vnet. For ex. IPsec, SSTP (Secure Socket Tunneling protocol) is specific to windows, OpenVPN SSL/TLS is not specific to windows, linux, ios and android devices and MAC OS. 


Azure Content Delivery Network (CDN)
It’s a collection of worldwide Servers that have cached content to local users
Reduces network latency, improves app response time

It begins with a user requesting content through a url
If that content is cached it will be serviced through the nearest CDN or server 
If that content is NOT cached it will be pulled from an origin server 
The caching is done by 7 days (default) 

It’s built into Azure app services (web apps)
Azure media services - used to stream media
It’s also integrated into azure storage accounts

When are configuration settings to be aware of : 
Geofiltering
Content compression
Caching rules
Site acceleration

ExpressRoute - is a private dedicated WAN link from on-premises to Azure Vnet
The Vnet needs to have a Vnet gateway configured with a gateway subnet in the Vnet. This allows connectivity directly to Azure

Traffic is not traverse through the internet. 
ExpressRoute circuit is an Azure cloud resource
You’ll need a router technician on premises to configure 

Configuration settings include:
Provider
Peering location (city)
Bandwidth (50 Mbps - 10 Gbps

The unique identifier used to identify the ExpressRoute circuit GUID is the service key
The service key is a long code of numbers and letters
The unique service key is provided to the service provider
The provider status needs to be connected before you can start transmitting traffic through the circuit

Azure Managed disks
VMs need at least one OS disk

Azure Storage accounts can be deployed manually by customer or automatically by another service
It’s an object that supports a number of storage types like blobs (binary large object service), file service, table service or queue service. 

Azure blob storage - is an object or a file stored in an azure storage account
It’s unstructured data storage

There is a hierarchy in azure blob storage
At the top is the storage account 
You can create one or more blob containers
Within the containers you can upload or manage blobs (different file types)
You can configure the blob custom DNS domain names instead of using blob.core.windows.net

Azure Files are shared folders in the cloud, configured within a storage account
Accesscible via SMB (Server Message block)- normally used by windows file sharing or NFS - used by Linux typically

SMB uses port 445 and many providers block this by default

Configuring File shares:
Name
Quota in GiB - how much data can be stored into this azure file share done in Gbs
Storage tier - you can let is choose automatically or change it to hot or cool 

You can share files from on-premises ad to azure ad

Steps to configure Azure file sync
Create an azure file share
Create an azure file sync resource
Create a sync group in the azure file sync resource
Download and install azure file sync agent in on-premise file server
Register azure file sync agent with sync group

Azure blueprints - an automatic testing environment for testing or production that is preconfigured with vms web apps storage accounts etc. 

Allows for automated repeatable cloud confirugration 
Compliance with security standards

Artifacts are the individual components that make up a blueprint such as:
Resource groups
Role assignments
Policy assignments
ARM template - where you’re going to have the definition of which resources will be deployed and how they’ll be configured

Bluepirnt doesn’t need all these configurations but it can

Azure blueprint storage
Can store it in subriscription level or Management group

Azure blueprint parameters are values provided to blueprint artifacts during deployment
Parameters or hard-coded values are determined when artifacts are added to blueprint

Parameter ex:
Policy assignment - policy effect
RBAC role assignment - user, group, or app assignment
ARM template - configured parameters
Resource group - name , location
 
ARM and resource group can be hard-wired when you configure and save the blueprint or when you deploy it. 

Azure blueprint assignment
Assigne to an azure subricpstion 
Select appropriate blueprint version
Lock assignment (don’t lock, do not delete, read only)

Azure Blueprint Life Cycle
You can create Blueprint (draft mode)
Test and make necessary changes
Publish (assign, set version)

Azure Built-in RBAC Roles
Owner - full resource management control
Contributor - Resource control other than granting RBAC access
Reader - read only access
CDN (Content delivery Network) Endpoint Reader - read only access to content distribution network endpoints
Cost  Management Contributor - Read and write azure cost configurations, including budges
Virtual Machine administrator Login - Read VMs in the portal, login with admin credentials

RBAC Role assignments can be assigned to 
Users
Groups
Service principal - a dummy user account that’s used by a software that needs permissions and is managed by azure cloud administrator
Managed identity - is automatically managed by Azure

Resource tagging 
You can set up to 50 key and value pairs to each resource
Tagging helps track items by filtering

Azure monitoring and service health
Ensuring availabitlity and optimal performance with SLAs (Service Level Agreement)

Azure Monitor
Collects resource performance metrics
Collects resource logs
Monitor performance, query logs using KQL
Configure alerts, dashboards

You need an azure account in order to use most services
Azure app service will let you use it without an account
You need 1 or more azure subscriptions

Azure charges are tied to subscriptions - it’s a logical grouping of your azure services that are tied to 1 azure account. 

Resource groups exist in subscriptions
You can create resource groups ahead of deploying resource or as you’re creating them. But you NEED a resource group when deploying azure resources. 

Azure subscription types
Free trial
Pay as you go
Azure for students
Visual studio enterprise subscription
Azure pass - sponsorship 
MSDN (microsoft developer network) platform subscription
Enterprise Dev/Test - are used by larger enterprises
Azure subscription is tied to Azure AD tenants
Multiple subscriptions can be associated with a single tenant at a time. 

Azure management group are used by larger enterprises for larger subscriptions
They organize a hierarchy of subscriptions - you can assign policies to a management group which will then be inherited to all subscriptions in that group. .

ARM templates - are an automation mechanism in azure environment. You can manage, deploy or create resources.
IaC (Infrastructure as code) - Uses Json syntax. 
Resources like storage accounts, web apps, VMs databases, load balancers etc. 

Using “parameters” makes it so you can use template over and over again. 

You can deploy templates with CLI, Powershell or with azure portal 
You can specify variables in ARM template, name of VMs etc 
Github is owned by microsoft - it’s where version changes to code are done. 

You can create a windows or linux template in azure portal








Data Privacy - 
PII (Personally Identifiable Information)- it’s one or more piece of information that can be traced back to one person - For ex an address and phone number

Web browser cookies can be PII depending on what information is on them
Collection and storage of data is important

There are regulations for PII for the:
Protection of sensitive data
IAM (identity and access management)
HA (high availability)
Data sovereignty (replication of storage accounts)

PCI DSS (Payment card industry data security standard)
This is international
Merchant protection of cardholder data
Designed to harden payment card-processing environments

HIPAA (Health Insurance portability & accountability act) - an act of legislation that limits the disclosure of protected health information (PHI) or electronic protected health information (EPHI) 


Defense in depth
There are layers of security:
Perimeter firewalls, IDS/IPS (Intrusion detection systems) /(Intrusion prevention system) , VPN requirements, MFA (Multi factor authentication), encryption and host firewalls

Azure is compliant with many international regulations and security standards. It has azure firewall, custom DNS domains, P2S & S2S VPN, encryption of data at rest using customer managed keys. 
Azure AD user MFA
Azure DDos Mitigation
Azure Sentinel

Microsoft OST (Online services terms) discusses service level agreements (SLA) and costs & Acceptable use policies 
 Microsoft DPA (Data Protection agreement) - agreement to protect sensitive customer data in accordance to laws and regulations - sensitive collection, storage, disclosure, transfer & disposal
Security breach notification laws



Azure Advisor - is an advisor to what you can do to increase performance, or resiliency to failure. Save on costs or make your environment more secure. 

SLA is a contractual agreement between csp (azure) and the customer

Azure Firewall - is a managed service that we don't’ have to deploy. Just configure the rules. We can limit access to IP addresses or ports. 
It controls inbound and outbound network traffic - it’s a statefull firewall which means that instead of looking of individual packets it tracks the state of a session which can be multiple packets. 
A stateless firewall looks at individual packets
Requires a VNet subnet named “AzureFirewallSubnet”
It uses a static public IP address
You control the rules of traffic flow
Rule processing is based on priority number

One type of rule is a network rule -
You can specify the protocol such as -  TCP, UDP, ICMP or Any
You can specify the source and desticnation IP address
Destination port 
Allow or deny action

Application Rule - is specific to outbound connectivity
Specify fully qualified domain names (FQDNs)
Wildcards are allowed such as “.domain.com or* like *facebook.com
You can also specify the protocol: port  such as HTTPS:443
Allow or deny

The 3rd type of rule is Network Address Translation (NAT)
Source Network Address Translation (SNAT) - outgoing traffic assumes the public IP address of the azure firewall
Destination Network Address Translation (DNAT) - Translates public IP address and port to private IP address and port 

Azure Key Vault - storage that microsoft doens’t have access to. It’s a managed Azure resource that doesn’t need to be servers to be provisioned 
It provides centralized storage to security “secrets”
 
You can keep key vault secrets like an authentication string and you can set an expiration date and activation date
You can keep keys in the key vault - you can also set and activation and expiration date 
You can create a certificate 

It is FIPS compliant (Federal information processing standards) and can be backed with HSM support
Key vault access policy or RBAC permissions to vault
Key vault administrator
Key vault reader
Key vault certificates officer

Every azure storage account has 2 access keys that provide full access to the storage account
You can find the keys and connection string under settings in access keys

Azure Cost management
Charges are associated with azure subscriptions
Running cloud incurs costs
Running VMs is quoted per hour but you are charged per second
Storage costs are incurred 24/7 - like storage accounts or uploading blobs
Set cost budgets to set an amount to get notifications when you’ve reached the limit
Enable VM auto-shutdown
Scaling vertically always incurs more costs for things like:
	VMs 
	Databases

Reserved Pricing - 
	Applies to resources like VM, Azure MySQL database compute costs
Making a commitment over the long term from 1 to 3 years for these resources. You can get an enormous discount for committing to long term usage. 

You’d be doing this for constant resource usage (storage account, VM, database, etc)
Commitment to 1 to 3 years
For VMs, if size/series and region match existing or new VMs, reserved pricing applies up to purchased quantity

Azure Spot VM
Take advantage of unused compute capacity at up to 90% discount
Uptime is NOT guaranteed, not suitable for workloads that can’t handle interruptions
Sets a maximum price that when exceeded, your vm is deallocated or deleted depending on the configured eviction policy
Not for mission-critical work

Scalability is NOT automatic
IaaS is storage!
Azure cosmos db is a PaaS - No SQL database is fully managed no SQL 
API - application programming interface
SDK - software development kit


Basic Support Plan: The Basic support plan provides access to Azure documentation, knowledge bases, community forums, and basic technical support during business hours. It's suitable for customers with self-service support needs. Standard Support Plan: The Standard support plan includes all the features of the Basic plan, along with 24/7 technical support for critical issues, guaranteed initial response times, and access to advisory services. It's suitable for production workloads requiring enhanced support. Professional Direct Support Plan: The Professional Direct support plan offers all the features of the Standard plan, plus direct access to Microsoft engineers via phone and email for technical support. It provides personalized, proactive support for critical issues and is suitable for mission-critical environments. Premier Support Plan: The Premier support plan is the highest level of support offered by Microsoft and includes all the features of the Professional Direct plan, along with additional services such as proactive account management, workshops, training, and architectural reviews. It's tailored to meet the specific needs of enterprise customers with complex environments and critical business applications. These support plans offer different levels of assistance and expertise to help customers effectively manage and optimize their Azure environments.














China connects with azure with 21vianet.com

Infrastructure as code?

PostgreSQL?
Service principal 
Shared access signature?
What is an action group?
IAM (Identity access management)




















application virtualization (app streaming)
app containers (house app components only) - do not contain or start OS (operating systems)

Software-defined networking (SDN)
will grab commands and use it to configure equipment in datacenter

What is GRS, LRS, RA GRS





what does vpn stand for?
 Virtual Private Network (Shane)



# __Microsoft Azure Fundementals Study Notes__




<p align="center">
  <img src="https://github.com/DKC-Bluegeneral/Notes/blob/main/Images/AzureFundementals.png" alt="DKC-Bluegeneral">
</p>





## Domain 1: Describe Cloud Concepts (20-25%)


### Introduction to Cloud Computing

- **What is cloud computing?**

  - Cloud computing is the delivery of computing services over the internet, offering resources such as compute power, storage, databases, networking, and software on a pay-as-you-go basis. Users can access these resources remotely without the need for physical infrastructure.

### Cloud Service Models

- **Infrastructure as a Service (IaaS)**

  - IaaS provides virtualized computing resources over the internet. Users can rent virtual machines, storage, and other infrastructure components without managing physical hardware.

- **Platform as a Service (PaaS)**

  - PaaS offers a platform for developers to build, deploy, and manage applications without worrying about the underlying infrastructure. It provides tools and services for application development, such as databases, middleware, and development frameworks.

- **Software as a Service (SaaS)**

  - SaaS delivers software applications over the internet on a subscription basis. Users can access these applications through a web browser without the need for installation or maintenance.

### Cloud Deployment Models

- **Public Cloud**

  - Public cloud services are provided by third-party providers over the internet. Resources are shared among multiple users and managed by the service provider.

- **Private Cloud**

  - Private cloud infrastructure is dedicated to a single organization, either managed internally or by a third-party provider. It offers more control and customization but requires higher upfront costs.

- **Hybrid Cloud**

  - Hybrid cloud combines public and private cloud environments, allowing data and applications to be shared between them. It provides flexibility, scalability, and data sovereignty.

### Azure Management Tools

- **Azure Portal**

  - The Azure Portal is a web-based interface for managing Azure resources and services. It provides a unified view of your Azure environment and allows you to perform various administrative tasks, such as provisioning resources, monitoring performance, and managing access control.

- **Azure CLI**

  - The Azure Command-Line Interface (CLI) is a cross-platform command-line tool for managing Azure resources. It offers a command-line interface to perform tasks such as resource provisioning, configuration management, and deployment automation.

- **Azure PowerShell**

  - Azure PowerShell is a command-line scripting environment for automating Azure management tasks using PowerShell scripts. It provides cmdlets for interacting with Azure resources, managing subscriptions, and deploying infrastructure as code.

- **Azure Resource Manager (ARM)**

  - Azure Resource Manager (ARM) is the deployment and management service for Azure that provides a consistent management layer for resources. It enables you to group related resources into resource groups, deploy and manage resources as a single unit, and apply access control and policies across resources.

- **Resource Groups**

  - Resource groups are containers that hold related Azure resources for a specific application, solution, or workload. They provide a way to manage and organize resources, apply access control, and track costs for billing purposes.


### Resource Pooling

- Resource Pooling is a fundamental concept in cloud computing where multiple users or tenants share a common pool of computing resources, such as processing power, memory, storage, and network bandwidth. It allows for efficient utilization of resources and dynamic allocation based on demand, leading to cost savings and improved scalability.

### Hypervisors

- Hypervisors are software or firmware components that create and manage virtual machines (VMs) by abstracting physical hardware resources and providing virtualized environments for running guest operating systems. They enable server consolidation, workload isolation, and flexibility in deploying and managing virtualized infrastructure.

### VM Sprawl

- VM Sprawl refers to the proliferation of virtual machines (VMs) within an organization's IT environment, leading to inefficiencies, increased management overhead, and potential security risks. It occurs when VMs are provisioned and deployed without proper oversight or governance, resulting in unused or underutilized resources and increased complexity.

### Bastion

- Azure Bastion is a fully managed platform-as-a-service (PaaS) offering that provides secure and seamless RDP and SSH access to virtual machines (VMs) deployed in Azure without exposing them to the public internet. It eliminates the need for bastion hosts or jump servers and simplifies remote management and troubleshooting of VMs in Azure.

### Azure Total Cost of Ownership (TCO) Calculator

- The Azure Total Cost of Ownership (TCO) Calculator is a tool provided by Microsoft to help customers estimate and compare the total cost of running workloads in the Azure cloud versus an on-premises environment. It takes into account factors such as hardware, software, labor, and operational costs to provide a comprehensive analysis of cost savings and return on investment (ROI) for migrating to Azure.

### Azure Service Level Agreements (SLAs) and Refunds

- Azure offers industry-leading Service Level Agreements (SLAs) for its services, guaranteeing high levels of availability, performance, and reliability. In the event of service disruptions or violations of the SLA terms, Azure provides refunds or credits to customers as compensation for the impact on their business operations.

- For example, if Azure fails to meet the uptime guarantee specified in the SLA, customers may be eligible for service credits based on the percentage of downtime experienced. Azure applies a pro-rata credit for each impacted service based on the monthly service fees, which can be used to offset future Azure usage charges.


## Domain 2: Describe Core Azure Services (15-20%)


### Core Azure services

- **Azure Compute**

  - Azure Compute provides virtualized computing resources to run applications and workloads. It includes services like Virtual Machines (VMs), Azure App Service, and Azure Functions.

- **Azure Storage**

  - Azure Storage offers scalable and durable cloud storage solutions for data storage needs. Key services include Blob Storage, Azure Files, and Azure Queue Storage.

- **Azure Networking**

  - Azure Networking facilitates the connection and communication between various components and services deployed on Azure. It includes services such as Virtual Network (VNet), Azure Load Balancer, and Azure VPN Gateway.

- **Azure Databases**

  - Azure Databases provide managed database services for storing and managing structured data. Examples include Azure SQL Database, Azure Cosmos DB, and Azure Database for MySQL.

- **Azure Identity**

  - Azure Identity services enable secure access management and identity authentication for users and applications. Services include Azure Active Directory (AD), Azure AD B2C, and Azure AD B2B.

### Azure Stack

- Azure Stack is an extension of Azure that enables organizations to deploy Azure services and applications on-premises or at the edge for scenarios requiring data sovereignty, low-latency, or disconnected environments. It provides consistent development, management, and operations experiences across hybrid cloud deployments.

### Azure Arc

- Azure Arc is a hybrid cloud management solution that extends Azure management and governance capabilities to resources outside of Azure, such as on-premises servers, Kubernetes clusters, and edge devices. It enables centralized management, policy enforcement, and monitoring of distributed resources using familiar Azure tools and services.

### Azure Data Center Components

- Azure Data Centers are state-of-the-art facilities that house the physical infrastructure and equipment required to operate Azure cloud services. Key components of Azure Data Centers include servers, storage arrays, networking hardware, power distribution units (PDUs), cooling systems, and physical security measures to ensure high availability, reliability, and security of cloud services.

### Azure Regions, AZ's, and Service Availability

- Azure Regions are geographic locations around the world where Azure resources and services are deployed and hosted. Each Azure Region consists of one or more data centers that are interconnected through high-speed networks and redundant infrastructure. Availability Zones (AZs) are unique physical locations within an Azure Region with independent power, cooling, and networking to ensure resilience and high availability of services.

### Spot Instances

- Azure Spot Instances are virtual machines (VMs) that are offered at significantly discounted prices compared to standard pay-as-you-go rates. They are ideal for workloads that can tolerate interruptions and have flexible timing requirements, such as batch processing, dev/test environments, or fault-tolerant applications.

### Azure Governance and Compliance

- **Azure Policy**

  - Azure Policy is a service that allows you to enforce and enforce rules and policies across your Azure environment to ensure compliance with organizational standards and regulatory requirements. It enables you to define and apply policies for resource configuration, access control, and security settings.

- **Azure Blueprints**

  - Azure Blueprints is a service that allows you to define a repeatable set of Azure resources, policies, and permissions as a blueprint for deploying standardized environments. It enables you to enforce organizational standards and best practices for governance, compliance, and security.

### Azure Monitoring and Management

- **Azure Monitor**

  - Azure Monitor is a comprehensive monitoring service for collecting, analyzing, and acting on telemetry data from Azure and on-premises environments. It provides insights into the performance, health, and availability of your applications and infrastructure, with features such as metrics, logs, alerts, and dashboards.

- **Azure Advisor**

  - Azure Advisor is a personalized recommendation service that helps you optimize your Azure resources for performance, security, reliability, and cost-efficiency. It analyzes your Azure usage and configurations to provide actionable recommendations for improving your deployments and reducing costs.

- **Azure Log Analytics**

  - Azure Log Analytics is a service that allows you to collect, analyze, and visualize log and telemetry data from your Azure resources and on-premises environments. It provides insights into system and application performance, security threats, and operational issues, with features such as query language, dashboards, and machine learning.

### Azure Networking

- **Azure Virtual Network (VNet)**

  - Azure Virtual Network (VNet) is a network isolation boundary within Azure that enables you to securely connect Azure resources and extend your on-premises networks to the cloud. It provides features such as subnetting, network security groups (NSGs), and virtual private network (VPN) gateways for controlling traffic flow and enforcing security policies.

- **Azure Load Balancer**

  - Azure Load Balancer is a Layer 4 (TCP/UDP) load balancer service that distributes incoming network traffic across multiple backend resources, such as virtual machines, virtual machine scale sets, and Azure Kubernetes Service (AKS) clusters. It improves application availability, scalability, and reliability by evenly distributing traffic and detecting and rerouting failed resources.

- **Azure Application Gateway**

  - Azure Application Gateway is a Layer 7 (HTTP/HTTPS) load balancer service that provides advanced application delivery and security features for web applications. It includes features such as SSL termination, URL-based routing, session affinity, and web application firewall (WAF) for optimizing and securing your web traffic.

### Azure Identity and Access Management (IAM)

- **Azure Active Directory (AD)**

  - Azure Active Directory (AD) is a cloud-based identity and access management service that provides single sign-on (SSO), multi-factor authentication (MFA), role-based access control (RBAC), and identity governance capabilities for securing access to Azure resources and applications. It serves as the identity foundation for Azure and integrates with thousands of SaaS applications.

- **Azure AD B2C (Business to Consumer)**

  - Azure Active Directory B2C (Azure AD B2C) is a cloud identity service that enables you to provide secure authentication and authorization for customer-facing applications and websites. It supports user authentication with social identity providers (e.g., Facebook, Google, Microsoft accounts) and provides customizable sign-up and sign-in experiences for end users.

- **Azure AD B2B (Business-to-Business)**

  - Azure Active Directory B2B (Azure AD B2B) is a collaboration service that enables you to securely share your organization's applications and resources with external users, such as partners, vendors, and contractors. It allows you to invite external users to access your applications using their own credentials while maintaining control over access policies and permissions.


## Domain 3: Describe Security, Privacy, Compliance, and Trust (25-30%)


### Security

- **Azure Security Center**

  - Azure Security Center provides unified security management and advanced threat protection across hybrid cloud workloads.

- **Azure Sentinel**

  - Azure Sentinel is a cloud-native security information and event management (SIEM) service that provides intelligent security analytics and threat intelligence.

### Privacy

- **Data Encryption**

  - Azure offers encryption at rest and in transit to protect data confidentiality and integrity. Encryption mechanisms include Transparent Data Encryption (TDE), Azure Disk Encryption, and Azure Storage Service Encryption (SSE).

### Compliance and Trust

- **Compliance Offerings**

  - Azure complies with various industry standards and regulations, such as GDPR, HIPAA, ISO, and SOC. It provides compliance offerings and certifications to meet the regulatory requirements of different industries and geographies.

- **Trust Center**

  - The Azure Trust Center provides resources and information about Azure's commitment to security, privacy, compliance, and transparency. It offers compliance documentation, reports, and audit information for customers and regulators.


  ### Azure Key Vault

- Azure Key Vault is a cloud-based service that enables customers to securely store and manage cryptographic keys, secrets, and certificates used for encrypting data, authenticating users, and securing applications. It provides centralized key management, access control, and auditing capabilities to protect sensitive information and comply with regulatory requirements.

### Azure Blueprint

- Azure Blueprints are a set of pre-defined configurations, policies, and resource templates that help organizations deploy and govern compliant Azure environments at scale. They provide a repeatable and standardized way to define and enforce governance controls, security baselines, and best practices for cloud deployments.

### Azure built-in RBAC roles, provide examples.

- Azure Role-Based Access Control (RBAC) provides fine-grained access management for Azure resources and services through pre-defined roles with specific permissions. Examples of built-in RBAC roles include:

  - Owner: Full access to all resources and can manage access to resources.

  - Contributor: Can create and manage all types of Azure resources but cannot grant access to others.

  - Reader: Can view all resources but cannot make any changes.

  - User Access Administrator: Can manage user access to Azure resources.

  - Security Administrator: Can manage security-related operations, such as configuring security policies and managing security alerts.


## Domain 4: Describe Azure Pricing, Service Level Agreements, and Lifecycles (20-25%)


### Azure Pricing

- **Pay-As-You-Go**

  - Azure offers a pay-as-you-go pricing model, where customers pay only for the resources they use without any upfront costs or long-term commitments. It provides flexibility and cost-effectiveness for varying workload demands.

- **Reserved Instances**

  - Azure Reserved Instances allow customers to reserve virtual machines for a one- or three-year term, offering significant discounts compared to pay-as-you-go pricing. It provides cost savings for predictable workloads with steady usage patterns.

### Service Level Agreements (SLAs)

- **SLA Overview**

  - Azure provides SLAs for its services, guaranteeing uptime, performance, and reliability. SLAs specify the level of service availability and response times, with compensation offered for any service disruptions that violate the SLA terms.

### Service Lifecycles

- **Azure Service Lifecycle**

  - Azure services follow a lifecycle management process, including introduction, growth, maturity, and retirement phases. Microsoft provides advance notice and support for customers during service retirement to ensure a smooth transition to alternative solutions.

### Resource Tagging

- Resource Tagging is a practice of assigning metadata tags to Azure resources to categorize, organize, and track them based on attributes such as environment, department, cost center, or project. It enables consistent resource management, cost allocation, and reporting across Azure subscriptions, helping organizations optimize spending and improve governance.

### Azure Subscription Types

- Azure offers various subscription types to meet the diverse needs and requirements of customers, including:
  - Pay-As-You-Go: Flexible pricing model with no upfront costs and pay-only-for-what-you-use billing.
  - Azure Enterprise Agreement (EA): Volume licensing agreement for large organizations with predictable usage and discounted pricing.
  - Azure Free Account: Trial subscription with limited usage and credits to explore Azure services for free.
  - Azure Sponsorship: Subscriptions provided through partnerships or sponsorships, such as MSDN subscriptions or educational grants.

### Infastructure as code

- Infrastructure as Code (IaC) is an approach to managing and provisioning infrastructure resources using machine-readable definition files, such as templates or scripts, rather than manual processes. It allows for automated, repeatable, and consistent deployment of infrastructure configurations, reducing errors, improving scalability, and enabling version control.

### PostgreSQL

- PostgreSQL is an open-source relational database management system (RDBMS) that is supported as a fully managed service on Azure. It provides features such as ACID compliance, JSON support, scalability, and extensibility, making it suitable for a wide range of applications and workloads.

### Action groups

- Azure Action Groups are a collection of notification preferences and actions that define how alerts are triggered and responded to in Azure Monitor. They allow users to define a set of actions, such as sending emails, SMS messages, or webhook notifications, and associate them with alert rules for automated incident response and remediation.

### IAM

- Identity and Access Management (IAM) is the practice of managing digital identities, authentication, and authorization for accessing resources and services in a secure and controlled manner. In Azure, IAM encompasses services such as Azure Active Directory (AD), role-based access control (RBAC), multi-factor authentication (MFA), and conditional access policies.

### Service Principal

- A Service Principal is a security identity used by applications, services, and automation tasks to access Azure resources and services securely. It provides a way to authenticate and authorize applications without requiring user credentials and enables controlled access to specific resources through role-based access control (RBAC) permissions.


## Additional Topics


### Azure Networking

- **Azure Virtual Network (VNet)**

  - Azure Virtual Network (VNet) is a network isolation boundary within Azure that enables you to securely connect Azure resources and extend your on-premises networks to the cloud. It provides features such as subnetting, network security groups (NSGs), and virtual private network (VPN) gateways for controlling traffic flow and enforcing security policies.

- **Azure Load Balancer**

  - Azure Load Balancer is a Layer 4 (TCP/UDP) load balancer service that distributes incoming network traffic across multiple backend resources, such as virtual machines, virtual machine scale sets, and Azure Kubernetes Service (AKS) clusters. It improves application availability, scalability, and reliability by evenly distributing traffic and detecting and rerouting failed resources.

- **Azure Application Gateway**

  - Azure Application Gateway is a Layer 7 (HTTP/HTTPS) load balancer service that provides advanced application delivery and security features for web applications. It includes features such as SSL termination, URL-based routing, session affinity, and web application firewall (WAF) for optimizing and securing your web traffic.

### Azure Identity and Access Management (IAM)

- **Azure Active Directory (AD)**

  - Azure Active Directory (AD) is a cloud-based identity and access management service that provides single sign-on (SSO), multi-factor authentication (MFA), role-based access control (RBAC), and identity governance capabilities for securing access to Azure resources and applications. It serves as the identity foundation for Azure and integrates with thousands of SaaS applications.

- **Azure AD B2C**

  - Azure Active Directory B2C (Azure AD B2C) is a cloud identity service that enables you to provide secure authentication and authorization for customer-facing applications and websites. It supports user authentication with social identity providers (e.g., Facebook, Google, Microsoft accounts) and provides customizable sign-up and sign-in experiences for end users.

- **Azure AD B2B**
  - Azure Active Directory B2B (Azure AD B2B) is a collaboration service that enables you to securely share your organization's applications and resources with external users, such as partners, vendors, and contractors. It allows you to invite external users to access your applications using their own credentials while maintaining control over access policies and permissions.

### Azure Total Cost of Ownership (TCO) Calculator

- The Azure Total Cost of Ownership (TCO) Calculator is a tool provided by Microsoft to help customers estimate and compare the total cost of running workloads in the Azure cloud versus an on-premises environment. It takes into account factors such as hardware, software, labor, and operational costs to provide a comprehensive analysis of cost savings and return on investment (ROI) for migrating to Azure.

### Azure Service Level Agreements (SLAs) and Refunds

- Azure offers industry-leading Service Level Agreements (SLAs) for its services, guaranteeing high levels of availability, performance, and reliability. In the event of service disruptions or violations of the SLA terms, Azure provides refunds or credits to customers as compensation for the impact on their business operations.

- For example, if Azure fails to meet the uptime guarantee specified in the SLA, customers may be eligible for service credits based on the percentage of downtime experienced. Azure applies a pro-rata credit for each impacted service based on the monthly service fees, which can be used to offset future Azure usage charges.

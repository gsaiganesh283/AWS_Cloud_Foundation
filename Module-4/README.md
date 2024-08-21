# AWS Cloud Security
## AWS Shared Responsibility model
### AWS Responsibility: Security of the Cloud
**Physical Security of data centers**
- Controlled, need-based access
  
**Hardware and Software infrastructure**
- Storage decommissioning, host operating system access logging, and auditing.
  
**Network infrastucture**
- Intrusion delection
  
**Virtualization Infrastructure**
- Instance isolation
### Customer Responsiblity: Security in the Cloud
- Amazon Elastic Compute Cloud (Amazon EC2) instance OS
  - Including patchong, Maintance
- Applications
  - Passwords, Role-based Access, etc...,
- Security group configuration
- OS or Host-based firewalls
  - Includeing intrusion detection or preventation systems.
- Network Configurations
- Account Management
  - Login and Permission setting for each user

### Service Characteristics and Security Responsibility
#### Infrastructure As a Service (IaaS)
- Customer has more flexibility over configuring networking and storage settings
- Customer is responsible for managing more aspects of the security
- Customer configures the access controls
#### Platform As a Service (PaaS)
- Customer does not need to manage the uderlaying infrastructure
- AWS handles the operating system, Database patching, firewall configuration, and disaster recovery.
- Customer can focus on managing code or data.
#### Software As a Service (SaaS)
- Software is centrally hosted
- Licensed on a subscription model or Pay-As-You-Go basis.
- Service are typically accessed via web browser, mobile app, or application program.
- Customers do not need to manage the infrastructure that support the service.
## AWS Identity and Access Management (IAM)
Use IAM to manage access to AWS resources
- A resource is an entity in an AWS account that you can work with the software
  
**Example** - Control who can terminate Amazon EC2 instances

Define fin-grained access rights
- who can access the resource
- which resources can be accessed and what can the user do to the resource
- How resource can be accessed.

IAM is a no-cost AWS account feature

### IAM: Essential Components
#### IAM User
A person or application that can authenticate with an AWS account
#### IAM group
A collection of IAM users that are granted identical authorization.
#### IAM Ploicy
The document that defines which resources can be accessed and the level of access to each resource.
#### IAM Role
Useful mechanism to grant a set of permission for making AWS service requests.
### Authenticate as an IAM user to gain access
When you define an IAM user, you select what types of access the user is permitted to use.
#### Programmatic Access
**Authenicate Using:**
- Access Key ID
- Secret access Key
**Provides AWS CLI and AWS SDK access**
#### AWS Management Console Access
**Authenicate Using:**
- 12-digit Account ID or alias
- IAM username
- IAM Password

If enabled, multi-factor authentication (MFA) prompts for an authentication code.

**IAM MFA**
- MFA provides increased security
- In addition to username and password, MFA requires a unique authentication code to access AWS services.

#### IAM: Authorization
- Assign permission by creating an IAM policy
- Permission determine which resources and operations are allowed.
  - All permissions are implicity denied by default.
  - If something is explicity denied, it is never allowed.
**Note:** The scope of IAM service configurations is global setting apply across all AWS regions.
#### IAM Policies
An IAM polocy is document that defines permissions
- Enables fine-grained access control
**Two types of policies**
  - Identity-based and
  - Resource-based
  ##### Identity-based
  Attach a policy to any IAM entity
  - An IAM user, an IAM group, or an IAM role
  - Actions that may be performed by the entity
  - Actions that may not be performed vy the entity
  - Single polocy can be attached to multiple entites
  - Single entity can have multiple policies attached to it.
  #### Resource-based policies
  Attached to a resource **(Such as an S3 bucket)**
#### IAM Group
- An IAM group is a collection of IAM users.
- A group is used to grant the same permission to multiple users.
  - Permission granted by attaching IAM policy or policies to the group
- A user can belong to multiple groups
- There is no default group
- Groups cannot be nested.
  

# Practical 1

Source PDF: Practical 1.pdf

--- Page 1 ---

Practical 1
AIM: To study cloud architecture and cloud computing model.


Architecture of Cloud Computing
Cloud computing architecture is the arrangement of all the hardware, software, network,
storage, and services that work together to deliver cloud services to users.




Cloud Computing Model
A cloud computing model is a method that explains how users access and use cloud
resources and services over the internet.




Cloud Service Model
A Cloud Service Model defines what type of service a cloud provider offers to users over
the internet. It tells us who manages what (hardware, operating system, applications, etc.)
between the cloud provider and the user.

--- Page 2 ---

There are three main cloud service models:
   1. IaaS (Infrastructure as a Service)
   2. PaaS (Platform as a Service)
   3. SaaS (Software as a Service)



1. IaaS (Infrastructure as a Service)
Definition
IaaS provides virtual infrastructure such as servers, storage, networking, and virtual
machines over the internet.
What the Cloud Provider Manages
   •   Physical servers
   •   Storage
   •   Networking
   •   Virtualization
What the User Manages
   •   Operating System
   •   Applications
   •   Data
   •

Features
   •   Users can create virtual machines.
   •   Resources can be increased or decreased as needed.
   •   Pay only for the resources you use.
Examples
   •   AWS EC2
   •   Azure Virtual Machines
   •   Google Compute Engine

--- Page 3 ---

2. PaaS (Platform as a Service)
Definition
PaaS provides a ready-to-use platform where developers can build, test, and deploy
applications without managing the underlying infrastructure.
What the Cloud Provider Manages
   •   Infrastructure
   •   Operating System
   •   Runtime Environment
   •   Storage
   •   Networking
What the User Manages
   •   Application code
   •   Data
Features
   •   No need to install or maintain servers.
   •   Faster application development.
   •   Supports multiple programming languages.
Examples
   •   Google App Engine
   •   Azure App Service



3. SaaS (Software as a Service)
Definition
SaaS provides ready-to-use software applications over the internet.
What the Cloud Provider Manages
   •   Infrastructure

--- Page 4 ---

•   Operating System
   •   Software
   •   Security
   •   Updates
   •   Maintenance
What the User Does
   •   Simply logs in and uses the software.
Features
   •   No installation required.
   •   Accessible from anywhere with an internet connection.
   •   Automatic updates and maintenance.
Examples
   •   Gmail
   •   Google Docs
   •   Microsoft 365
   •   Zoom


A cloud deployment model is the way a cloud environment is set up and made available
to users or organizations.
There are 4 types of Cloud Deployment Models:
   1. Public Cloud
   2. Private Cloud
   3. Hybrid Cloud
   4. Community Cloud



   1. Public Cloud
Definition
A Public Cloud is a cloud environment where services are available to everyone over the
internet. It is owned and managed by a third-party cloud provider.

--- Page 5 ---

Features
   •   Available to anyone with an internet connection.
   •   Low cost because resources are shared among many users.
   •   Easy to scale resources up or down.
Advantages
   •   No need to buy hardware.
   •   Pay only for what you use.
Disadvantages
   •   Less control over the infrastructure.
   •   May not be suitable for highly sensitive data.
Examples
   •   AWS (Amazon Web Services)
   •   Microsoft Azure



   2. Private Cloud
Definition
A Private Cloud is a cloud environment used only by one organization. It can be managed
by the organization itself or by a third party.
Features
   •   Used by a single organization.
   •   Provides high security and privacy.
   •   Offers greater control over resources.
Advantages
   •   Better security.
   •   Full control over data and infrastructure.
Disadvantages
   •   More expensive.
   •   Requires maintenance and management.
Example

--- Page 6 ---

A bank or hospital using its own private cloud.


   3. Hybrid Cloud
Definition
A Hybrid Cloud combines Public Cloud and Private Cloud. Organizations can keep sensitive
data in the private cloud and use the public cloud for less sensitive tasks.
Features
   •   Combines both public and private clouds.
   •   Data can move between both environments.
   •   Provides flexibility and scalability.
Advantages
   •   Better security for sensitive data.
   •   Cost-effective and flexible.
Disadvantages
   •   More complex to manage.
   •   Requires proper integration between clouds.
Example
A company stores employee records in a private cloud and hosts its website on AWS.




   4. Community Cloud
A Community Cloud is a cloud deployment model in which the same cloud infrastructure is
shared by multiple organizations that have similar needs, goals, or security requirements.
Features
   •   Shared by two or more organizations with similar needs.
   •   Organizations share the cost, resources, and infrastructure.
   •   Provides better security than a public cloud.
   •   Managed by one or more organizations or by a third-party provider.


Advantages

--- Page 7 ---

•   Cost is shared among organizations.
   •   Better security and privacy than a public cloud.


Disadvantages
   •   Less flexible than a public cloud.
   •   Management can be more complex because multiple organizations share the cloud.


Examples
   •   Hospitals sharing patient records securely.




Architecture of Cloud Computing
How the cloud system is designed and how different parts work together.

--- Page 8 ---

1. The Frontend (Client Side)
The frontend is the visible side of the cloud computing system. It contains all the user interfaces and client
infrastructure required for end-users to interact with the cloud.
   •   Client Infrastructure: The hardware and software components (like a laptop, mobile phone, or web
       browser) that provide a Graphical User Interface (GUI) to access cloud services.



2. Internet
   Connects users to cloud services.
    A stable internet connection is required to access the cloud.
   Example: Wi-Fi or mobile data connecting to cloud servers.



3. The Backend
The backend is the "cloud" itself. Managed by the service provider, it houses the core resources, manages
traffic, deploys models, and enforces security.
1. Application
The application is the software that user access through the cloud.

--- Page 9 ---

Example: Gmail


2. Service
A service is a cloud facility provided to users, such as storage, databases, or virtual machines.
Example: AWS EC2


3. Cloud Runtime
Cloud Runtime is the environment where applications are executed.
Example: Java Runtime


4. Storage
Storage is used to save data in the cloud.
Example: Google Drive


5. Infrastructure
Infrastructure is the physical and virtual hardware that supports cloud computing.

Example: AWS Data Centers


6. Management
Example: AWS Management Console


7. Security
Example: Multi-Factor Authentication (MFA)

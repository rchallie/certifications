# Cloud concept
## What is AWS and its value proposition:
[What is AWS](https://aws.amazon.com/what-is-aws/)
AWS is the cloud platform of amazon, offering over 200 featured services. Interresting to lower costs, become more agile and innovate faster.
### Advantages of AWS cloud:
[Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/?pg=WIAWS-N&tile=learn_more)
- Security:
Is built to satisfy security requirements for the military, global banks and other high-sensitivity organizations. Usage of security tool with 230 secutiry, compliance and governance services. Support 90 security standards ans compliance certifications. The 117 AWS service that store customer data offer to encrypt datas. The infrastrucure is monitored 24/7 to help ensure the confidentiality of datas. Data flowing accros global network is encrypted at the physical layer before leaves secured facilities. User can control data: encrypt it, move it, manage it.
- Availability:
Provide offers as many Regions with multiple avaibility zones connected by low atency, high throughput and redundant networking. AWS hase 81 avaibility zones within 25 geographic regions. The AWS Region and avaibility zone is recommended for running entreprise applications that require high avaibility. It's possible to split applications in multiple zones in the same region to isolated possible problems. AWS control planes and management console are distribued across regions and include regional API endpoints to allow the the customer to access it, during 24 hours is isolated from the global control plane, without external networks.
- Scalability:
AWS Global Infrastructure enables companies to be flexible by the infinite scalibility of the cloud. Ensure customers they had enought capacity at the peak level of activity. Provide the amount of resources that actually needed, with the possibility to instanly scale up or down along which also reduces cost and match customer's ability with users's demandes. Possibility to deploying thousands of servers in minutes.
- Flexibility:
Give the flexibility of choosing how and where you want to run your workloads, so use the same network, contorl plane, API's and AWS Services. Chosse any AWS region to run applications globally, or a specific region for a reason (like need latencies to mobile devices) with AWS Local Zones or AWS Wavelength. Run applications on-premises with AWS Outposts.
- Pay-as-you-go:
Pay only for the individual services needed, without long-term contracts or complex licensing. Pay for the services consumed and once the services are stoped, ther are no additional costs or termination fees. 
- Save on reserve:
Can invest on reserved capacity (ex: EC2, Amazon RDS). With Reserved Instances, save up to 75% over equivalent on-demande capacity. The larger the upfront payment, the greater the discount.
- Economie of scale:
Get volume based discounts and realize important saving as the usage increases. 
(ex S3, pricing is tiered, more use = less pay per GB). AWS give options to acquire services that help to address business needs.
### How AWS Cloud allow customer to focus on operational value:
AWS Cloud give services in many areas, enought for that the customer may be focus on income generator activities, not on the infrastructure.
## AWS Cloud and economic aspects:
### Content of the total cost of ownership proposal:
- OpEx (Functionnary costs): are the current charges to exploit services.
- CapEx (Investment): The investment on services to be profitable in the long term.
- On-site operations labor costs: The total management of an infrastructur on-site require to invest on servers bay, skilled workers, time, constant security check etc.     
by definition a certain amount of money.
- Software Licence: The user of a licence pay a higher starting cost, next he will pay maintenance costs, updates, and support.
### How reduct costs when using the cloud
- Infrastructure with an adapted size: The best way to doesn't pay to much is to have a to pay only that those which are necessary. Saved on reserve can be more iterresting if the usage is not contant, otherwise the best is to use/pay only what it needed.
- Automation advantages:
	- it reduce costs
	- redirect the productivity on other tasks
	- disponibility (ex: data redundancy on multiple disks)
	- increase the fiability, human error is possible where a computer with a script will do the exact same task in the same way
	- automation increase performances of a system
- Scope of conformity: Reform data used / stocked to don't invest time / money on certifications or licenses. 
-  Managed services: The best stay to adapt used services, and use managed services, like ECS or EKS (managed cluster or managed kubernetes)
## Fundamental cloud architecture model 
### Explain model principles
- Failsafe: Is a model method permitting to a system to continue to work, possibly throttled but not totally killed, when a component doesn't work properly.
- Difference between splitted component and a monolithic architecture: Split an application in different component (in micro-services), like multiple containers (Ex: 1: API, 2: DB, 3: Frontend etc..) help an application to be failsafe, start each part of the application in parrallel, update only one part to don't have to stop everything and a repatirtion of erratic workloads. Monolithic architecture is the invert of all the good points of splitted component, excepted that everything is at the same place.
- Cloud vs on-site elasticity: On cloud it's easy to expand applications by adding services, on-site it possible to, but it has a cost (ex: add physical servers) 
# Security and compliance
## Define the shared responsability design (AWS)
[Shared responsabily model (FR)](https://aws.amazon.com/fr/compliance/shared-responsibility-model/)
### Elements of the shared responsability model
This model distribute responsability between AWS (Hardware, availibility, networking etc..) and the customer (Used applications, laws, encryption etc..)
- AWS responsability : This model permetted to reduce the customer's operational burden. AWS execute, manage and control the components from the OS to the virtualization layer passing by the physical security of intallations.
-  Customer responsaibility: The customer have the responsability of the guest OS, the executed applications (update & security), the group firewall provides by WAS, the laws relevant to the applications, data security (encryption) and the integrations of used services. This model of responsability provide a flexibility that give some control to the customer.![Amazon shared responsability model](https://d1.awsstatic.com/security-center/Shared_Responsibility_Model_V2.59d1eccec334b366627e9295b304202faf7b899b.jpg)
## Security and compliance concept (AWS)
### Where can be found AWS compliance informations:
[AWS Compliance ressources](https://aws.amazon.com/compliance/resources/)
[AWS Compliance program](https://aws.amazon.com/compliance/programs/)
The compliance requierement vary between applications, it depends of the region and of components aims , the level of security depends often of the critical level/type of datas (RGPD != PCI != HIPAA...), the customer have the responsability to adapt security and compliance. 
### How the customer can respect compliance:
AWS provide tools to respects compliances like AES (AES-256) the strongest industry-adopted and government-approved algorithm for encrypting data, used by Amazon S3 for server-side encryptin.
- Protecting key as rest: Best way to encrypting data is to stored the key in an HSM (Hardwars security modul) a specialised computing device that has several security controls built into it to. Amazon provide KMS (AWS Key Management Service) to manage keys using AWS system or CloudHSM to manage keys using own HSM.
- In motion: Encrypt datas transmissions using TLS. AWS Certificate Manager and AWS Private Certificate Authority, are two services used to manage and rotate certificates accros infrastructures. AWS s2n is an open source implementation of TLS.

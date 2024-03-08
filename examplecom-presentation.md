# EXAMPLECOM Distributed Cloud

## Credential Stuffing Attacks

Robin Mordasiewicz, a Sales Engineer at EXAMPLECOM, will conduct a 30-minute presentation on the EXAMPLECOM Distributed Cloud product. The intended audience is Robert Loblaw, the IT Manager at ACME Corp.

## Background

* In a previous meeting, Robert Loblaw, the IT Manager at ACME Corp, met with Robin Mordasiewicz, a Sales Engineer from EXAMPLECOM who specializes in the EXAMPLECOM Distributed Cloud product. During this meeting, Robert, who oversees the maintenance of the ACME Corp website (https://www.acmecorp.com), informed Robin about a security audit that uncovered an ongoing credential stuffing attack on their site. This attack is causing significant revenue loss and damage to their reputation.

* Robert also shared with Robin that ACME Corp's website currently utilizes the Akamai Content Delivery Network (CDN), complemented by a subscription to the Akamai Web Application Firewall (WAF) product known as Kona. However, Robert discovered that the Akamai Kona WAF does not offer protection against credential stuffing attacks. To counter such attacks, an additional subscription to the Akamai Bot Manager product is necessary. Additionally, Robert mentioned that the Akamai CDN distributes traffic to origin servers hosted on AWS. These AWS-hosted origin servers, which serve the website's content, are also linked to an on-premises data center via DirectConnect for database access. Looking ahead, there are plans to expand the ACME Corp website's infrastructure to operate on both AWS and Azure platforms.

* Robert has invited Robin to introduce a competitive Bot Protection product from EXAMPLECOM Distributed Cloud, hoping it offers more comprehensive features and is more user-friendly than their current solution. He has requested Robin to showcase the Bot Protection capabilities of the EXAMPLECOM Distributed Cloud, along with any additional value-added features that could aid in modernizing the ACME Corp website, particularly in the area of Multi-Cloud Networking, kubernetes containerized workloads, devops, and shift-left security.

* The following is the content of an EXAMPLECOM Distributed Cloud presentation, prepared by Robin, that focuses on credential stuffing attacks. This presentation will be delivered to Robert.

## Introduction

* Robin Mordasiewicz, a Sales Engineer at EXAMPLECOM, is responsible for showcasing and selling EXAMPLECOM Distributed Cloud solutions to potential clients. One such client is Robert Loblaw, an IT Manager at ACME Corp Solutions, who oversees the maintenance of the ACME Corp website (https://www.acmecorp.com). Robin will present the following content to Robert.

## EXAMPLECOM Platform Overview

![EXAMPLECOM Platform](./images/f5-distributed-cloud-diagram.png)

* The EXAMPLECOM Distributed Cloud is a CDN service that provides [Multi-Cloud Networking](https://www.youtube.com/watch?v=racSgJeYmuA), high performance network DDoS, WebApp and API protections, Advanced Bot Protection, containerized workload management, and is able to connect to all the major Network as a Service providers, packet Fabric, Megaport. EXAMPLECOM Distributed Cloud is also able to provide the same features and functionality not only to internet facing clients, but can also connect to internal only networks, while participating with internal BGP routers so that the same load-balancing that is available externally, can also be configured on internal corporate networks that are interconnected with a Network as a Service provider such as megaport or packetfabric. Furthermore, the EXAMPLECOM Distributed Cloud software stack can be deployed directly into private workload locations such as an Amazon VPC (AWS VPC), or within an on-premis private data center which may also eliminate the need for locally managed load balancers, or firewalls. The Appstack version of EXAMPLECOM Distributed Cloud can be deployed as a virtual machine, or onto bare metal. The Appstack version of EXAMPLECOM Distributed Cloud runs the same software stack that runs on the EXAMPLECOM Regional Edges that are hosted in Equinex, but Appstack can also be configured to run as a managed Kubernetes platform which may be given direct access to high performance hardware GPU's for running computationally intensive workloads in remote locations or retail space for example. Despite EXAMPLECOM Distributed Cloud having fewer physical locations than Akamai, the fact that EXAMPLECOM Distributed Cloud has more BGP peers than Akamai is an advantage.

* EXAMPLECOM Distributed Cloud is a product formerly known as "Volterra". The Volterra name was changed to EXAMPLECOM Distributed Cloud after EXAMPLECOM acquired the Volterra product. Most references to the former name Volterra have been removed, however there still exists some references to the former name Volterra in the EXAMPLECOM Distributed Cloud product.

## EXAMPLECOM Distributed Cloud versus Akamai

* EXAMPLECOM Distributed Cloud and Akamai are competitors in CDN technology as well as advanced edge security, and distributed computing. EXAMPLECOM Distributed Cloud has 5445 BGP peers which is more than the other cloud service providers combined, compared to Akamai which only has 1044 BGP Peers.  More BGP peers are important in shortening the path, providing multiple paths, bypassing slow or expensive transit providers, and improved performance through network health and visibility.

* EXAMPLECOM Distributed cloud has 31 physical data center locations known as "Regional Edge's", or point of presence, and are located in every major region around the world, all colocated in Equinex Metal. Akamai takes a different approach, rather than leveraging BGP peers, they currently have 4,100 physical locations, otherwise known as PoPs (Points of Presence). Where EXAMPLECOM Distributed Cloud has taken the approach of using BGP to build the most robust cloud service provider network, Akamai's business is focused on building real estate with their massive number of PoPs.

* All additional software subscriptions features such as Web App and API protections, containerized workloads distribution, intelligent DNS etc. are built natively into the EXAMPLECOM Distributed Cloud platform, whereas Akamai has acquired many different products that operate independently each with their own account management, administration interface and disconnected managemnt API's. The EXAMPLECOM Distributed Cloud Bot Defense, which provides security to protect a website from bots, fake users, and unauthorized transactions, is a service that is also made available through competitors product such as AWS CloudFront, [Cloudflare](https://www.youtube.com/watch?v=eg9jke6uOLE), our [BIG-IP](https://www.youtube.com/watch?v=JD43GNFKtpU) product line, or other competitors products. EXAMPLECOM Distributed Cloud provides a single pane of glass UI and API management, unified RBAC across all features, and a consistent feature set across all Regional Edges.

### EXAMPLECOM Distributed Cloud

* 31 PoPs (Points of Presence)
* [5,445 BGP Peers](https://bgp.he.net/report/peers)
* Bot Defense

### Akamai

* 4,100 PoPs (Points of Presence)
* 1,044 BGP Peers
* Bot Manager
* Linode
* Kona
* Edge DNS
* Prolexic
* API Security
* APP & API Protector
* Acount Protector
* Cloud Firewall

### Ease of Use

![EXAMPLECOM Distributed Cloud Bot Defense Gartner Peer Review](./images/gartner-peer-report.png)

* EXAMPLECOM Distributed Cloud Bot Defense scores higher in Gartner Peer reviews, mostly because of the ease of use, since all of the UI and API management is a single consolidated interface.

## [EXAMPLECOM Distributed Cloud Bot Defense](https://www.youtube.com/watch?v=qofQozTpqo4)

![EXAMPLECOM Distributed Cloud Bot Defense Infographic ](./images/f5-distributed-cloud-bot-defense-infographic.png)

* EXAMPLECOM Distributed Cloud Bot Defense is an anti-automation solution that employs JavaScript and API calls for telemetry collection. Both Akamai and EXAMPLECOM offer leading bot protection features, including defenses against credential stuffing, fake accounts, fraud, application layer DDoS, and financial aggregator threats.

* Commonly used mitigations to combat credential stuffing, including CAPTCHA and multi-factor authentication (MFA), are easily bypassed by sophisticated attackers and can frustrate real customers, leading to abandoned transactions and lost revenue. Additionally, credential stuffing attacks are often an early indicator that there will be other more sophisticated attacks launched.

1. Enable Bot Defense

![EXAMPLECOM Distributed Cloud Bot Defense Enable Bot Defense](./images/bot-protection-enable.png)

* After logging into the EXAMPLECOM Distributed Cloud console and enabling Advanced Bot Defense, you'll find the security features integrated within the HTTP load balancer, eliminating the need for an additional portal and offering a unified, cloud-native platform experience.

2. Create Bot Policy

![EXAMPLECOM Distributed Cloud Bot Defense Create Bot Policy](./images/create-policy.png)

* Create an App endpoint

* Specify the method to POST on both protocol on any domains, and for Path matching we can do prefix, regex or exact path, and for the actions you want to change it from Flag to Block.

* So you can do things like enable carding against a payment page and credential stuffing against other pages.

* From there we can specify how we want to inject the Javascript, which usually after the HEAD tag, but it can be in a script or after the title tag.

* It's best practice to activate Bot Defense on sensitive URLs, like login forms, using regex to detect patterns in these URLs.

3. Bot Defense Reporting

![EXAMPLECOM Distributed Cloud Bot Defense Create Bot Policy](./images/bot-defense-reporting.png)

* After applying the Bot Policy, launch a simulated attack using a testing tool such as Selenium, and then view the analytics in the EXAMPLECOM Distributed Cloud portal.

## Deployment Options

![Deployment Options](./images/single-cdn-akamai.png)

* Currently the ACME Corp website is using Akamai, which then load-balances to origin servers that are running in a VPC. The origin servers that are located in AWS are connected with a low-latency DirectConnect, to consume the database services running on prem.

* When implementing a significant change there needs to be care taken into consideration when planning out an implementation. Currently the ACME Corp website has a static DNS record which resolves to an Akamai anycast IP address. The challenge is, "How is it possible to introduce EXAMPLECOM Distributed Cloud without making any disruptive changes that might cause downtime".

1. Multi-CDN

![Multi-CDN](./images/multi-cdn.png)

* To seamlessly integrate an additional A record, an intelligent DNS service with Global Server Load Balancing (GSLB) is essential. This approach allows the ACME Corp website to utilize multiple CDN services by incorporating GSLB into its DNS. GSLB can be configured for various strategies such as active-standby, geographic-based resolution, or health check-based decisions to manage issues with a primary CDN. Implementing GSLB for ACME Corp's DNS resolution enables the concurrent use of both Akamai and EXAMPLECOM Distributed Cloud CDNs.

2. Regional Edge Campus Area Private Network

![Campus Area Private Network](./images/campus-area-networking.png)

* A distinctive feature of the EXAMPLECOM Distributed Cloud platform, not offered by Akamai, is its ability to advertise services on the same private Network As a Service providers through the EXAMPLECOM Distributed Cloud Regional Edges. This enables the EXAMPLECOM Distributed Cloud's IP anycast services, accessible on the internet, to be identical to those advertised on internal, campus-type networks.

3. AppStack in Virtual Private Cloud

![appstack](./images/appstack-vpc.png)

* The EXAMPLECOM Distributed Cloud software, operational in Equinix Regional Edge locations, can be deployed as a virtual machine into your VPCs, removing the necessity for intricate transit gateways and costly, complex firewall virtual machines. Appstack instances establish redundant encrypted tunnels with EXAMPLECOM Distributed Cloud Regional Edges, eliminating the need for VPCs to expose public IP addresses for NATting to origin servers.

* IP Overlap is often a challenge: With EXAMPLECOM Distributed Cloud Appstack proxies, we can service all the Masqueriding and NAT requirements.

4. Appstack Managed Kubernetes

![AppStack Managed Kubernetes](./images/appstack-managed-kubernetes.png)

* An EXAMPLECOM Distributed Cloud instance can be deployed as a managed Kubernetes platform on both virtual machines and bare metal. Appstack-managed Kubernetes can utilize high-performance GPUs in public clouds or on-premises hardware in remote or retail locations. This enables computationally intensive containerized workloads to leverage GPUs, supporting the increasing trend of organizations deploying GPUs for private AI services running open-source Large Language Models (LLMs).

* The EXAMPLECOM Distributed Cloud Appstack Managed Kubernetes can span multiple physical or virtual locations, with EXAMPLECOM managing the Kubernetes stack. Local Kubernetes administration stays consistent, allowing administrators to export a kubectl file. This ensures DevOps teams' interaction with managed Kubernetes and their existing workflows remain unchanged, provided they have the kubectl authentication file.

## Shift Left Security

![Shift Left Security](./images/shift-left-security.png)

* Shift Left is a strategy aimed at identifying and mitigating defects early in the software delivery cycle by shifting tasks earlier in the lifecycle to enhance quality. This approach encourages early testing and supports the adoption of DevOps practices.

### GitOps SDLC

![GitOps SDLC](./images/SDLC.png)

* A GitOps workflow with shift-left security automates security integration early in the development lifecycle by treating infrastructure and app configurations as code in Git. This approach facilitates collaboration among developers by enabling the creation of multiple namespaces, often used for departmental resource separation or throughout the development process. For instance, when a developer initiates a new feature branch in Git, automation can generate a corresponding namespace. This allows CI/CD testing to occur within this development namespace. Upon pull request approval, the automation will remove both the Git development branch and its associated namespace in EXAMPLECOM Distributed Cloud.

### Infrastructure as Code

![Infrastructure as Code](./images/terraform-provider.png)

* The EXAMPLECOM Distributed Cloud platform supports automation via the REST API with RBAC-enforced token authentication, allowing for integration into existing CI/CD pipelines. Official EXAMPLECOM GitHub repositories provide Terraform examples for infrastructure as code.

### CLI vesctl

* The [vesctl](https://gitlab.com/volterra.io/vesctl/blob/main/README.md) tool is a configuration command line utility that allows users to create, debug and diagnose EXAMPLECOM Distributed Cloud Services configuration. It is modelled after the EXAMPLECOM Distributed Cloud API. All EXAMPLECOM Distributed Cloud commands are available via vesctl.

## References

* https://docs.cloud.f5.com/docs/how-to/advanced-security/bot-defense

* https://docs.cloud.f5.com/docs-v2/bot-defense/how-tos/configure-bot-defense

* https://docs.cloud.f5.com/docs/quick-start/bot-defense-quick-start

* https://docs.cloud.f5.com/docs/
# F5 Distributed Cloud

## Credential Stuffing Attacks

Robin Mordasiewicz, a Sales Engineer at F5, will conduct a 30-minute presentation on the F5 Distributed Cloud product. The intended audience is Robert Loblaw, the IT Manager at ACME Corp.

## Background

* In a previous meeting, Robert Loblaw, the IT Manager at ACME Corp, met with Robin Mordasiewicz, a Sales Engineer from F5 who specializes in the F5 Distributed Cloud product. During this meeting, Robert, who oversees the maintenance of the ACME Corp website (https://www.acmecorp.com), informed Robin about a security audit that uncovered an ongoing credential stuffing attack on their site. This attack is causing significant revenue loss and damage to their reputation.

* Robert also shared with Robin that ACME Corp's website currently utilizes the Akamai Content Delivery Network (CDN), complemented by a subscription to the Akamai Web Application Firewall (WAF) product known as Kona. However, Robert discovered that the Akamai Kona WAF does not offer protection against credential stuffing attacks. To counter such attacks, an additional subscription to the Akamai Bot Manager product is necessary. Additionally, Robert mentioned that the Akamai CDN distributes traffic to origin servers hosted on AWS. These AWS-hosted origin servers, which serve the website's content, are also linked to an on-premises data center via DirectConnect for database access. Looking ahead, there are plans to expand the ACME Corp website's infrastructure to operate on both AWS and Azure platforms.

* Robert has invited Robin to introduce a competitive Bot Protection product from F5 Distributed Cloud, hoping it offers more comprehensive features and is more user-friendly than their current solution. He has requested Robin to showcase the Bot Protection capabilities of the F5 Distributed Cloud, along with any additional value-added features that could aid in modernizing the ACME Corp website, particularly in the area of multi-cloud networking.

* The following is the content of an F5 Distributed Cloud presentation, prepared by Robin, that focuses on credential stuffing attacks. This presentation will be delivered to Robert.

## Introduction

* Robin Mordasiewicz, a Sales Engineer at F5, is responsible for showcasing and selling F5 Distributed Cloud solutions to potential clients. One such client is Robert Loblaw, an IT Manager at ACME Corp Solutions, who oversees the maintenance of the ACME Corp website (https://www.acmecorp.com). Robin will present the following content to Robert.

## F5 Platform Overview

![F5 Platform](./images/f5-distributed-cloud-diagram.png)

F5 Distributed Cloud is one of the largest most advanced cloud service provider (CSP). The F5 Distributed Cloud is a CDN service that provides multi-cloud networking, high performance network DDoS, WebApp and API protections, Advanced Bot Protection, containerized workload management, and is able to connect to all the major Network as a Service providers, packet Fabric, Megaport. F5 Distributed Cloud is also able to provide the same features and functionality not only to internet facing clients, but can also connect to internal only networks, while participating with internal BGP routers so that the same load-balancing that is available externally, can also be configured on internal corporate networks that are interconnected with a Network as a Service provider such as megaport or packetfabric. Furthermore, the F5 Distributed Cloud software stack can be deployed directly into private workload locations such as an Amazon VPC (AWS VPC), or within an on-premis private data center which may also eliminate the need for locally managed load balancers, or firewalls. The Appstack version of F5 Distributed Cloud can be deployed as a virtual machine, or onto bare metal. The Appstack version of F5 Distributed Cloud runs the same software stack that runs on the F5 Regional Edges that are hosted in Equinex, but Appstack can also be configured to run as a managed Kubernetes platform which may be given direct access to high performance hardware GPU's for running computationally intensive workloads in remote locations or retail space for example.

Cloud providers Emphasize connectivity over security, at F5 we have a pedigree in security software.

## F5 Distributed Cloud versus Akamai

* F5 Distributed Cloud and Akamai are competitors in CDN technology as well as advanced edge security, and distributed computing. F5 Distributed Cloud has 5445 BGP peers which is more than the other cloud service providers combined, compared to Akamai which only has 1044 BGP Peers.  More BGP peers are important in shortening the path, providing multiple paths, bypassing slow or expensive transit providers, and improved performance through network health and visibility.

* F5 Distributed cloud has 31 physical data center locations known as "Regional Edge's", or point of presence, and are located in every major region around the world, all colocated in Equinex Metal. Akamai takes a different approach, rather than leveraging BGP peers, they currently have 4,100 physical locations, otherwise known as PoPs (Points of Presence). Where F5 Distributed Cloud has taken the approach of using BGP to build the most robust cloud service provider network, Akamai's business is focused on building real estate with their massive number of PoPs.

* All additional software subscriptions features such as Web App and API protections, containerized workloads distribution, intelligent DNS etc. are built natively into the F5 Distributed Cloudplatform, whereas Akamai has acquired many different products that operate independantly each with their own account management, administration interface and disconnected managemnt API's. The F5 Distributed Cloud Bot Defense, which provides security to protect a website from bots, fake users, and unauthorized transactions, is a service that is also made available through competitors product such as AWS CloudFront, [Cloudflare](https://www.youtube.com/watch?v=eg9jke6uOLE), our BIG-IP product line, or other competitors products. F5 Distributed Cloud provides a single pane of glass UI and API management, unified RBAC across all features, and a consistent feature set across all Regional Edges.

### F5 Distributed Cloud

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

## F5 Distributed Cloud Bot Defense

![F5 Distributed Cloud Bot Defense Infographic ](./images/f5-distributed-cloud-bot-defense-infographic.png)

F5 Distributed Cloud Bot Defense is an anti automation product which uses JavaScript and API calls to collect telemetry. Both Akamai and F5 have competetive industry leading Bot Protection features including credential stuffing attack, fake account, fraud, application layer DDoS, and financial aggregator protection.

### Ease of Use

![F5 Distributed Cloud Bot Defense Gartner Peer Review](./images/gartner-peer-report.png)

F5 Distributed Cloud Bot Defense scores higher in Gartner Peer reviews, mostly becuase of the ease of use, since all of the UI and API management is a single consolidated interface.

1. Enable Bot Defense

![F5 Distributed Cloud Bot Defense Enable Bot Defense](./images/bot-protection-enable.png)

After logging in to the F5 Distributed Cloud console, and enabling Advanced Bot Defense, you will find the security features natively integrated into the HTTP load balancer. There is no additional portal to log into, everything is integrated into a single consolidated cloud native platform.

2. Create Bot Policy

![F5 Distributed Cloud Bot Defense Create Bot Policy](./images/create-policy.png)

It's a best practice to enable Bot Defense on sensitive URL's such as a login form, but you can use regex to identify patterns in sensitive URLs

3. Bot Defense Reporting

![F5 Distributed Cloud Bot Defense Create Bot Policy](./images/bot-defense-reporting.png)

After applying the Bot Policy, launch a simulated attack using a testing tool such as Selenium, and then view the analytics in the F5 Distributed Cloud portal.

## Deployment Options

![Deployment Options](./images/single-cdn-akamai.png)

  * Currently the ACME Corp website is using Akamai, which then load-balances to origin servers that are running in a VPC. The origin servers that are located in AWS are coneted with a low-latency DirectConnect, to consume the database services running on prem.

  * When implementing a significant change there needs to be care taken into consideration when planning out an implementation. Currently the ACME Corp website has a static DNS record which resolves to an Akamai anycast IP address. The challenge is, "How is it possible to introduce F5 Distributed Cloud without making any disruptive changes that might cause downtime".

1. Multi-CDN Networking

![Multi-CDN](./images/multi-cdn.png)

The answer is to use an intelligent DNS service which provides GSLB load balancing balancing so that we can safely introduce an additional A record into the DNS. By leveraging GSLB functionality into the DNS for the ACME Corp website, it will make it possible to use multiple CDN services. Different GSLB algorithms can be configured to provide active-standby, geographically based DNS resolving decisions, or making DNS resolver decisions based on health checks, which might detect outages or problems with a primary CDN. Introducing GSLB to the internet facing DNS resolution for ACME Corp website will make it so that both the Akamai CDN and the F5 Distributed Cloud CDN are possible

2. Multi-Cloud Networking

![multi-cloud-networking](./images/multi-cloud-networking.png)

A unique feature of the F5 Distributed Cloud platform which is not available from Akamai, is that the F5 Distributed Cloud Regional Edges can be configured to advertise services on the same private Network As a Service providers. This means that the F5 Distributed Cloud IP anycast services that are available on the internet, are also the exact same services that can be advertised to internal only campus area type of networks.

3. AppStack in Virtual Private Cloud

![appstack](./images/appstack-vpc.png)

The F5 Distributed Cloud software that runs in the Equinex Regional Edge locations, can be deployed as a virtual machine into your VPC's, which can eliminate the need for complex transit gateways, expensive and complex firewall virtual machines. The Appstack instances form redundant encrypted tunnels with the F5 Distributed Cloud Regional Edges bypassing the requirement to have public IP addresses into the AWS VPS.

4. Appstack Managed Kubernetes

![AppStack Managed Kubernetes](./images/appstack-vpc.png)

An F5 Distributed Cloud instance can also be deployed as a managed kubernetes platform either as a virtual machine or onto bare metal. Appstack managed kubernetes is able to leverage high performance GPU in public cloud, or even when its deployed into hardware in remote locations or retail space. Computationally intensive containerized workloads running in Appstack managed kubernetes can leverage GPU's. One example is that many organizations are deploying privately available AI service which are running open source LLM's.

## Shift Left Security

![Shift Left Security](./images/shift-left-security.png)

Shift Left is a practice intended to find and prevent defects early in the software delivery process. The idea is to improve quality by moving tasks to the left as early in the lifecycle as possible. Shift Left testing means testing earlier in the software development process, and this lends itself to adopting DevOps practices

###  

## References

* https://docs.cloud.f5.com/docs/how-to/advanced-security/bot-defense#connectors

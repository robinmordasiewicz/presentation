# Protecting against credential stuffing attacks using F5 Distributed Cloud presentation

This is a 30 minute presentation delivered by F5 employee Robin Mordasiewicz with job title Sales Engineer, which specializes in the F5 Distributed Cloud product. The audience is the ACME Corp employee Robert Loblaw whose job title is "IT Manager".

## Background

In a previous meeting the ACME Corp employee with the job title "IT Manager", Robert Loblaw, who is responsible for maintaining the ACME Corp website https://www.acmecorp.com, met with the F5 employee Robin Mordasiewicz who's job title is Sales Engineer and is repsonsible for selling the F5 Distributed Cloud product.. During the meeting Robert explained to Robin that a security audit of the ACME Corp website https://www.acmecorp.com revealed that the website is currently experiencing a credential stuffing attack. Robert also explained to Robin that the current architecture of the ACME Corp website is using the Akamai Content Delivery Network (CDN), with the additional subscription of the Akamai Web Application Firewall (WAF) product named Kona. Robert has learned that the Akamai Kona product does not protect against credential stuffing attacks, and that in order for Akamai to prevent credential stuffing attacks, Robert would need the purchase of an addition product subscription named Akamai Bot Manager. Robert has invited Robin to present a competetive offering from F5 Distributed Cloud in the hopes that the F5 Distributed Cloud product is more fully featured. Furthermore, Robert explained that the Akamai CDN load balances to origin servers that are hosted in AWS, and the origin servers hosting the website content are also connected to an on premisis datacenter using DirectConnect for database access, and that future plans to be considered are that the ACME Corp website will also expand to be running in both AWS and Azure.

## F5 Distributed Cloud versus Akamai

F5 Distributed Cloud and Akamai are competitors in CDN technology as well as advanced edge security, and distributed computing. F5 Distributed Cloud is ostenisbly one of the largest service providers on the planet with more BGP peers (5,445) than the other cloud service providers combined. More BGP peers are important in shortening the path, providing multiple paths, bypassing slow or expensive transit providers, and improved performance through network health and visibility. F5 Distributed cloud has 31 PoPs which are located in every major region around the world, which are all colocated in Equinex Metal locations. Akamai takes a different approach, rather than leveraging BGP peers, they have built 4,100 PoPs (Points of Presence). Where F5 Distributed Cloud has taken the approach of using BGP to build the most robust cloud service provider network, Akamai's business is focused on building real estate.

With F5 Distributed Cloud all additional software subscriptions features such as Web App and API protections, containerized workloads distribution, intelligent DNS etc. are built natively into the platform, whereas Akamai has acquired many different products that operate independantly each with their own account management, administration interface and disconnected managemnt API's. The only exception is that the F5 Distributed Cloud Bot Defense, which provides security to protect a website from bots, fake users, and unauthorized transactions, is a service that is made available through competitors product such as AWS CloudFront, [Cloudflare](https://www.youtube.com/watch?v=eg9jke6uOLE), our BIG-IP product line, or other competitors products. F5 Distributed Cloud provides a single pane of glass UI and API management, unified RBAC across all features, and a consistent feature set across all Regional Edges.

### F5 Distributed Cloud

31 PoPs (Points of Presence)
5,445 BGP Peers - https://bgp.he.net/report/peers
Bot Defense

### Akamai

4,100 PoPs (Points of Presence)
1,044 BGP Peers
Bot Manager
Linode
Kona
Edge DNS
Prolexic
API Security
APP & API Protector
Acount Protector
Cloud Firewall

## F5 Distributed Cloud Bot Defense

![F5 Distributed Cloud Bot Defense Infographic ](./images/f5-distributed-cloud-bot-defense-infographic.png)

F5 Distributed Cloud Bot Defense is an anti automation product which uses JavaScript and API calls to collect telemetry. Both Akamai and F5 have competetive industry leading Bot Protection features including credential stuffing attack, fake account, fraud, application layer DDoS, and financial aggregator protection.

### Ease of Use

![F5 Distributed Cloud Bot Dense Gartner Peer Review](./images/gartner-peer-report.png)

F5 Distributed Cloud Bot Defense scores higher in Gartner Peer reviews, mostly becuase of the ease of use, since all of the UI and API management is a single consolidated interface.

### Enabling Bot Defense Workflow

![
After logging in to the F5 Distributed Cloud console, and enabling Advanced Bot Defense, you will find the security features natively integrated into the HTTP load balancer. There is no additional portal to log into, everything is integrated into a single consolidated cloud native platform.

It's a best practice to enable Bot Defense on sensitive URL's such as a login form, but you can use regex to identify patterns in sensitive URLs

### Results

After everything is configured, you will want to launch attacks using a testing tool such as Selenium, and then view the analytics in the F5 Distributed Cloud portal.


F5 Bot Defense
 - deploy VIP
 - configure policy
MCN
  -  The ideal service would provide a low-latency connection, with adequate throughput, to consume the storage service. This would include using services like DirectConnect for AWS, ExpressRoute for Azure, and Cloud Interconnect for GCP.
Private link
  -
AppAstack - branch/retail


Multi-CDN
Terraform
CICD

Cloud providers Emphasizie connectivity over security


* https://docs.cloud.f5.com/docs/how-to/advanced-security/bot-defense#connectors

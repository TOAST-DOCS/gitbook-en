## Network > Direct Connect > Overview

Direct Connect serves as a point of contact that connects NHN Cloud’s IaaS resources and external networks (e.g., on-premises networks of the customer) with a dedicated line provided by mobile carriers. Using a dedicated line offers more reliable speed and secure communication against external security environments.

## Main Features
Direct Connect provides various features as follows.
> [Note] This service is currently only available in the Korea (Pangyo) and Korea (Pyeongchon) regions, and will be supported by other regions gradually.
* Various speeds: Provides bandwidths ranging from a minimum of 10Mbps to 10Gbps.
* Redundancy support: Supports redundancy of a point of contact for a dedicated line.
* Excellent security: Provides excellent security at the same level with the relevant data center, when connecting to a dedicated line through various security certifications and technologies achieved by NHN Cloud.
* Neutral data center: Allows customers to use a mobile carrier’s line of their choice.
* Various communication settings: Supports various communication protocols such as L2, L3-based VLAN, and BGP.

## Configuration Environment 
The cloud configuration environment supported by Direct Connect is as follows.

| Category | Specifications |
| --- | --- |
| Region | Korea (Pangyo), Korea (Pyeongchon) regions |
| Bandwidth | 10Mbps~10Gbps |
| Line type | Ethernet method |
| Communication method | L2 (Vlan), L3 (BGP, Static, IPsec) |
| Connection method 1 | Dedicated connection - Dedicated line connection through mobile carriers<br>- Choose from KT, LG U+, SK Broadband, Dreamline, Sejong Telecom (line contract and connection by NHN Cloud) |
| Connection method 2 | Hosted connection- Cloud platform connection method through N/W partners<br>- [KINX Cloud Hub](https://www.kinx.net/service/cloudhub/)<br>- [LG U+ Cloud Multi-Connect](https://www.lguplus.com/biz/all/telecom/idc/cloud-connection-service/B000000036)<br>- [Dreamline Cloud Exchange Platform](https://www.dreamline.co.kr/service/cloud_overview.php)

> [Note] *Dedicated connection is a physical connection between the Direct Connect network port within the NHN Cloud location and a user’s network port. NHN Cloud secures and provides a dedicated line from the line provider of your choice.

> [Note] **Hosted connection is a logical (VLAN) connection that you provision through the network environment of a partner providing Direct Connect. Customers can directly apply for the N/W partner's cloud platform.
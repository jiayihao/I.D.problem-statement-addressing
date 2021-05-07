---
coding: utf-8

title: "Challenging Scenarios and Problems in Internet Addressing"
abbrev: "Scenarios and Problems in Addressing"
docname: draft-jia-intarea-scenarios-problems-addressing-00
category: info
area: Internet
workgroup: Internet Area Working Group
keyword: Internet-Draft

ipr: trust200902
date: {DATE}
stand_alone: yes
pi: [toc, sortrefs, symrefs, docmapping]


author:
-
  ins: Y. Jia
  name: Yihao Jia
  org: Huawei Technologies Co., Ltd
  abbrev: Huawei
  # role: editor
  street: 156 Beiqing Rd.
  city: Beijing
  country: P.R. China
  code: '100095'
  email: jiayihao@huawei.com
-
  ins: D. Trossen
  name: Dirk Trossen
  org: Huawei Technologies Duesseldorf GmbH
  abbrev: Huawei
  # role: editor
  street: Riesstr. 25C
  city: Munich
  country: Germany
  code: '80992'
  email: dirk.trossen@huawei.com
-
  ins: L. Iannone
  name: Luigi Iannone
  org: Huawei Technologies France S.A.S.U.
  abbrev: Huawei
  # role: editor
  street: 18, Quai du Point du Jour
  city: Boulogne-Billancourt
  country: France
  code: '92100'
  email: luigi.iannone@huawei.com
-
  ins: D. Eastlake 3rd
  name: Donald E. Eastlake 3rd
  org: Futurewei Technologies
  abbrev: Futurewei
  # role: editor
  street: 2386 Panoramic Circle
  city: Apopka, FL
  country: United States of America
  code: '32703'
  email: d3e3e3@gmail.com
-
  ins: P. Liu
  name: Peng Liu
  org: China Mobile
  abbrev: China Mobile
  # role: editor
  street: 32 Xuanwumen West Ave
  city: Xicheng, Beijing
  country: P.R. China
  code: '100053'
  email: liupengyjy@chinamobile.com


normative:
  # RFCxxxx: if we cite as {{!RFCxxxx}} (rather than {{RFCxxxx}}), then we do not need to declare it here :D

informative:
  # RFCxxxx: if we cite as {{?RFCxxxx}} (rather than {{RFCxxxx}}), then we do not need to declare it here :D
  
  I-D.ietf-lisp-nexagon:
  I-D.ietf-lisp-introduction:
  I-D.ietf-lisp-mn:
  I-D.ietf-intarea-gue:
  # DYNCAST: I-D.liu-dyncast-ps-usecases
  # (I don't know why it is not archived/tracked by datatracker.ietf.org)
  DYNCAST: I-D.geng-rtgwg-cfn-dyncast-ps-usecase
  QUIC: I-D.ietf-quic-transport
  ICN5G: I-D.irtf-icnrg-5gc-icn
  ICNIP: I-D.trossen-icnrg-internet-icn-5glan
  BIER-MC: I-D.ietf-bier-multicast-http-response
  
  ANYCAST: DOI.10.1145/3230543.3230547
  ADDRLESS: DOI.10.1371/journal.pone.0246293
  MANET1: DOI.10.1177/1550147716671255
  CCN: DOI.10.1145/1658939.1658941
  HANDLEY: DOI.10.1145/3286062.3286075
  TROSSEN: DOI.10.1145/1764873.1764878
  REED: DOI.10.1109/ICC.2016.7511036
  SPHINX: DOI.10.1109/SP.2009.15
  ALOHA: DOI.10.1145/205447.205451
  CARTISEAN: DOI.10.1007/978-3-540-39611-6_27

  LR-WPAN:
    title: "IEEE 802.15.4 - IEEE Standard for Low-Rate Wireless Networks"
    date: 2020-05
    seriesinfo:
      IEEE: 802.15 WPAN Task Group 4
    target: https://standards.ieee.org/standard/802_15_4-2020.html
  DECT-ULE:
    title: "Digital Enhanced Cordless Telecommunications (DECT); Common Interface (CI); Part 1: Overview"
    date: 2009-05
    seriesinfo:
      ETSI: European Standard, EN 300 175-1, V2.6.1
    target: https://www.etsi.org/deliver/etsi_en/300100_300199/30017501/02.06.01_60/en_30017501v020601p.pdf
  BACnet:
    title: "BACnet-A Data Communication Protocol for Building Automation and Control Networks"
    date: 2016-01
    seriesinfo:
      ANSI/ASHRAE: Standard 135-2016
    target: https://www.techstreet.com/ashrae/standards/ashrae-135-2016?product_id=1918140
  ECMA-340:
    title: "Near Field Communication - Interface and Protocol (NFCIP-1) 3rd Ed."
    date: 2013-06
    author:
      org: EECMA-340
  IEEE_1901.1:
    title: "Standard for Medium Frequency (less than 15 MHz) Power Line Communications for Smart Grid Applications"
    date: 2018-05
    seriesinfo:
      IEEE 1901.1: IEEE-SA Standards Board
    target: https://ieeexplore.ieee.org/document/8360785
  BLE:
    title: Bluetooth Specification
    seriesinfo:
      Bluetooth: SIG Working Groups
    target: https://www.bluetooth.com/specifications
  OCADO:
    title: Ocado Technology’s robot warehouse a Hive of IoT innovation
    target: https://techmonitor.ai/tech-leaders/ocado-technology-robot-hive-innovation
  TERASTREAM:
    title: Deutsche Telekom tests TeraStream, the network of the future, in Croatia
    target: https://www.telekom.com/en/media/media-information/archive/deutsche-telekom-tests-terastream-the-network-of-the-future-in-croatia-358444
  PEARG:
    title: Privacy Enhancements and Assessments Research Group - PEARG
    target: https://irtf.org/pearg
  DETNET:
    title: Deterministic Networking (DetNet)
    target: https://datatracker.ietf.org/wg/detnet/about/
  ETSI-NIN:
    title: Non-IP Networking - NIN
    author:
      org: ETSI - European Telecommunication Standards Institute
    target: https://www.etsi.org/technologies/non-ip-networking
  TOR:
    title: The Tor Project
    target: https://www.torproject.org/
  HICN:
    title: "Hybrid Information-Centric Networking: ICN inside the Internet Protocol"
    author: 
      ins: L. Muscariello
    target: https://datatracker.ietf.org/meeting/interim-2018-icnrg-01/materials/slides-interim-2018-icnrg-01-sessa-hybrid-icn-hicn-luca-muscariello
    date: 2018-03

--- abstract

<!-- 
NOTES: keep title since it is fitting [DONE]
NOTES: replace any wording that suggests a solution, like 'flexible addressing' or the last sentences in each use case, with more 'capability' type of language. [DONE]
NOTES: replace all 'use cases' with 'scenarios' [DONE]
AP Dirk: Do the above
-->

The Internet Protocol (IP) has been the major technological success in information technology of the last half century. As Internet become pervasive, IP start replacing communication technology for domain-specific solutions. However, domains with specific requirements as well as communication behaviors and semantics still exists and represent what {{?RFC8799}} recognizes as "limited domains". When communicating within limited domains, the address semantic and format may differ with respect to the IP address one. As such, there is a need to adapt the domain-specific addressing to the Internet addressing paradigm. In certain scenarios, such adaptation may raise challenges.

This document describes well-recognized scenarios that showcase possibly different addressing requirements which are challenging to be accommodated in the IP addressing model. These scenarios highlight issues related to the Internet addressing model and call for starting a discussion on a way to re-think/evolve the addressing model so to better accommodate different domain-specific requirements. 

--- middle


# Introduction {#SEC:intro}

<!-- Yihao: Some check points to confirm
- Position: problematic scenarios for IP adaption/dressing?
- avoiding: terms directly/indirectly related to "flexible", e.g., flexible address structure, flexible addressing.
- better to have a clear text about the relationship of "limited domain" and "scenarios" (like these scenarios can usually be categoried as limited domains)
AP Dirk: look again [the second paragraph below links limited domain to scenarios and the exhibited requirements and behaviours defined through them]
-->

The Internet Protocol (IP), positioned as the unified protocol at the (Internet) network layer, is seen by many as key to the innovation stemming from Internet-based applications and services. Even more so, with the success of TCP/IP protocol stack, IP has been gradually replacing existing domain-specific protocols, evolving into the core protocol of the entire communication system. At its inception roughly 40 years ago {{!RFC0791}}, the Internet's addressing system, represented in the form of the IP address and its locator-based semantics, has brought the notion of a 'common addressing for all communication'. Compared to proprietary technology-specific solutions, such 'common addressing for all communication' advance ensures end-to-end communication from any device connected to the Internet to another.

However, scenarios, associated service, node behaviors, and requirements on packet delivery have since been significantly extended, with Internet technologies being developed to accommodate them in the framework of addressing that stood at the beginning of the Internet's development. This evolution is reflected in the concept of the "Limited domain", first introduced in {{?RFC8799}}. It refers to a single physical network, attached to or running in parallel with the Internet, or is defined by set of users and nodes distributed over a much wider area, but drawn together by a single virtual network over the Internet. Key to a limited domain is that requirements, behaviors, and semantics could be noticeable local and, more importantly, specific to the limited domain. Very often, the realization of a limited domain is defined by specific communication scenario(s) that exhibit the domain-specific behaviors and pose the requirements that lead to the establishment of the limited domain.

One key architectural aspect, when communicating within limited domains, is that of addressing and, therefore, the address structure, as well as the semantic that is being used for the routing of packets. The topological location centrality of IP is fundamental when reconciling the often differing semantics for 'addressing' that can be found in those limited domains. The result of this fundamental role of the single IP addressing is that limited domains have to adopt specific solutions, e.g., translating/mapping/converting concepts, semantics, and ultimately, domain-specific addressing, into the common IP addressing used across limited domains.

This document advocates the flexibility in addressing in order to accommodate limited domain specific semantics, while, if possible, ensuring a single holistic addressing scheme able to reduce, or even entirely remove, the need for aligning the address semantics of different limited domains, such as the current topological location semantic of the Internet. Ultimately, such holistic addressing could be beneficial to those communication scenarios realized within limited domains by improving efficiency, removing of constraints imposed by needing to utilize the limited semantics of IP addressing, and/or in other ways.

In other words, this document revolves around the following question:

> "Should limited domains purely rely on IP addresses and therefore deal with the complexity of translating any semantic mismatch themselves, or should flexibility for supporting those limited domains be a key focus for an evolved Internet addressing?"

To that end, this document describes well-recognized scenarios in limited domains that could benefit from a greater flexibility in addressing and analyses problems encountered throughout these scenarios due to the lack of that flexibility. The purpose of this draft is thus to stimulate discussion on the emerging needs for addressing at large with the possibility to fundamentally re-think the addressing in the Internet beyond the current objectives of IPv6.

<!-- LUIGI: Tentative paragraph to related to the RRG effort == PLEASE REVIEW == -->
It is important to remark that any change in the addressing, hence at the data plane level, leads to changes and challenges on the control plane level, i.e., routing. The latter is an even harder problem than just addressing and might need more research efforts that are beyond the objective of this document, which focuses solely on the data plane.



<!-- BACKUP

# Conventional Terminology {#SEC:term}
The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in BCP 14 RFC2119 RFC8174 when, and only when, they appear in all capitals, as shown here.

-->




# Communication Scenarios in Limited Domains {#SEC:cases}


The following sub-section outlines a number of scenarios, all of which belong to the concept of "limited domains" {{?RFC8799}}. While a list of scenarios may be long, this document focuses on scenarios with a number of aspects that we observe in those limited domains, captured in the sub-section titles. For each scenarios, we point at possible challenges, which we will pick upon in {{SEC:problem}} when describing more formally the issues existing in current Internet addressing.


## Communication in Constrained Environments {#SEC:constrained}

In a number of communication scenarios, such as those encountered in the Internet of Things (IoT),
a simple, low-cost communication network is required, and there are limitations for network devices in computational power, memory, and energy availability.
In addition to IEEE 802.15.4, i.e., Low-Rate Wireless Personal Area Network {{LR-WPAN}}, several limited domains exists through utilizing link layer technologies such as Bluetooth Low Energy (BLE) {{BLE}}, Digital European Cordless Telecommunications (DECT) - Ultra Low Energy (ULE) {{DECT-ULE}}, Master-Slave/Token-Passing (MS/TP) {{BACnet}}, Near-Field-Communication (NFC) {{ECMA-340}}, and Power Line Communication (PLC) {{IEEE_1901.1}}.
Generally, a group of IoT network devices form a constrained node network at the edge, and IoT terminals connect to these network devices for data transmission.
This type of networks and IoT devices in the network require as little computational power as possible, smaller memory requirements, better energy availability to reduce the total cost of ownership of the network.
Furthermore, in the context of industrial IoT, real-time requirements and scalability make IP technology not naturally suitable as communication technology ({{OCADO}}).


The end-to-end principle (detailed in {{?RFC2775}}) requires Internet protocols (e.g., IPv6 {{?RFC8200}}) to run on such constrained node networks, allowing IoT devices using multiple communication technologies to talk on the Internet.
Often, devices located on the edge of constrained networks act as gateway devices, usually performing header compression ({{?RFC4919}}).
To ensure security and reliability, multiple gateways must be deployed. IoT devices on the network can easily select one of gateways for traffic passthrough by the devices on the (limited domain) network.


Given the constraints imposed on the computational and possibly also communication technology, the usage of a single addressing semantic in the form of a 128-bit endpoint identifier, i.e., IPv6 address, may pose a challenge when operating such networks.

<!-- NOTES: Dirk
Can we add any references here that evaluated those overheads? [Yihao] the overhead of what?
-> do this in the gap analysis?

Yihao: I find 2 paper below that might help.
1. Margi C B, Simplicio Jr M A, Näslund M, et al. Impact of operating systems on wireless sensor networks (security) applications and testbeds[C]//2010 Proceedings of 19th International Conference on Computer Communications and Networks. IEEE, 2010: 1-6.
2. Mesrinejad F, Hashim F, Noordin N K, et al. The effect of fragmentation and header compression on IP-based sensor networks (6LoWPAN)[C]//The 17th Asia Pacific Conference on Communications. IEEE, 2011: 845-849.
Luigi: may be consider:
- Abdelfadeel KQ, Cionca V, Pesch D. Lschc: Layered static context header compression for lpwans. InProceedings of the 12th Workshop on Challenged Networks 2017 Oct 20 (pp. 13-18).
- Tömösközi M, Seeling P, Ekler P, Fitzek FH. Performance evaluation and implementation of IP and robust header compression schemes for TCP and UDP traffic in static and dynamic wireless contexts. Computer Science and Information Systems. 2017;14(2):283-308.
-->


Greater flexibility in Internet addressing may avoid complex and energy hungry operations, like header compression and fragmentation, necessary to translate protocol headers from one limited domain to another.


## Communication within Dynamically Changing Topologies {#SEC:dynamic}

Communication may occur over networks that exhibit dynamically changing topologies. One such example is that of satellite networks, providing global Internet connections through a combination of inter-satellite and ground station communication.
With the convergence of space-based and terrestrial networks, users can experience seamless broadband access, e.g., on cruise ships, flights, and within cars, often complemented by and seamlessly switching between Wi-Fi, cellular, or satellite based networks at any time.
The satellite network service provider will plan the transmission path of user traffic based on the network coverage, satellite orbit, route, and link load, providing potentially high-quality Internet connections for users in areas that are not, or hard to be, covered by terrestrial networks. The involved topologies of the satellite network will be changing constantly while observing a regular flight pattern in relation to other satellite and predictable overflight patterns to ground users.

Another example is that of vehicular communication, where services may be accessed across vehicles, such as self-driving cars, for the purpose of collaborative objection recognition (e.g., for collision avoidance), road status conveyance (e.g., for pre-warning of road-ahead conditions) and other purposes. Communication may include RoadSide Units (RSU) with the possibility to create ephemeral connections to those RSUs for the purpose of workload offloading, joint computation over multiple (vehicular) inputs and other purposes {{I-D.ietf-lisp-nexagon}}. Communication here may exhibit a multi-hop nature, not just involving the vehicle and the RSU over a direct link. Those topologies are naturally changing constantly due to the dynamic nature of the involved communication nodes.

In both network technologies, there is a significant difference between the high dynamics of the underlying network topologies, compared to the relative static nature of terrestrial network topology, as reported in {{HANDLEY}}. As a consequence, the notion of a topological network location becomes restrictive in the sense that not only the relation between network nodes and user endpoint may change, but also the relation between the nodes that form the network itself. This may lead to the challenge of maintaining and updating the topological addresses in this constantly changing network topology.

In attempts to utilize entirely different semantics for the addressing itself, geographic-based routing, such as in {{CARTISEAN}}, has been proposed for MANETs (mobile ad-hoc networks) through providing geographic coordinates based addresses to achieve better routing performance, lower overhead, and lower latency {{MANET1}}.


Flexibility in Internet addressing here would allow for accommodating such geographic address semantics into the overall Internet addressing.


## Communication among Moving Endpoints {#SEC:mobility}

<!-- Luigi:
This Section was initially suggested to be between steering ans security, however, becasue the topic is close to :changing topology" I put it here. Not sure whether or not we should actually merge it to the previous.
Even more, because this section refers to protocols presented in other sections we might consider putting both section after the alternative forwarding section. 
-->

<!-- Yihao:
As for the name of the subsection, "Communication among Moving Endpoints" and "Communication within Dynamically Changing Topologies" have some overlap. Moving endpoint can lead to Dynamically Changing Topologies (like mobile phone), and Dynamically Changing Topologies can also refer to moving endpoint (like moving vehicles). 

How about:

2.3 Communication within Dynamically Changing Topologies

2.3.1 Communication among Moving Endpoints

2.3.2 Communication within Moving backbone

2.3.3 Communication within Moving Mesh-networking

NOTE: Point taken and need to think how to structure better but to be done in future version
NOTE: let's leave the structure for now and possibly discuss changes if mailing list discussions suggest doing so, also allowing for engaging with the list on how to do those changes

-->


When packet switching was first introduced, back in the 60s/70s, it was intended to replace the rigid circuit switching with a communication infrastructure that was more resilient to failures. As such, the design never really considered communication endpoints as mobile. Even in the pioneering ALOHA {{ALOHA}} system, despite considering wireless and satellite links, the network was considered static (with the exception of failures and satellites, which fall in what is discussed in {{SEC:dynamic}}). Ever since, a lot of efforts have been devoted to overcome such limitations once that it became clear that endpoint mobility will become a main (if not THE main) characteristic of ubiquitous communication systems.

The IETF has for a long time worked on solutions that would allow extending the IP layer with mobility support. Because of the topological semantic of IP addresses, endpoints need to change addresses each time they visit a different network. However, because routing and endpoint identification is also IP address based, this leads to a communication disruption.

To cope with such a situation, anchor-based Mobile IP mechanisms have been introduced ({{?RFC5177}}, {{?RFC6626}} {{?RFC5944}}, {{?RFC5275}}). Mobile IP is based on a relatively complex and heavy mechanism that makes it hard to deploy and not very efficient. Furthermore, it is even less suitable than native IP in constrained environments like the ones discussed in {{SEC:constrained}}.

Alternative approaches to Mobile IP often leverage the introduction of some form of overlay. LISP {{I-D.ietf-lisp-introduction}}, by separating the topological semantic from the identification semantic of IP addresses, is able to cope with endpoint mobility by dynamically mapping endpoint identifiers with routing locators {{I-D.ietf-lisp-mn}}. This comes at the price of an overlay that needs its own additional control plane {{?I-D.ietf-lisp-rfc6833bis}}. Similarly, the NVO3 (Network Virtualization Overlays) Working Group, while focusing on Data Center Environments, also explored an overlay-based solution for multi-tenancy purposes, but also resilient to mobility since relocating Virtual Machines (VMs) is common practice. NVO3 considered for a long time several data planes that implement slightly different flavors of overlays ({{?RFC8926}}, {{?RFC7348}}, {{I-D.ietf-intarea-gue}}), but lack of an efficient control-plane specifically tailored for DCs.

Alternative mobility architectures have also been proposed in order to cope with endpoint mobility outside the IP layer itself. The Host Identity Protocol (HIP) {{?RFC7401}} introduced a new namespace in order to identify endpoints, namely the Host Identity (HI), while leveraging the IP layer for topological location. On the one hand, such an approach needs to revise the way applications interact with the network layer, by modifying the DNS (now returning an HI instead of an IP address) and applications to use the HIP socket extension. On the other hand, early adopters do not necessarily gain any benefit unless all communicating endpoints upgrade to use HIP.  In spite of this, such a solution may work in the context of a limited domain.

Another alternative approach is adopted by Information-Centric Networking (ICN) {{?RFC7476}}. By making content a first class citizen of the communication architecture, the "what" rather than the "where" becomes the real focus of the communication. However, as explained in the next sub-section, ICN can run either over the IP layer or completely replace it, which in turn can be seen as running the Internet and ICN as logically completely separated limited domains.

Sometimes, the transport layer gets involved in mobility solutions, either by introducing explicit in-band signaling to allow for communicating IP address changes (e.g., in SCTP {{?RFC5061}} and MPTCP {{?RFC6182}}), or by introducing some form of connection ID that allows for identifying a communication independently from IP addresses (e.g., the connection ID used in QUIC {{QUIC}}).

Greater flexibility in addressing may help in dealing with mobility more efficienctly, e.g., through an augmented semantic that may fufill the mobility requirements {{?RFC7429}}.


## Communication Across Services {#SEC:service}

As a communication infrastructure spanning many facets of life, the Internet integrates services and resources from various aspects such as remote collaboration, shopping, content production as well as delivery, education and many more. Accessing those services and resources directly through URIs has been proposed by methods such as those defined in ICN {{?RFC7476}}, where providers of services and resources can advertise those through unified identifiers without additional planning of identifiers and locations for underlying data and their replicas. Users can access required services and resources by virtue of using the URI-based identification, with an ephemeral relationship built between user and provider, while the building of such relationship may be constrained with user- as well as service-specific requirements, such as proximity (finding nearest provider), load (finding fastest provider), and others.

While systems like ICN {{CCN}} provide an alternative to the locator-based addressing of IP, its deployment requires an overlay (over IP) or native deployment (alongside IP), the latter with dedicated gateways needed for translation. Underlay deployments are also envisioned in {{?RFC8763}}, where ICN solutions are being used to facilitate communication between IP addressed network endpoints or URI-based service endpoints, still requiring gateway solutions for interconnection with ICN-based networks as well as IP routing based networks (cf., {{ICN5G}}{{ICNIP}}).

Although various approaches to combining service and location-based addressing have been devised, the key challenge here is to facilitate a "natural", i.e., direct communication, without the need for gateways above the network layer.


<!-- Yihao:
specifically for the SFC part, there is a strong overlap between "Communication Across Services" and "Steering Communication Traffic". have a better storyline for it? 
For me, ICN related works imply an Alternative Forwarding Architectures. How about we move ICN to the last sub-section and merge "Communication Across Services" and "Steering Communication Traffic" into one sub-section?
(not sure about the postion of dyncast, is it more close to ICN?)

like:

2.4 Communication under traffic control

2.4.1 Communication with traffic permission
vlan...vxlan...

2.4.2 Communication with traffic navigation
SFC...MPLS...SRv6

-->


Another aspect of communication across services is that of chaining individual services to a larger service. Here, an identifier could be used that serves as a link to next hop destination within the chain of individual services, as done in the work on Service Function Chaining (SFC). With this, services are identified at the level of Layer 2/3 ({{?RFC7665}}, {{?RFC8754}}, {{?RFC8595}}) or at the level of name-based service identifiers like URLs {{?RFC8677}} although the service chain identification is carried as an NSH header ({{?RFC7665}} separate to the packet identifiers. The forwarding with the chain of services utilizes individual locator-based IP addressing (for L3 chaining) to communicate the chained operations from one Service Function Forwarder {{?RFC7665}} to another, leading to concerns regarding overhead incurred through the stacking of those chained identifiers in terms of packet overhead and therefore efficiency in handling in the intermediary nodes.

Greater flexibility in addressing may allow for incorporating different information, e.g., service as well as chaining semantics, into the overall Internet addressing.


## Steering Communication Traffic {#SEC:steering}

Steering traffic within a communication scenario may involve at least two aspects, namely (i) limiting certain traffic towards a certain set of communication nodes and (ii) constraining the sending of packets towards a given destination (or a chain of destinations) with metrics that would allow the selection among one or more possible destinations.

One possibility for limiting traffic inside limited domains, towards specific objects, e.g., devices, users, or group of them, is subnet partition with techniques such as VLAN {{?RFC5517}}, VxLAN {{?RFC7348}}, or more evolved solution like Terastream {{TERASTREAM}} realizing such partitioning. Such mechanisms usually involve quite some configuration, and even small changes in network and user nodes could result in a repartition and possibly even more configuration efforts. Another key aspect is the complete lack of correlation of the topological address and any likely more semantic-rich identification that could be used to make policy decision regarding traffic steering. Suitably enriching the semantics of the packet address, either that of the sender or receiver, so that such decision could be made while minimizing the involvement of higher layer mechanisms, is a crucial challenge for improving on network operations and speed of such limited domain traffic.

When making decisions to select one out of a set of possible destinations for a packet, IP anycast semantics can be applied albeit being limited to the locator semantic of the IP address itself. Recent work in {{DYNCAST}} suggests utilizing the notion of IP anycast address to encode a "service identifier", which is dynamically mapped onto network locations where service instances fulfilling the service request may be located.
Scenarios where this capability may be utilized are provided in {{DYNCAST}} and include, but are not limited to, scenarios such as edge-assisted VR/AR, transportation and digital twins.

The challenge here lies in the possible encoding of not only the service information itself but the constraint information that helps the selection of the "best" service instance and which is likely a service-specific constraint in relation to the particular scenario. The notion of an address here is a conditional (on those constraints) one where this conditional part is an essential aspect of the forwarding action to be taken. It needs therefore consideration in the definition of what an address is, what is its semantic, and how the address structure ought to look like.

As outlined in the previous sub-section, chaining services are another aspect of steering traffic along a chain of constituent services, where the chain is identified through either a stack of individual identifiers, such as in Segment Routing {{?RFC8402}}, or as an identifier that serves as a link to next hop destination within the chain, such as in Service Function Chaining (SFC). The latter can be applied to services identified at the level of Layer 2/3 ({{?RFC7665}}, {{?RFC8754}}, {{?RFC8595}}) or at the level of name-based service identifiers like URLs {{?RFC8677}}. However, the overhead incurred through the stacking of those chained identifiers is a concern in terms of packet overhead and therefore efficiency in handling in the intermediary nodes.


<!-- NOTES: Dirk
What other references?
AP: add references also here but discuss gap later (ALL)
-->


<!-- NOTES: Yihao
Shall we spilt this sub-section into two: 1. Communication with traffic permission; 2. Communication with traffic navigation
Dirk: not sure that dividing into explicit sub-section helps. It is steering, one guided by permission and the other by chaining objectives (the latter has a linkage to the previous sub-section on comms across services). Also, the suggested second item is merely another expression for traffic steering (since navigation is close/similar to steering)

NOTE: see above about changes
-->


Flexibity in addressing may enable more semantic rich encoding schemes that may help in steering traffic at hardware level and speed, without complex mechanisms usually resulting in handling packets in the slow path of routers.

## Communication with built-in security {#SEC:builtin-sec}

Today, strong security and privacy in the Internet is usually implemented as an overlay based on the concept of Mix Networks ({{TOR}}, {{SPHINX}}). Among the various reasons for such approach is the limited semantic of current IP addresses, which do not allow to natively express security features or trust relationship. Efforts like Cryptographically Generated Addresses (CGA) {{?RFC3972}}, provide some security features by embedding a truncated public key in the last 57-bit of IPv6 address, thereby greatly enhancing authentication and security within an IP network via asymmetric cryptography and IPsec {{?RFC4301}}. The development of the Host Identity Protocol (HIP) {{?RFC7401}} saw the introduction of cryptographic identifiers for the newly introduced Host Identity (HI) to allow for enhanced accountability, and therefore trust. The use of those HIs, however, is limited by the size of IPv6 128bit addresses.

Through a greater flexibility in addressing, any security-related key, certificate, or identifier could instead be included in a suitable address structure without any information loss (i.e., as-is, without any truncation or operation as such), avoiding therefore compromises such as those in HIP. Instead, CGAs could be created using full length certificates, or being able to support larger HIP addresses in a limited domain that use it.

Greater flexibility in addressing semantic could significantly help in constructing a trusted and secure communication at the network layer. This could lead to connections that could be considered as absolute secure (assuming the cryptography involved is secure). Even more, anti-abuse mechanisms and/or DDoS protection mechanisms like the one under discussion in PEARG ({{PEARG}}) Research Group may leverage a greater flexibility of the overall Internet addressing, if provided, in order to be more effective.


## Communication in Alternative Forwarding Architectures {#SEC:nin}

<!-- Yihao: 

Now if our position is only pointing out the problem of the current Internet addressing, is it really apporiate to say the current internet have problem when apply it in an Alternative Forwarding Architectures?

how about we use name: Communication for flow-level optimization

-->

<!-- Yihao:

I feel that the way we narrate this sub-section is somehow weird.
As this section is talk about use cases/requirement from the real world, like constrained devices, security, traffic steering... However, an Alternative Forwarding Architectures look like requirement from another dimension. For me, Alternative Forwarding Architectures is more like requirement from technical aspect, not the real world. Since user in real world never care about the forwarding architecture, and it's not the use case from users' perspective.

On the other hand, flexible addressing itself could imply the Alternative Forwarding Architectures. For example, "Communication Across Services" should already imply an Alternative Forwarding Architectures.

I suggest that we use the real use cases for these Alternative Forwarding Architectures as we describe here, like video, Deterministic QoS, and what works better under flow-based or path-based stream (instead of packet-based).

Besides, Sheng Jiang is worrying about NIN, and the way we mention NIN.
Maybe it is better to talk the "use case" of NIN, instead of Alternative Forwarding Architectures like NIN. Thus we could totally avoid mentioning NIN.

-->

<!-- Dirk: I suggest keeping the 'alternative forwarding architecture'. In the other sections, we address the 'aspect' of communication, e.g., changing topology, mobility, ..., not the use cases either. The use case for the sat aspect in 'changing topologies' is plain Internet access, so not particularly 'out there'. Further, the introduction of SDN was not just, if at all, motivated by better handling of streaming scenarios; nor for NIN. Hence, I'd leave it as is. -->


<!-- AP: Dirk: start this sub-section with a clear goal motivating 'alternative forwarding architecture'. This could be the desired higher efficiency, e.g., for streaming scenarios [DOne: create the starting paragraph, also with reference to MPLS and its motivation to improve on traffic engineering]
AP: Luigi: review that new paragraph and link it to ETSI paragraph  [DONE minor changes]

-->

The performance of communication networks has long been a focus for optimization due to the immediate impact on cost of ownership for communication service providers. Technologies like MPLS {{?RFC3031}} have been introduced to optimize lower layer communication, e.g., by mapping L3 traffic into aggregated labels of forwarding traffic for the purposes of, e.g., traffic engineering.

Even further, other works have emerged in recent years that have replaced the notion of packets with other concepts for the same purpose of improved traffic engineering and therefore efficiency gains. One such area is that of Software Defined Networks (SDN) {{?RFC7426}}, which has highlighted how a majority of Internet traffic is better identified by flows, rather than packets. Based on such observation, alternate forwarding architectures have been devised that are flow-based or path-based. With this approach, all data belonging to the same traffic stream is delivered over the same path, and traffic flows are identified by some connection or path identifier rather than by complete routing information, possibly enabling fast hardware based switching.

On the one hand, such a communication model may be more suitable to real-time traffic like that in the context of Deterministic Networks ({{DETNET}}), where indeed a lot of work has focused on how to "identify" packets belonging to the same DETNET flow in order to jointly manage the forwarding within the desired deterministic boundaries.

On the other hand, it may improve the communication efficiency in constrained wireless environments (cf., {{SEC:constrained}}), by reducing the overhead, hence increasing the number of useful bits per second per Hz. Also, the delivery of information across similar flows may be combined into a multipoint delivery of a single return flow, e.g., for scenarios of requests for a video chunk from many clients being responded to with a single (multi-destination) flow, as outlined in {{BIER-MC}} as an example. Another opportunity to improve communication efficiency is being pursued in ongoing IETF/IRTF work to deliver IP- or HTTP-level packets directly over path-based or flow-based transport network solutions, such as in {{TROSSEN}}{{BIER-MC}}{{ICNIP}}{{ICN5G}} with the capability to bundle unicast forward communication streams flexibly together in return path multipoint relations. Such capability is particularly opportune in scenarios such as chunk-based video retrieval or distributed data storage. However, those solutions currently require gateways to "translate" the flow communication into the packet-level addressing semantic in the peering IP networks. Furthermore, the use of those alternative forwarding mechanisms often require the encapsulation of Internet addressing information, leading to wastage of bandwidth as well as processing resources. 

<!-- NOTES: Dirk: I reworded the paragraph here, particularly removing any linkage to TCP and IP but centring the work on the alternative forwarding architectures and the formation of a limited domain through this
Luigi: Looks OK for me.
-->

Alternative way of forwarding data has also been the motivation for the efforts created in the European Telecommunication Standards Institute (ETSI), who formed a Industry Specification Group (ISG) named Non-IP Networking (NIN) {{ETSI-NIN}}. This group sets out to develop and standardize a set of protocols leveraging an alternative forwarding architecture, such as provided by a flow-based switching paradigm. The deployment of such protocols may be seen to form limited domains, still leaving the need to interoperate with the (packet-based forwarding) Internet; a situation possibly enabled through a greater flexibility of the addressing used across Internet-based and alternative limited domains alike.

<!-- NOTES: Dirk
Make the addressing angle of NIN here clearer (Dirk, then Luigi to review)
DIRK: changed the NIN paragraph to position NIN solutions as limited domains with the need for flexible addressing for cross-domain comms.
DIRK: simplifed first paragraph since there was repetition in the next one (where the comms model was seen more suitable for real-time traffic)
-->

A greater flexibility in addressing semantics may reduce the aforementioned wastage by accommodating Internet addressing in the light of such alternative forwarding architectures, instead enabling the direct use of the alternative forwarding information. 


# Issues in Addressing {#SEC:problem}
<!-- NOTES Dirk: I tried addressing the sub-section headings as something 'limiting' to some extent, given that it's the "problems" section -->


<!-- AP Dirk -->

## Limiting Alternative Address Semantics {#SEC:pro:semantics}

Many approaches to changing the semantics of communication, e.g., through separating host identification from network node identification {{?RFC7401}} or through identifying content and services directly {{HICN}}, are limited by the existing packet size and semantic constraints of IPv6, e.g., in the form of its source and destination network addresses.

While approaches such as {{ICNIP}} may override the addressing semantics, e.g., by replacing IPv6 source and destination information with path identification, a possible unawareness of endpoints still requires the carrying of other address information as part of the payload, as discussed in {{SEC:pro:efficiency}}.
Also, the expressible service or content semantic may be limited, as in {{HICN}} or the size of supported networks {{REED}} due to relying on the limited bit positions usable in IPv6 addresses.

<!-- Move paragraph to secuirty section since it is more suitable -->
<!-- AP Luigi [DONE] -->

## Hampering Security {#SEC:pro:security}

Fitting any new semantic into existing size constraints may hamper the original objectives for introducing the new semantics in the first place. For instance, host identifiers {{?RFC7401}} or security information may be limited by the IPv6 address size, as discussed in {{SEC:builtin-sec}} with the example of CGA {{?RFC3972}}. On the one hand, greater flexibility of addressing would allow to introduce fully featured security in endpoint identification, potentially able to eradicate the spoofing problem. On the other hand, it may be used to include application gateways' certificates in order to provide more efficiency, e.g., using web certificates also used in the addressing of web services.

While increasing security, privacy protection can be improved. IP addresses, even temporary ones, have been long recognized as a "Personal Identification Information" that allows even to geolocating the communicating endpoints {{?RFC8280}}. Greater flexibility in addressing may allow the use of cryptographically generated anonymous addresses when considered needed, and protect from geolocation by making such addresses topologically independent. Such property potentially allows implemetation of secure architetures like {{TOR}} and {{SPHINX}} at network layer, improving the overall efficiency as described in {{SEC:pro:efficiency}}.

Alternative addressing semantics may also help in (D)DoS mitigation. This can be achieved by changing the service identification model, making it completely orthogonal from network topology semantic. And by not exposing all of the topological information the attack exposes, the potential disruptions, may remain limited {{ADDRLESS}}. In this way, mounting such type of attack may become harder.

<!-- AP Dirk -->

## Complicating Traffic Engineering {#SEC:pro:traffic}

Efforts in traffic engineering have long shown that the IP address itself is not enough to steer traffic properly, seeing the introduction of differentiated service code points (DSCP), the use of header information of various kinds (such as ports) as flow information, and the entirely separate expression of path information, e.g., in the form of MPLS labels or through introducing bitposition-based path identifiers (cf., {{BIER-MC}}, {{REED}}). Newer approaches to IP anycast suggest the use of service identification in combination with a binding IP address model {{DYNCAST}} as a way to allow for metric-based traffic steering decisions; approaches for service function chaining {{?RFC7665}} utilize the next service header (NSH) information and packet classification to determine the destination of the next packet hop.

Overall, when it comes to providing capabilities for traffic engineering, the IP address itself is not semantically rich enough to adequately describe the forwarding decision to be taken in the network, not only impacting WHERE the packet will need to go but also HOW it will need to be sent. Instead, various supplementary information needs to be taken into account for a successful delivery to take place.


<!-- AP Luigi -->
<!-- NOTES Dirk: I suggest folding this under efficiency since this is mainly covered by 'introducing path stretch' -->
<!-- LUIGI: Agreed. I added some mobility-related sentences in the efficiency sub-sections -->
<!-- ## Supporting Mobility {#SEC:pro:mobility} -->


<!-- AP Yihao -->

## Hampering Efficiency {#SEC:pro:efficiency}

### Header proportion

Although fiber and ethernet dominate the Internet infrastructure, numerous radio channels are expected to improve the wireless communication efficiency. As IPv6 header fixedly occupies 40 byte in a packet {{!RFC8200}}, header compression techniques are introduced to shaping payload occupation within a packet. RObust Header Compression (ROHC) {{?RFC5795}}, which customized for cellar network, is being widely adopted in radios like WCDMA, LTE, and 5G. Considering one base station is supposed to serve hundreds of user devices, maximizing the effectiveness for specific spectrum directly improve user quality of experience.

Similar header compression mechanisms are usually adopted for communications among constrained devices. Due to the memory or battery constraint, constrained devices prefer maximize carrying efficiency for each packet they deliver. For personal area network, the IEEE 802.15.4 enabled devices, which occupy the most share of the market, either equipped with customized proprietary protocols, or compress the header utterly as in {{?RFC4944}}. Particular for proprietary protocols, e.g., Zigbee, an application level gateway should be introduced at the edge of the local network. Terminations of the communications by such gateway break the end-to-end principle via uncondictional trust as potential weak points, thus looping back to the security crisis in {{SEC:pro:security}}.

Also, constraints coming from either devices or carrier links would lead to a mixed scenarios and compound requirements for extraordinary header compression. For native IPv6 communications on DECT ULE and MS/TP Networks, dedicated compression mechanisms are specified in {{?RFC8105}} and {{?RFC8163}}, while the transmission of IPv6 packets over NFC and PLC, specifications are being developed in {{?I-D.ietf-6lo-nfc}} and {{?I-D.ietf-6lo-plc}}. For low power wide-area network, a generic framework for static context header compression is depicted in {{?RFC8724}} for efficiency improvement.


### Introducing Path Stretch

To serve a moving endpoint (cf., {{SEC:mobility}}), mechanisms like Mobile IP {{?RFC3775}} are used for the maintenance of connection continuity. As the result of the locator semantic in IP address {{?RFC2101}}, traffic must follow a triangular route before arriving the updated location inevitably affecting the transmission efficiency as well as latency.

<!-- NOTES Dirk: didn't really quite get the paragraph below -->
<!-- LUIGI: TOR actually uses path stretch as part of path privacy, in TOR nobody knows how many relays are used and nobody knows all the set of them. SO basically this is a feature not a bug. AKA I miss the point as well ...   -->

Another example for introducing additional path lengthening is the routing in TOR (cf., {{SEC:builtin-sec}}). As the address indicates identifications to a certain extent {{?RFC2101}}, privacy enhancement mechanisms usually involve the concealment of the source IP address during communications. To achieve high anonymity, traffic should be handed over by several (at least three) intermediates before reaching the destination. Undoubtedly, frequent relaying enhance the privacy at the cost of lower communication efficiency, no matter how close the destination is located.

IP Anycast {{?RFC7094}} is usually adopted for efficient content delivery through extensive replica distribution. In most cases, request packets should be guided to the nearest server in relation to, e.g., geography or network topology, while occasionally, traffic may also be directed to a remote or suboptimal site. Given that Autonomous Systems (AS) always select route according to their own preference, e.g., route of customer AS path (rather than shortest path), traffic guidance for the nearest site is hard to be guaranteed (cf., {{ANYCAST}}), while computing-related metrics are mostly ignored.


### Repetitive encapsulation

Addressing proposals such as those in {{ICNIP}} utilize path identification within an alternative forwarding architecture that acts upon the provided path identification. However, due to the limitation of existing flow-based architectures with respect to the supported header structures (in the form of IPv4 or IPv6 headers), the new routing semantics are being inserted into the existing header structure, while repeating the original, sender-generated header structure, in the payload of the packet as it traverses the limited domain, effectively doubling the header overhead per packet.

The problem is also present in a number of solutions tackling different issues, e.g., mobility  {{I-D.ietf-lisp-introduction}}, DC networking ({{?RFC8926}}, {{?RFC7348}}, {{I-D.ietf-intarea-gue}}), and privacy ({{TOR}}, {{SPHINX}}). Certainly these solutions are able to avoid other issues, like path lengthening or privacy, but they come at the price of multiple encapsulations that reduce the effective payload.






# Problem Statement

This document highlights that, with the emergence of limited domains, novel approaches to addressing in communication scenarios are being developed and deployed within those limited domains.

While this may be interpreted as a crucial point to the flexibility of addressing in the Internet, evidences exist (as describe in this document) that the existing Internet addressing structure itself is a potential hinderance in solving key problems for Internet service provisioning. Such problems include supporting new, e.g., service-oriented, scenarios more efficiently, with improved security and efficient traffic engineering, as well as large scale mobility.

As a problem statement, this document's goal is not to propose or promote specific solutions to the problems here portrayed. Instead, this document aims at stimulating discussion on the emerging needs for addressing with the possibility to fundamentally re-think the addressing in the Internet beyond the current objectives of IPv6.


# Security Considerations {#SEC:sec}

TBD.


# IANA Considerations {#SEC:iana}

This document does not include an IANA request.


--- back


<!-- 

# Change Log

**NOTES**: Please remove this section prior to publication of a final version of this document.

TBD.

# Acknowledgments
{:numbered="false"}

Here is Acknowledgements.

-->

---
coding: utf-8

title: "Challenging Scenarios and Problems in Internet Addressing"
abbrev: "Scenarios and Problems in Addressing"
docname: draft-jia-intarea-scenarios-problems-addressing-02
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
  ins: N. Shenoy
  name: Nirmala Shenoy
  org: Rochester Institute of Technology
  abbrev: RIT
  # role: editor
  street: ''
  city: New-York
  country: USA
  code: '14623'
  email: nxsvks@rit.edu
-
  ins: P. Mendes
  name: Paulo Mendes
  org: Airbus
  abbrev: Airbus
  # role: editor
  street: Willy-Messerschmitt Strasse 1
  city: Munich
  country: Germany
  code: '81663'
  email: paulo.mendes@airbus.com
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
  # placeholder here for the gap analysis draft
  I-D.jia-intarea-internet-addressing-gap-analysis:

  # DYNCAST: I-D.liu-dyncast-ps-usecases
  # (I don't know why it is not archived/tracked by datatracker.ietf.org)
  SFCANYCAST: DOI.10.1145/3314148.3314355
  #DYNCAST: I-D.geng-rtgwg-cfn-dyncast-ps-usecase
  QUIC: I-D.ietf-quic-transport
  ICN5G: I-D.irtf-icnrg-5gc-icn
  ICNIP: I-D.trossen-icnrg-internet-icn-5glan
  BIER-MC: I-D.ietf-bier-multicast-http-response


  MANET1: DOI.10.1177/1550147716671255
  CCN: DOI.10.1145/1658939.1658941
  HANDLEY: DOI.10.1145/3286062.3286075
  TROSSEN: DOI.10.1145/1764873.1764878
  ALOHA: DOI.10.1145/205447.205451
  CARTISEAN: DOI.10.1007/978-3-540-39611-6_27
  #ANYCAST: DOI.10.1145/3230543.3230547
  #ADDRLESS: DOI.10.1371/journal.pone.0246293
  #REED: DOI.10.1109/ICC.2016.7511036
  WANG19: DOI.10.1109/ACCESS.2019.2963223
  CHRIKI19: DOI.10.1016/j.comnet.2019.106877
  MAROJEVIC20: DOI.10.1109/MVT.2020.2979494
  PILA: DOI.10.1109/ICCCN52240.2021.9522235
  CHEN21: DOI.10.1109/IWCMC51323.2021.9498722

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
  EIBP:
    title: "A Structured Approach to Routing in the Internet"
    author:
      ins: N. Shenoy, S. Chandraiah, P. Willis
    target: First Intl Workshop on Semantic Addressing and Routing for Future Networks
    date: 2021-06


  # Below are history of current draft
  # I-D.jia-intarea-scenarios-problems-addressing-00:

--- abstract

The Internet Protocol (IP) has been the major technological success in information technology of the last half century. As the Internet becomes pervasive, IP has been replacing communication technology for many domain-specific solutions. However, domains with specific requirements as well as communication behaviors and semantics still exist and represent what {{?RFC8799}} recognizes as "limited domains".

This document describes well-recognized scenarios that showcase possibly different addressing requirements, which are challenging to be accommodated in the IP addressing model. These scenarios highlight issues related to the Internet addressing model and call for starting a discussion on a way to re-think/evolve the addressing model so to better accommodate different domain-specific requirements.

The issues identified in this document are complemented and deepened by a detailed gap analysis in a separate companion document {{I-D.jia-intarea-internet-addressing-gap-analysis}}.

--- middle


# Introduction {#SEC:intro}

The Internet Protocol (IP), positioned as the unified protocol at the (Internet) network layer, is seen by many as key to the innovation stemming from Internet-based applications and services. Even more so, with the success of TCP/IP protocol stack, IP has been gradually replacing existing domain-specific protocols, evolving into the core protocol of the entire communication eco-system. At its inception, roughly 40 years ago {{!RFC0791}}, the Internet addressing system, represented in the form of the IP address and its locator-based semantics, has brought the notion of a 'common namespace for all communication'. Compared to proprietary technology-specific solutions, such 'common namespace for all communication' advance ensures end-to-end communication from any device connected to the Internet to another.

However, use cases, associated services, node behaviors, and requirements on packet delivery have since been significantly extended, with the Internet technology being developed to accommodate them in the framework of addressing that stood at the beginning of the Internet's development. This evolution is reflected in the concept of "Limited Domains", first introduced in {{?RFC8799}}. It refers to a single physical network, attached to or running in parallel with the Internet, or is defined by a set of users and nodes distributed over a much wider area, but drawn together by a single virtual network over the Internet. Key to a limited domain is that requirements, behaviors, and semantics could be noticeable local and, more importantly, specific to the limited domain. Very often, the realization of a limited domain is defined by specific communication scenario(s) and/or use case(s) that exhibit the domain-specific behaviors and pose the requirements that lead to the establishment of the limited domain.

One key architectural aspect, when communicating within limited domains, is that of addressing and, therefore, the address structure, as well as the semantic that is being used for packet forwarding. The topological location centrality of IP is fundamental when reconciling the often differing semantics for 'addressing' that can be found in those limited domains. The result of this fundamental role of the single IP addressing is that limited domains have to adopt specific solutions, e.g., translating/mapping/converting concepts, semantics, and ultimately, domain-specific addressing, into the common IP addressing used across limited domains.

This document advocates flexibility in addressing in order to accommodate limited domain specific semantics, while, if possible, ensuring a single holistic addressing scheme able to reduce, or even entirely remove, the need for aligning the address semantics of different limited domains, such as the current topological location semantic of the Internet. Ultimately, such holistic addressing could be beneficial to those communication scenarios realized within limited domains by improving efficiency, removing of constraints imposed by needing to utilize the limited semantics of IP addressing, and/or in other ways.

In other words, this document revolves around the following question:

> "Should interconnected limited domains purely rely on IP addresses and therefore deal with the complexity of translating any semantic mismatch themselves, or should flexibility for supporting those limited domains be a key focus for an evolved Internet addressing?"

To that end, this document describes well-recognized scenarios in limited domains that could benefit from greater flexibility in addressing and overviews the problems encountered throughout these scenarios due to the lack of that flexibility. A detailed gap analysis can be found in {I-D.jia-intarea-internet-addressing-gap-analysis}}, which elaborates on the issues identified in this memo in reference to extensions to Internet addressing that have attempted to address those issues. The purpose of this memo is rather to stimulate discussion on the emerging needs for addressing at large with the possibility to fundamentally re-think the addressing in the Internet beyond the current objectives of IPv6 {{?RFC8200}}.

It is important to remark that any change in the addressing, hence at the data plane level, leads to changes and challenges at the control plane level, i.e., routing. The latter is an even harder problem than just addressing and might need more research efforts that are beyond the objective of this document, which focuses solely on the data plane.


# Communication Scenarios in Limited Domains {#SEC:cases}

The following sub-sections outline a number of scenarios, all of which belong to the concept of "limited domains" {{?RFC8799}}. While the list of scenarios may look long, this document focuses on scenarios with a number of aspects that can be observed in those limited domains, captured in the sub-section titles. For each scenario, possible challenges are highlighted, which are then picked upon in {{SEC:problem}}, when describing more formally the existing  shortcomings in current Internet addressing.


## Communication in Constrained Environments {#SEC:constrained}

In a number of communication scenarios, such as those encountered in the Internet of Things (IoT), a simple, communication network demanding minimal resources is required, allowing for a group of IoT network devices to form a network of constrained nodes, with the participating network and end nodes requiring as little computational power as possible and having small memory requirements in order to reduce the total cost of ownership of the network. Furthermore, in the context of industrial IoT, real-time requirements and scalability make IP technology not naturally suitable as communication technology ({{OCADO}}).

In addition to IEEE 802.15.4, i.e., Low-Rate Wireless Personal Area Network {{LR-WPAN}}, several limited domains exist through utilizing link layer technologies such as Bluetooth Low Energy (BLE) {{BLE}}, Digital European Cordless Telecommunications (DECT) - Ultra Low Energy (ULE) {{DECT-ULE}}, Master-Slave/Token-Passing (MS/TP) {{BACnet}}, Near-Field-Communication (NFC) {{ECMA-340}}, and Power Line Communication (PLC) {{IEEE_1901.1}}.

The end-to-end principle (detailed in {{?RFC2775}}) requires Internet protocols (e.g., IPv6 {{?RFC8200}}) to run on such constrained nodes networks, allowing IoT devices using multiple communication technologies to talk on the Internet. Often, devices located at the edge of constrained networks act as gateway devices, usually performing header compression ({{?RFC4919}}). To ensure security and reliability, multiple gateways must be deployed. IoT devices on the network can select one of those gateways for traffic passthrough by the devices on the (limited domain) network.

Given the constraints imposed on the computational and possibly also communication technology, the usage of a single addressing semantic in the form of a 128-bit endpoint identifier, i.e., IPv6 address, may pose a challenge when operating such networks.

Another type of (differently) constrained environment is an aircraft, which encompasses not only passenger communication but also the integration of real-time data exchange to ensure that processes and functions in the cabin are automatically monitored or actuated. The goal for any aircraft network is to be able to send and receive information reliably and seamlessly. From this perspective, the medium with which these packets of information are sent is of little consequence so long as there is a level of determinism to it. However, there is currently no effective method in implementing wireless inter- and intra-communications between all subsystems. The emerging wireless sensor network technology in commercial applications such as smart thermostat systems, and smart washer/dryer units could be transposed onto aircraft and fleet operations. The proposal for having an Wireless Avionics Intra-Communications (WAIC) system promises reduction in the complexity of electrical wiring harness design and fabrication, reduction in wiring weight, increased configuration, and potential monitoring of otherwise inaccessible moving or rotating aircraft parts. Similar to the IoT concept, WAIC systems consist of short-range communications and are a potential candidate for passenger entertainment systems, smoke detectors, engine health monitors, tire pressure monitoring systems, and other kinds of aircraft maintenance systems.

While there are still many obstacles in terms of network security, traffic control, and technical challenges, future WAIC can enable real-time seamless communications between aircraft and between ground teams and aircraft as opposed to the discrete points of data leveraged today in aircraft communications. For that, WAIC infrastructure should also be connected to outside IP based networks in order to access edge/cloud facilities for data storage and mining. However, the restricted capacity (energy, communication) of most aircraft devices (e.g. sensors) and the nature of the transmitted data – periodic transmission of small packets – may pose some challenges for the usage of a single addressing semantic in the form of a 128-bit endpoint identifier, i.e., an IPv6 address. Moreover, most of the aircraft applications and services are focused on the data (e.g. temperature of gas tank on left wing) and not on the topological location of the data source. This means that the current topological location semantic of IP addresses is not beneficial for aircraft applications and services.

Greater flexibility in Internet addressing may avoid complex and energy hungry operations, like header compression and fragmentation, necessary to translate protocol headers from one limited domain to another, while enabling semantics different from locator-based addressing may better support the communication that occurs in those environments.

## Communication within Dynamically Changing Topologies {#SEC:dynamic}

Communication may occur over networks that exhibit dynamically changing topologies. One such example is that of satellite networks, providing global Internet connections through a combination of inter-satellite and ground station communication. With the convergence of space-based and terrestrial networks, users can experience seamless broadband access, e.g., on cruise ships, flights, and within cars, often complemented by and seamlessly switching between Wi-Fi, cellular, or satellite based networks at any time {{WANG19}}.

The satellite network service provider will plan the transmission path of user traffic based on the network coverage, satellite orbit, route, and link load, providing potentially high-quality Internet connections for users in areas that are not, or hard to be, covered by terrestrial networks. The involved topologies of the satellite network will be changing constantly while observing a regular flight pattern in relation to other satellite and predictable overflight patterns to ground users {{CHEN21}}.

Although satellite bearer services are capable of transporting IPv4 and IPv6, as well as associated protocols such as IP Multicast, DNS services and routing information, no IP functionality is implemented on-board the spacecraft limiting the capability of leveraging for instance large scale satellite constellations.

One of the major constraints of deploying routing capability on board of a satellite is power consumption. Due to this, space routers may end up being intermittently powered up during a daytime sunlit pass. Another limitation of the first generation of IP routers in space was the lack of capability to remotely manage and upgrade software while in operation.

The limitations faced in early development of IP based satellite communication payloads, showed the need to develop a flexible networking solution that would only allow delay tolerant communications in the present of intermittent connectivity as well as a networking solution able to perform in a scenario encompassing mobile devices with the capability of storing data, leading to a significant reduction of latency, which is the major impairment of satellite networks.

Moreover, due to the current IP addressing scheme and its focus on IP unicast addressing with extended deployment of IP multicast and some IP anycast, current deployments do not take advantage of the broadcast nature of satellite networks.

Moreover networking platforms based on a name (data or service) based addressing scheme would bring several potential benefits to satellite networks aiming to tackle their major challenges, including high propagation delay and changing network topology in the case of LEO constellations.

Another example is that of vehicular communication, where services may be accessed across vehicles, such as self-driving cars, for the purpose of collaborative objection recognition (e.g., for collision avoidance), road status conveyance (e.g., for pre-warning of road-ahead conditions), and other purposes. Communication may include Road Side Units (RSU) with the possibility to create ephemeral connections to those RSUs for the purpose of workload offloading, joint computation over multiple (vehicular) inputs, and other purposes {{I-D.ietf-lisp-nexagon}}. Communication here may exhibit a multi-hop nature, not just involving the vehicle and the RSU over a direct link. Those topologies are naturally changing constantly due to the dynamic nature of the involved communication nodes.

The advent of Flying Ad-hoc NETworks (FANETs) has opened up an opportunity to create new added-value services {{CHRIKI19}}. Although these networks share common features with vehicular ad hoc networks, they present several unique characteristics such as energy efficiency, mobility degree, the capability of swarming, and the potential large scale of swarm networks. Due to high mobility of FANET nodes, the network topology changes more frequently than in a typical vehicular ad hoc network. From a routing point of view, although ad-hoc reactive and proactive routing approaches can be used, there are other type of routing protocols that have been developed for FANETS, such as hybrid routing protocols and position based routing protocols, aiming to increase efficiency in large scale networks with dynamic topologies.


Both type of protocols challenge the current Internet addressing semantic: in the case of hybrid protocols, two different routing strategies are used inside and outside a network zone. While inside a zone packets are routed to a specific destination IP address, between zones, query packets are routed to a subset of neighbors as determined by a bordercast algorithm. In the case of position based routing protocol, the IP addressing scheme is not used at all, since packets are routed to a different identifier, corresponding to the geographic location of the destination and not its topological location. Hence, what is needed is to consolidate the geo-spatial addressing with that of a locator-based addressing in order to optimize routing policies across the zones.

Moreover most of the application/services deployed in FANETs tend to be agnostic of the topological location of nodes, rather focusing on the location of data or services. This distinction is even more important because is dynamic network such as FANET robust networking solutions may rely on the redundancy of data and services, meaning that they may be found in more than one device in the network. This in turn may bring into play a possible service-centric semantic for addressing the packets that need routing in the dynamic network towards a node providing said service (or content).

In the aforementioned network technologies, there is a significant difference between the high dynamics of the underlying network topologies, compared to the relative static nature of terrestrial network topology, as reported in {{HANDLEY}}. As a consequence, the notion of a topological network location becomes restrictive in the sense that not only the relation between network nodes and user endpoint may change, but also the relation between the nodes that form the network itself. This may lead to the challenge of maintaining and updating the topological addresses in this constantly changing network topology.

In attempts to utilize entirely different semantics for the addressing itself, geographic-based routing, such as in {{CARTISEAN}}, has been proposed for MANETs (Mobile Ad-hoc NETworks) through providing geographic coordinates based addresses to achieve better routing performance, lower overhead, and lower latency {{MANET1}}.

Flexibility in Internet addressing here would allow for accommodating such geographic address semantics into the overall Internet addressing, while also enabling name/content-based addressing, utilizing the redundancy of many network locations providing the possible data.

## Communication among Moving Endpoints {#SEC:mobility}

When packet switching was first introduced, back in the 60s/70s, it was intended to replace the rigid circuit switching with a communication infrastructure that was more resilient to failures. As such, the design never really considered communication endpoints as mobile. Even in the pioneering ALOHA {{ALOHA}} system, despite considering wireless and satellite links, the network was considered static (with the exception of failures and satellites, which fall in what is discussed in {{SEC:dynamic}}). Ever since, a lot of efforts have been devoted to overcome such limitations once it became clear that endpoint mobility will become a main (if not THE main) characteristic of ubiquitous communication systems.

The IETF has for a long time worked on solutions that would allow extending the IP layer with mobility support. Because of the topological semantic of IP addresses, endpoints need to change addresses each time they visit a different network. However, because routing and endpoint identification is also IP address based, this leads to a communication disruption.

To cope with such a situation, sometimes, the transport layer gets involved in mobility solutions, either by introducing explicit in-band signaling to allow for communicating IP address changes (e.g., in SCTP {{?RFC5061}} and MPTCP {{?RFC6182}}), or by introducing some form of connection ID that allows for identifying a communication independently from IP addresses (e.g., the connection ID used in QUIC {{QUIC}}).

Concerning network layer only solutions, anchor-based Mobile IP mechanisms have been introduced ({{?RFC5177}}, {{?RFC6626}} {{?RFC5944}}, {{?RFC5275}}). Mobile IP is based on a relatively complex and heavy mechanism that makes it hard to deploy and it is not very efficient. Furthermore, it is even less suitable than native IP in constrained environments like the ones discussed in {{SEC:constrained}}.

Alternative approaches to Mobile IP often leverage the introduction of some form of overlay. LISP {{I-D.ietf-lisp-introduction}}, by separating the topological semantic from the identification semantic of IP addresses, is able to cope with endpoint mobility by dynamically mapping endpoint identifiers with routing locators {{I-D.ietf-lisp-mn}}. This comes at the price of an overlay that needs its own additional control plane {{?I-D.ietf-lisp-rfc6833bis}}.

Similarly, the NVO3 (Network Virtualization Overlays) Working Group, while focusing on Data Center environments, also explored an overlay-based solution for multi-tenancy purposes, but also resilient to mobility since relocating Virtual Machines (VMs) is common practice. NVO3 considered for a long time several data planes that implement slightly different flavors of overlays ({{?RFC8926}}, {{?RFC7348}}, {{I-D.ietf-intarea-gue}}), but lacks an efficient control plane specifically tailored for DCs.

Alternative mobility architectures have also been proposed in order to cope with endpoint mobility outside the IP layer itself. The Host Identity Protocol (HIP) {{?RFC7401}} introduced a new namespace in order to identify endpoints, namely the Host Identity (HI), while leveraging the IP layer for topological location. On the one hand, such an approach needs to revise the way applications interact with the network layer, by modifying the DNS (now returning an HI instead of an IP address) and applications to use the HIP socket extension. On the other hand, early adopters do not necessarily gain any benefit unless all communicating endpoints upgrade to use HIP.  In spite of this, such a solution may work in the context of a limited domain.

Another alternative approach is adopted by Information-Centric Networking (ICN) {{?RFC7476}}. By making content a first class citizen of the communication architecture, the "what" rather than the "where" becomes the real focus of the communication. However, as explained in the next sub-section, ICN can run either over the IP layer or completely replace it, which in turn can be seen as running the Internet and ICN as logically completely separated limited domains.

Unmanned Aircraft Systems (UAS) are examples of moving devices that require a stable mobility management scheme since they consist of a number of Unmanned Aerial Vehicles (UAV) subordinated to a Ground Control Station (GCS) {{MAROJEVIC20}}. The information produced by the different sensors and electronic devices available at each UAV is collected and processed by a software or hardware data acquisition unit, being transmitted towards the GCS, where it is inspected and/or analyzed. Analogously, control information transmitted from the GCS to the UAV enables the execution of control operations over the aircraft, such as changing the route planning or the direction pointed by a camera.

Although UAVs may have redundant links to maintain communications in long-range missions (e.g., satellite), most of the communications between the GCS and the UAVs take place over wireless data links, e.g., based on a radio line-of-sight technology, Wi-Fi or 3G/4G/5G. While in some scenarios, UAVs will operate always under the range of the same cellular base station, in missions with large range, UAVs will move between different cellular or wireless ground infrastructure, meaning that the UAV needs to upload its topological locator and re-start the ongoing communication sessions. In such cases, most of existing Mobile IP approaches may play a role, as well as approaches to split the UAV identifier and the topological locator, such as HIP.

However, while the industry is given the first steps towards evolved UAS architectures and communication models, the data-centric communication plays an increasing role, where information is named and decoupled from its location, and applications/services operate over these named data rather than on host-to-host communications.

In this context, the Data Distribution Service (DDS) has emerged as an industry-oriented open standard that follows this approach. The space and time decoupling allowed by DDS is very relevant in any dynamic and distributed system, since interacting entities are not forced to know each other and are not forced to be simultaneously present to exchange data. Time decoupling can significantly simplify the management of intermittent data-links, in particular for wireless connectivity between UAS, as well as facilitate seamless UAV mobility between GCSs. This model of communication, in turn, questions the locator-based addressing used in IP and instead utilizes a data-centric naming.

In the case of using TCP/IP, mobility of UAVs introduces a significant challenge. Consider the case where a GCS is receiving telemetry information from a specific UAV. Assuming that the UAV moves and changes its point of attachment to the network, it will have to configure a new IP address on its wireless interface. However, this is problematic, as the telemetry information is still being sent by to the previous IP address of the UAV. This simple example illustrates the necessity to deploy mobility management solutions to handle this type of situations.

However, mobility management solutions increase the complexity of the deployment and may impact the performance of data distribution, both in terms of signaling/data overhead and communication path delay. Considering the specific case of multicast data streams, mobility of content producers and consumers is inherently handled by multicast routing protocols, which are able to react to changes of location of mobile nodes by reconstructing the corresponding multicast delivery trees. Nevertheless, this comes with a cost in terms of signaling and data overhead (data may still flow through branches of a multicast delivery tree where there are no receivers while the routing protocol does not converge).

Another alternative is to perform the mobility management of producers and consumers not at the application layer based on IP multicast trees, but on the network layer based on an Information Centric Network approach, which was already mentioned in this section.

Greater flexibility in addressing may help in dealing with mobility more efficiently, e.g., through an augmented semantic that may fulfil the mobility requirements {{?RFC7429}} or through moving from a locator- to a content or service-centric semantic for addressing.

## Communication Across Services {#SEC:service}

As a communication infrastructure spanning many facets of life, the Internet integrates services and resources from various aspects such as remote collaboration, shopping, content production as well as delivery, education, and many more. Accessing those services and resources directly through URIs has been proposed by methods such as those defined in ICN {{?RFC7476}}, where providers of services and resources can advertise those through unified identifiers without additional planning of identifiers and locations for underlying data and their replicas. Users can access required services and resources by virtue of using the URI-based identification, with an ephemeral relationship built between user and provider, while the building of such relationship may be constrained with user- as well as service-specific requirements, such as proximity (finding nearest provider), load (finding fastest provider), and others.

While systems like ICN {{CCN}} provide an alternative to the locator-based addressing of IP, its deployment requires an overlay (over IP) or native deployment (alongside IP), the latter with dedicated gateways needed for translation. Underlay deployments are also envisioned in {{?RFC8763}}, where ICN solutions are being used to facilitate communication between IP addressed network endpoints or URI-based service endpoints, still requiring gateway solutions for interconnection with ICN-based networks as well as IP routing based networks (cf., {{ICN5G}}{{ICNIP}}).

Although various approaches combining service and location-based addressing have been devised, the key challenge here is to facilitate a "natural", i.e., direct communication, without the need for gateways above the network layer.

Another aspect of communication across services is that of chaining individual services to a larger service. Here, an identifier would be used that serves as a link to next hop destination within the chain of single services, as done in the work on Service Function Chaining (SFC). With this, services are identified at the level of Layer 2/3 ({{?RFC7665}}, {{?RFC8754}}, {{?RFC8595}}) or at the level of name-based service identifiers like URLs {{?RFC8677}} although the service chain identification is carried as a Network Service header (NSH) {{?RFC7665}}, separate to the packet identifiers. The forwarding with the chain of services utilizes individual locator-based IP addressing (for L3 chaining) to communicate the chained operations from one Service Function Forwarder {{?RFC7665}} to another, leading to concerns regarding overhead incurred through the stacking of those chained identifiers in terms of packet overhead and therefore efficiency in handling in the intermediary nodes.

Greater flexibility in addressing may allow for incorporating different information, e.g., service as well as chaining semantics, into the overall Internet addressing.


## Communication Traffic Steering {#SEC:steering}

Steering traffic within a communication scenario may involve at least two aspects, namely (i) limiting certain traffic towards a certain set of communication nodes and (ii) constraining the sending of packets towards a given destination (or a chain of destinations) with metrics that would allow the selection among one or more possible destinations.

One possibility for limiting traffic inside limited domains, towards specific objects, e.g., devices, users, or group of them, is subnet partition with techniques such as VLAN {{?RFC5517}}, VxLAN {{?RFC7348}}, or more evolved solution like TeraStream {{TERASTREAM}} realizing such partitioning. Such mechanisms usually involve significant configuration, and even small changes in network and user nodes could result in a repartition and possibly additional configuration efforts. Another key aspect is the complete lack of correlation of the topological address and any likely more semantic-rich identification that could be used to make policy decisions regarding traffic steering. Suitably enriching the semantics of the packet address, either that of the sender or receiver, so that such decision could be made while minimizing the involvement of higher layer mechanisms, is a crucial challenge for improving on network operations and speed of such limited domain traffic.

When making decisions to select one out of a set of possible destinations for a packet, IP anycast semantics can be applied albeit being limited to the locator semantic of the IP address itself. Recent work in {{SFCANYCAST}} suggests utilizing the notion of IP anycast address to encode a "service identifier", which is dynamically mapped onto network locations where service instances fulfilling the service request may be located. Scenarios where this capability may be utilized are provided in {{SFCANYCAST}} and include, but are not limited to, scenarios such as edge-assisted VR/AR, transportation, and digital twins.

The challenge here lies in the possible encoding of not only the service information itself but the constraint information that helps the selection of the "best" service instance and which is likely a service-specific constraint in relation to the particular scenario. The notion of an address here is a conditional (on those constraints) one where this conditional part is an essential aspect of the forwarding action to be taken. It needs therefore consideration in the definition of what an address is, what is its semantic, and how the address structure ought to look like.

As outlined in the previous sub-section, chaining services are another aspect of steering traffic along a chain of constituent services, where the chain is identified through either a stack of individual identifiers, such as in Segment Routing {{?RFC8402}}, or as an identifier that serves as a link to next hop destination within the chain, such as in Service Function Chaining (SFC). The latter can be applied to services identified at the level of Layer 2/3 ({{?RFC7665}}, {{?RFC8754}}, {{?RFC8595}}) or at the level of name-based service identifiers like URLs {{?RFC8677}}. However, the overhead incurred through the stacking of those chained identifiers is a concern in terms of packet overhead and therefore efficiency in handling in the intermediary nodes.

Flexibility in addressing may enable more semantic rich encoding schemes that may help in steering traffic at hardware level and speed, without complex mechanisms usually resulting in handling packets in the slow path of routers.


## Communication with built-in security {#SEC:builtin-sec}

Today, strong security in the Internet is usually implemented as a general network service ({{PILA}}, {{?RFC6158}}). Among the various reasons for such approach is the limited semantic of current IP addresses, which do not allow to natively express security features or trust relationships. Efforts like Cryptographically Generated Addresses (CGA) {{?RFC3972}}, provide some security features by embedding a truncated public key in the last 57-bit of IPv6 address, thereby greatly enhancing authentication and security within an IP network via asymmetric cryptography and IPsec {{?RFC4301}}. The development of the Host Identity Protocol (HIP) {{?RFC7401}} saw the introduction of cryptographic identifiers for the newly introduced Host Identity (HI) to allow for enhanced accountability, and therefore trust. The use of those HIs, however, is limited by the size of IPv6 128bit addresses.

Through a greater flexibility in addressing, any security-related key, certificate, or identifier could instead be included in a suitable address structure without any information loss (i.e., as-is, without any truncation or operation as such), avoiding therefore compromises such as those in HIP. Instead, CGAs could be created using full length certificates, or being able to support larger HIP addresses in a limited domain that uses it. This could significantly help in constructing a trusted and secure communication at the network layer, leading to connections that could be considered as absolute secure (assuming the cryptography involved is secure). Even more, anti-abuse mechanisms and/or DDoS protection mechanisms like the one under discussion in PEARG ({{PEARG}}) Research Group may leverage a greater flexibility of the overall Internet addressing, if provided, in order to be more effective.


## Communication in Alternative Forwarding Architectures {#SEC:nin}

The performance of communication networks has long been a focus for optimization due to the immediate impact on cost of ownership for communication service providers. Technologies like MPLS {{?RFC3031}} have been introduced to optimize lower layer communication, e.g., by mapping L3 traffic into aggregated labels of forwarding traffic for the purposes of, e.g., traffic engineering.

Even further, other works have emerged in recent years that have replaced the notion of packets with other concepts for the same purpose of improved traffic engineering and therefore efficiency gains. One such area is that of Software Defined Networks (SDN) {{?RFC7426}}, which has highlighted how a majority of Internet traffic is better identified by flows, rather than packets. Based on such observation, alternate forwarding architectures have been devised that are flow-based or path-based. With this approach, all data belonging to the same traffic stream is delivered over the same path, and traffic flows are identified by some connection or path identifier rather than by complete routing information, possibly enabling fast hardware based switching.

On the one hand, such a communication model may be more suitable for real-time traffic like in the context of Deterministic Networks ({{DETNET}}), where indeed a lot of work has focused on how to "identify" packets belonging to the same DETNET flow in order to jointly manage the forwarding within the desired deterministic boundaries.

On the other hand, it may improve the communication efficiency in constrained wireless environments (cf., {{SEC:constrained}}), by reducing the overhead, hence increasing the number of useful bits per second per Hz.

Also, the delivery of information across similar flows may be combined into a multipoint delivery of a single return flow, e.g., for scenarios of requests for a video chunk from many clients being responded to with a single (multi-destination) flow, as outlined in {{BIER-MC}} as an example. Another opportunity to improve communication efficiency is being pursued in ongoing IETF/IRTF work to deliver IP- or HTTP-level packets directly over path-based or flow-based transport network solutions, such as in {{TROSSEN}}{{BIER-MC}}{{ICNIP}}{{ICN5G}} with the capability to bundle unicast forward communication streams flexibly together in return path multipoint relations. Such capability is particularly opportune in scenarios such as chunk-based video retrieval or distributed data storage. However, those solutions currently require gateways to "translate" the flow communication into the packet-level addressing semantic in the peering IP networks. Furthermore, the use of those alternative forwarding mechanisms often require the encapsulation of Internet addressing information, leading to wastage of bandwidth as well as processing resources.

Providing an alternative way of forwarding data has also been the motivation for the efforts created in the European Telecommunication Standards Institute (ETSI), which formed a Industry Specification Group (ISG) named Non-IP Networking (NIN) {{ETSI-NIN}}. This group sets out to develop and standardize a set of protocols leveraging an alternative forwarding architecture, such as provided by a flow-based switching paradigm. The deployment of such protocols may be seen to form limited domains, still leaving the need to interoperate with the (packet-based forwarding) Internet; a situation possibly enabled through a greater flexibility of the addressing used across Internet-based and alternative limited domains alike.

As an alternative to IP routing, EIBP (Extended Internet Bypass Protocol) {{EIBP}} offers a communications model that can work with IP in parallel and entirely transparent and independent to any operation at network layer. For this, EIBP proposes the use of physical and/or virtual structures in networks and among networks to auto assign routable addresses that capture the relative position of routers in a network or networks in a connected set of networks, which can be used to route the packets between end domains. EIBP operates at Layer 2.5 and provides encapsulation (at source domain), routing, and de-encapsulation (at destination domain) for packets. EIBP can forward any type of packets between domains. A resolver to map the domain ID to EIBP’s edge router addresses is required. When queried for a specific domain, the resolver will return the corresponding edge router structured addresses.

EIBP decouples routing operations from end domain operations, offering to serve any domain, without point solutions to specific domains. EIBP also decouples routing IDs or addresses from end device/domain addresses. This allows for accommodation of new and upcoming domains. A domain can extend EIBP’s structured addresses into the domain, by joining as a nested domain under one or more edge routers, or by extending the edge router’s structure addresses to its devices.  

A greater flexibility in addressing semantics may reduce the aforementioned wastage by accommodating Internet addressing in the light of such alternative forwarding architectures, instead enabling the direct use of the alternative forwarding information.


# Issues in Addressing {#SEC:problem}

There are a number of issues that we can identify from the communication scenarios in {{SEC:cases}}, not claiming to be exhaustive in our list:

1. Limiting Alternative Address Semantics: Several communication scenarios pursue the use of alternative semantics of what constitute an 'address' of a packet traversing the Internet, which may fall foul of the defined network interface semantic of IP addresses.

2. Hampering Security: Aligning with the semantic and length limitations of IP addressing may hamper the security objectives of any new semantic, possibly leading to detrimental effects and possible other workarounds (at the risk of introducing fragility rather than security).

3. Complicating Traffic Engineering: Utilizing a plethora of non-address inputs into the traffic steering decision in real networks complicates traffic engineering in that it makes the development of suitable policies more complex, while also leading to possible contention between methods being used.

4. Hampering Efficiency: Extending IP addressing through point-wise solutions also hampers efficiency, e.g., through needed re-encapsulation (therefore increasing the header processing overhead as well as header-to-payload ratio), through introducing path stretch, or through requiring compression techniques to reduce the header proportion of large addresses when operating in constrained environments.

5. Fragility: The introduction of point solutions, each of which comes with possibly own usages of address or packet fields, together with extension-specific operations, increases the overall fragility of the resulting system, caused, for instance, through contention between feature extensions that were neither foreseen in the design nor tested during the implementation phase.

6. Extensibility: Accommodating new requirements through ever new extensions as an extensibility approach to addressing compounds aspects discussed before, i.e., fragility, efficiency etc. It complicates engineering due to the clearly missing boundaries against which contentions with other extensions could be managed. It complicates standardization since extension-based extensibility requires independent, and often lengthy, standardization processes. And ultimately, deployments are complicated due to backward compatibility testing required for any new extension being integrated into the deployed system.

The table below shows how the above identified issues do arise somehow in our outlined communication scenarios in {{SEC:cases}}.
This overview will be deepened in more details in the gap analysis document {{I-D.jia-intarea-internet-addressing-gap-analysis}}.


|                                      | Issue 1 | Issue 2 | Issue 3 | Issue 4 | Issue 5 | Issue 6 |
| ------------------------------------ | ------- | ------- | ------- | ------- | ------- | ------- |
| Constrained Environments             |         |         |         | x       | x       | x       |
| Dynamically Changing Topologies      | x       |         | x       | x       | x       | x       |
| Moving Endpoints                     | x       |         | x       | x       | x       | x       |
| Across Services                      | x       |         | x       | x       | x       | x       |
| Traffic Steering                     | x       |         | x       | x       | x       | x       |
| Built-in Security                    | x       | x       |         | x       | x       | x       |
| Alternative Forwarding Architectures | x       |         |         | x       |         | x       |
{: #mapping title="Issues Involved in Challenging Scenarios"}


# Problem Statement


This document identifies a number of scenarios that position the existing Internet addressing structure itself as a potential hinderance in solving key problems for Internet service provisioning. Such problems include supporting new, e.g., service-oriented, scenarios more efficiently, with improved security and efficient traffic engineering, as well as large scale mobility. We can observe that those new forms of communication are particularly driven by the conceptual framework of limited domains, realizing the requirements of stakeholders for an optimized communication in those limited domains, while still utilizing the Internet for interconnection as well as for access to the wealth of existing Internet services.


This co-existence of optimized LD-level as well as Internet communication creates a tussle between those requirements on addressing stemming from those limited domains and those coming from the Internet in the form of agreed IPv6 semantics. This tussle directly refers back to our introductory question on flexibility in addressing (or leaving the problem to limited domain solutions to deal with).

At this stage, this document, does not provide a definite answer nor does propose or promote specific solutions to the problems here portrayed. Instead, this document aims at stimulating discussion on the emerging needs for addressing with the possibility to fundamentally re-think the addressing in the Internet beyond the current objectives of IPv6 in order to provide the flexibility to suitably support the many new forms of communication that will emerge.

To complement the problem statement in this document, the companion gap analysis document {{I-D.jia-intarea-internet-addressing-gap-analysis}} deepens the issues identified in {{SEC:problem}} along key properties of today's Internet addressing.

# Security Considerations {#SEC:sec}

The present memo does not introduce any new technology and/or mechanism and as such does not introduce any security threat to the TCP/IP protocol suite.

Nevertheless, it is worth to observe whether or not greater flexibility of addressing (as suggested in previous sections) would allow to introduce fully featured security in endpoint identification, potentially able to eradicate the spoofing problem, as one example. Furthermore, it may be used to include application gateways' certificates in order to provide more efficiency, e.g., using web certificates also in the addressing of web services. While increasing security, privacy protection may also be improved.

# IANA Considerations {#SEC:iana}

This document does not include an IANA request.


--- back

# Change Log

**NOTES**: Please remove this section prior to publication of a final version of this document.

## Since draft-jia-intarea-scenarios-problems-addressing-01

* TBD

## Since draft-jia-intarea-scenarios-problems-addressing-00

* Simplify the 'issues' section with simpler bullet list.
* Several editorial changes to create a clear link with the gap analysis.
* Added issues and scenarios mapping Table.



# Acknowledgments
{:numbered="false"}

Thanks to Stewart Bryant for useful conversations.
Ron Bonica, Toerless Eckert and Brian E. Carpenter made helpful suggestions.

---
coding: utf-8

title: "Use Cases and Problems in Internet Addressing"
abbrev: UC PS Internet Addressing
docname: draft-jia-use-cases-problems-internet-addressing
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
    role: editor
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
    role: editor
    street: WRITEME
    city: WRITEME
    country: WRITEME
    code: 'WRITEME'
    email: dirk.trossen@huawei.com
-
    ins: L. Iannone
    name: Luigi Iannone
    org: Huawei Technologies France S.A.S.U.
    abbrev: Huawei
    role: editor
    street: 18, Quai du Point du Jour
    city: Boulogne-Billancourt
    country: France
    code: '92100'
    email: luigi.iannone@huawei.com

normative:
    # RFCxxxx: if we cite as {{!RFCxxxx}} (rather than {{RFCxxxx}}), then we do not need to declare it here :D

informative:
    # RFCxxxx: if we cite as {{?RFCxxxx}} (rather than {{RFCxxxx}}), then we do not need to declare it here :D
    I-D.ietf-lisp-nexagon:
    I-D.ietf-lisp-introduction:
    I-D.ietf-lisp-mn:
    I-D.ietf-intarea-gue:
    I-D.quic-transport34:
    ANYCAST: DOI.10.1145/3230543.3230547
    https://doi.org/10.1371/journal.pone.0246293
    I-D.geng-rtgwg-cfn-dyncast-ps-usecase: dyncast   # use newer draft "draft-liu-dyncast-ps-usecases"
    LR-WPAN:
        title: IEEE 802.15.4 - IEEE Standard for Low-Rate Wireless Networks
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
        target: https://www.bluetooth.com/specifications/
    OCADO:
        title: Ocado Technology’s robot warehouse a Hive of IoT innovation
        seriesinfo: Tech Monitor
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
    SPHINX:
      	title: Sphinx - A compact and provably secure mix format
      	author:
        -
            ins: G. Danezis
        -
            ins: I. Goldberg
		seriesinfo:
			IEEE: 30th Symposium on Security and Privacy, pages 269-282
		date: 2009-05
    ICN5G: 
		title: Enabling ICN in 3GPP's 5G NextGen Core Architecture
		author: Ravindran, R., Suthar, P., Trossen, D., Wang, C., White, G., 
		target: https://www.ietf.org/archive/id/draft-irtf-icnrg-5gc-icn-04, (work in progress)
		date: 2021-01
    ICNIP:
		title: Internet Services over ICN in 5G LAN Environments
		author: D. Trossen, S. Robitzsch, M. Reed, M. Al-Naday, J. Riihijarvi, 
		target: https://tools.ietf.org/html/draft-trossen-icnrg-internet-icn-5glan-04, (work in progress)
        date: 2021-01
    HANDLEY:
        title: "Delay is Not an Option: Low Latency Routing in Space"
        author: M. Handley
        target: In Proceedings of the 17th ACM Workshop on Hot Topics in Networks (HotNets ’18). Association for Computing Machinery, New York, NY, USA, 85–91., 
        date: 2018
    BIER-MC:
        title: Applicability of BIER Multicast Overlay for Adaptive Streaming Services
        author: 
        -
            ins: D. Trossen
        - 
            ins: A. Rahman
        -
            ins: C. Wang
        -
            ins: T. Eckert
        target: https://tools.ietf.org/html/draft-ietf-bier-multicast-http-response-05, (work in progress), 
        date: 2021-01
    MANET1:
        title: Randomized geographic-based routing with nearly guaranteed delivery for three-dimensional ad hoc network
        author:
        -
            ins: Alaa E. Abdallah
        -
            ins: Emad E. Abdallah
        -
            ins: Mohammad Bsoul
        author:
        -
            ins: Ahmed Fawzi Otoom
        target: https://doi.org/10.1177/1550147716671255
        date: 2016-10
    CARTESIAN:
        title:  Routing and Addressing Problems in Large Metropolitan-Scale Internetworks
        author: G. Finn
        target: University of Southern California, ISI/RR-87-180
        date: March 1987
    HICN: 
        title: Hybrid Information-Centric Networking: ICN inside the Internet Protocol
        author: Muscariello, L., et al
        target: ICNRG Interim Meeting, <https://datatracker.ietf.org/meeting/interim-2018-icnrg-01/materials/slides-interim-2018-icnrg-01-sessa-hybrid-icn-hicn-luca-muscariello>.
        date: March 2018
    CCN: 
        title: Networking Named Content
        author: Jacobson, V., et al.
        target: Proceedings of the 5th international conference on Emerging networking experiments and technologies (CoNEXT'09), DOI 10.1145/1658939.1658941, <https://doi.org/10.1145/1658939.1658941>
        date: December 2009
    TROSSEN:
        title: Arguments for an information-centric internetworking architecture
        author:
        -
            ins: D. Trossen
        -
            ins: M. Sarela
        -
            ins: K. Sollins
        target: ACM SIGCOMM Computer Communication Review Vol. 40 Issue 2
        date: April 2010
    REED:
        title: Stateless multicast switching in software defined networks
        author:
        -
            ins: M. J. Reed
        -
            ins: M. Al-Naday
        -
            ins: N. Thomos
        - 
            ins: D. Trossen
        -
            ins: G. Petropoulos
        -
            ins: S. Spirou
        target: ICC 2016, Kuala Lumpur, Maylaysia
        date: 2016
     ADDRLESS: 
		title: Addressless - A new internet server model to prevent network scanning
		author: Shanshan Hao, Renjie Liu, Zhe Weng, Deliang Chang, Congxiao Bao, Xing Li 
		target: https://doi.org/10.1371/journal.pone.0246293
		date: 2021-02
    entity:
        SELF: "[RFCXXXX]"



--- abstract

Although RFC8799 {{?RFC8799}} recognizes "limited domains" as exhibiting domain-specific requirements as well as communication behaviors and semantics, the topological location defined in the IP address structure requires the mapping of those domain-specific concepts onto that single address structure, used across what makes up the Internet as a whole at the networking layer.

This document describes well-recognized use-cases that exhibit possibly different addressing requirements with the intention to outline gaps in existing solutions, as well as requirements for a flexible address structure that could be used instead of the fixed address structure of current IP.

<!-- Yihao: 
text in abstract is a little bit tight and complex
After we finish the doc body, we then back to abstract to make it easier to read and understand 
-->

--- middle


# Introduction {#SEC:intro}

<!-- 
not portraying IP as being bad, but as possible to evolve to make it better 
-->

The Internet Protocol (IP), positioned as the unified protocol at the (Internet) network layer, is seen by many as key to the innovation stemming from Internet-based applications and services. Even more so, with the success of TCP/IP protocol stack, IP has been gradually replacing existing domain-specific protocols, evolving into the core protocol of the entire communication system. At its inception roughly 40 years ago {{!RFC791}}, the Internet's addressing system, represented in the form of the IP address and its locator-based semantics, has brought the notion of a 'common addressing for all communication' as a major advance over proprietary technology-specific solutions to ensure end-to-end communication from any device connected to the Internet to another.  

However, use cases, associated service and node behaviors as well as requirements on packet delivery have since extended significantly, with Internet technologies being developed to accommodate them with the given framework of addressing that stood at the beginning of the Internet's development. This evolution is reflected in the concept of the "Limited domain", first introduced in {{?RFC8799}}. It refers to a single physical network, attached to or running in parallel with the Internet, or is defined by set of users and nodes distributed over a much wider area, but drawn together by a single virtual network over the Internet. Key to a limited domain is that requirements, behaviors, and semantics could be noticeable local and, more importantly, specific to the limited domain. Very often, the realization of a limited domain is defined by specific communication scenario(s) that exhibit the domain-specific behaviors and pose the requirements that lead to the establishment of the limited domain.

One key architectural aspect when communicating within limited domains is that of addressing and, therefore, the address structure, as well as the semantic that is being used for the routing of packets within such limited domains. The topological location centricity of IP is fundamental when reconciling the often differing semantics for 'addressing' that can be found in those limited domains. The result of this fundamental role of the single IP addressing is that limited domains have to adopt specific solutions, e.g., translating/mapping/converting concepts, semantics, and ultimately, domain-specific addressing into the common IP addressing used across limited domains.


<!-- Yihao: 

Here we have a clear notion of "flexible addressing" and a question to discuss, but avoid "address structure". However, "address structure" is still already mentioned in "...therefore, the address structure, as well as.." before. So I guess people could be confused that - will the term "flexible addressing" change the IP(v6) address structure? As we mentioned in Q&A - FA can be achieved in many ways, one of which is a single albeit flexible addressing structure. So for better understanding, I suggest that we have a sentence here to clearly include this answer. 

-->

This document advocates the notion of "flexible addressing" as a concept to accommodate limited domain specific semantics in a single holistic albeit flexible addressing scheme able to reduce, or even entirely remove, the need for aligning the address semantics of different limited domains, like for instance the current topological location semantic of the Internet. Ultimately, such flexible addressing could be beneficial to those communication scenarios realized within the limited domain, e.g., in the form of improved efficiency, removing of constraints imposed by needing to utilize the limited semantics of IP addressing, and/or others. 

<!-- Yihao
Similar question as the last comment: people may still be curious/confuse about the scope of the "flexible" in " addressing"?
For most of people, they maybe have a stereotype that IPv6 addressing is flexible (compared to IPv4), and the CGA is a good example of the flexible addressing of IPv6.

Dirk: sure, we have those in the scenarios and gap analysis later. So IPv6 does afford flexibility but also sets constraints, which must come out of the gap analysis. 

Luigi: Agreed. The gap analysis should highlight this point.

Yihao: Shall we put a sentence somewhere in the intro first, saying "IPv6 do provide some flexibility, but not enough". This may relax people who are expert or staunch supporter of IPv6. 
-->

In other words, this document revolves around the following question:

> "Should limited domains purely rely on IP addresses and therefore deal with the complexity of translating any semantic mismatch themselves, or should a more flexible addressing support those limited domains?"

For this, this document describes well-recognized scenarios in limited domains that can benefit from flexible addressing and analyses problems encountered throughout these scenarios. The purpose of this draft is thus to stimulate discussion on the emerging needs for addressing at large with the possibility to fundamentally re-think the addressing in the Interrnet beyond the current objectives of IPv6.

<!-- LUIGI: Tentative paragraph to related to the RRG effort == PLEASE REVIEW == -->
It is important to remark that any change in the addressing, hence at the data plane level, leads to changes and challenges on the cotnrol plane level, i.e., routing. The latter is an even harder problem than just addressing and might need more research efforts that are not the objective of this document, which focuses solely on the data plane. 

<!-- NOTE: Yihao
confusion: flexible addressing - flexible address structure? [LUIGI] I would suggest we use "flexible addressing" everywhere.
AP: Dirk to correct intro with proposition to use flexible address structure as possible alternative [DONE]

confusion: scenarios - limited domains
AP: Dirk to make relation between scenario and limited domain clearer [Added a sentence above on limited domains realized as a consequence of requirements and behaviours stemming from use cases.]
-->




<!-- BACKUP
Information documents usually do not use RFC 2119 terminology.
We can put it back if necessary.

# Conventional Terminology {#SEC:term}
The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in BCP 14 RFC2119 RFC8174 when, and only when, they appear in all capitals, as shown here.
-->




<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->



<!-- Dirk: I suggest renaming this section from 'use cases' to the proposed one below. This is to (a) better capture the link to limited domains and (b) don't present what we have as use cases since I'm not sure this is even the right word 
Luigi: OK for me. I replaced a couple of "use cases" recurrences in the Intro with "Communication scenarios" so that the reader will understand the new title.
-->

# Communication Scenarios in Limited Domains {#SEC:cases}


<!--NOTES: Dirk
I suggest focussing the use cases on various aspects of 'communication' at large, which includes many things, but then honing into the addressing impact of that 'communication'.
Yihao: agree
-->

<!--NOTES: Yihao

-->

The following sub-section outlines a number of scenarios, all of which belong to the concept of "limited domains" {{?RFC8799}}. While a list of use cases may be long, this document focussed use cases on a number of aspects that we can observe in those limited domains, captured in the sub-section titles. For each use case, we point at possible challenges, which we will pick upon in Section {{SEC:problem}} when describing more formally the shortcomings exisitng in current Internet addressing.


## Communication in Constrained Environments {#SEC:constrained}

In a number of communication scenarios, such as those encountered in the Internet of Things (IoT),
a simple, low-cost communication network is required, and there are limitations for network devices in computational power, memory, and energy availability.
In addition to IEEE 802.15.4, i.e., Low-Rate Wireless Personal Area Network {{LR-WPAN}}, several limited domains exists through utilizing link layer technologies such as Bluetooth Low Energy (BLE) {{BLE}}, Digital European Cordless Telecommunications (DECT) - Ultra Low Energy (ULE) {{DECT-ULE}}, Master-Slave/Token-Passing (MS/TP) {{BACnet}}, Near-Field-Communication (NFC) {{ECMA-340}}, and Power Line Communication (PLC) {{IEEE_1901.1}}.
Generally, a group of IoT network devices form a constrained node network at the edge, and IoT terminals connect to these network devices for data transmission.
This type of networks and IoT devices in the network require as little computational power as possible, smaller memory requirements, better energy availability to reduce the total cost of ownership of the network.
Furthermore, in the context of industrial IoT, real-time requirements and scalability make IP technology not naturally suitable as communication technology ({{OCADO}}).

<!-- [Yihao] 

Maybe we can have below references somewhere in the document, if appropriate.

- RFC 5826 (Home Automation Routing Requirements in Low-Power and Lossy Networks)
    - All other proposed references show a new header to be used for underlay/overlay/translation of IPv6. As such May be is better to use RFC 8138 since 5826 does not propose any header adaptation.  
    - good suggestion.
- RFC 8105 (Transmission of IPv6 Packets over Digital Enhanced Cordless Telecommunications (DECT) Ultra Low Energy (ULE))
    - OK
- RFC 8163 (Transmission of IPv6 over Master-Slave/Token-Passing (MS/TP) Networks)
    - OK
- draft-ietf-6lo-nfc-17 (Transmission of IPv6 Packets over Near Field Communication)
    - OK
- draft-ietf-6lo-plc-05 (Transmission of IPv6 Packets over PLC Networks)
    - OK
And please correct me if the these references/specifications are not appropriate (I am not familiar with the layer-2 specifications).
AP: Luigi to double check
Done: Suggested one change.

Yihao: any change to the references of these layer-2 specification. That the stuff I mean to check.
-->


<!-- Yihao: "allowing IoT devices using multiple communication technologies" -change to-> "... with different wireless/radio technologies..." (the term "communication" could be confused due to the name of the sub-section. I suggest we avoid "communication" if it is not in the name of the sub-section) 
Luigi: IMO, just keep using communication is fine since it makes the content coherent with the title.
-->

The end-to-end principle (detailed in {{?RFC2775}}) requires Internet protocols (e.g., IPv6 {{?RFC8200}}) to run on such constrained node networks, allowing IoT devices using multiple communication technologies to talk on the Internet.
Often, devices located on the edge of constrained networks act as gateway devices, usually performing header compression ({{?RFC4919}}).
To ensure security and reliability, multiple gateways must be deployed. IoT devices on the network can easily select one of gateways for traffic passthrough by the devices on the (limited domain) network.


<!-- Yihao: 
1. as we mentioned RFC4919 just in last paragraph, is it still appropriate to say that a 128-bit IPv6 will be challenge? 
2. readers may not have clear answers about why flexible addressing could help this? is it refers to short address?
-->

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

<!-- NOTES: Add flexible addressing paragraph, i.e., how FA may be useful here
AP: Luigi [DONE] 
--->
A flexible addressing scheme may allow avoiding complex and energy hungry operations, like header compression and fragmentation, necessary to translate protocol headers from one limited domain to another.


## Communication within Dynamically Changing Topologies {#SEC:dynamic}

Communication may occur over networks that exhibit dynamically changing topologies. One such example is that of satellite networks, providing global Internet connections through a combination of inter-satellite and ground station communication.
With the convergence of space-based and terrestrial networks, users can experience seamless broadband access, e.g., on cruise ships, flights, and within cars, often complemented by and seamlessly switching between Wi-Fi, cellular, or satellite based networks at any time.
The satellite network service provider will plan the transmission path of user traffic based on the network coverage, satellite orbit, route, and link load, providing potentially high-quality Internet connections for users in areas that are not, or hard to be, covered by terrestrial networks. The involved topologies of the satellite network will be changing constantly while observing a regular flight pattern in relation to other satellite and predictable overflight patterns to ground users.

Another example is that of vehicular communication, where services may be accessed across vehicles, such as self-driving cars, for the purpose of collaborative objection recognition (e.g., for collision avoidance), road status conveyance (e.g., for pre-warning of road-ahead conditions) and other purposes. Communication may include RoadSide Units (RSU) with the possibility to create ephemeral connections to those RSUs for the purpose of workload offloading, joint computation over multiple (vehicular) inputs and other purposes {{I-D.ietf-lisp-nexagon}}. Communication here may exhibit a multi-hop nature, not just involving the vehicle and the RSU over a direct link. Those topologies are naturally changing constantly due to the dynamic nature of the involved communication nodes.

In both network technologies, there is a significant difference between the high dynamics of the underlying network topologies, compared to the relative static nature of terrestrial network topology, as reported in {{HANDLEY}}. As a consequence, the notion of a topological network location becomes restrictive in the sense that not only the relation between network nodes and user endpoint may change, but also the relation between the nodes that form the network itself. This may lead to the challenge of maintaining and updating the topological addresses in this constantly changing network topology.

In attempts to utilize entirely different semantics for the addressing itself, georgraphic-based routing, such as in {{CARTISEAN}}, has been proposed for MANETs (mobile ad-hoc networks) through providing geographic coordinates based addresses to achieve better routing performance, lower overhaead, and lower latency {{MANET1}}.


<!-- Yihao: 
same question: readers may have no idea why flexible addressing could help?
Maybe for each of the sub-section/use case, we can have at least one clear sentence that explicitly says why flexible addressing could help. 
 -->

 <!-- NOTES: Add flexible addressing paragraph, i.e., how FA may be useful here
AP: Dirk
NOTES: Dirk: I have real trouble to outline how FA may be useful here without having addressed the gaps of solutions since it's mostly about either removing those gaps or stay very high level, namely "accommodating the limited domain semantic in a single (flexible) addressing structure", which is too generic as a statement and we have said as much already in the introduction.

NOTE: Luigi: I start to wonder whether the FA benefits shuld be in the gap analysis. Because for each use case, in the gap analysis first we state what is the gap then what FA brings .... this will make the link with the requirements part... To Be Discussed at our next meeting.
-->

Flexible addressing here would allow for accommodating such geographic address semantic in a single (flexible) addressing structure.


## Communication among Moving Endpoints {#SEC:mobility} 

<!-- NOTE Luigi: This Section was initially suggested to be between steering ans security, however, becasue the topic is close to :changing topology" I put it here. Not sure whether or not we should actually merge it to the previous.
Even more, because this section refers to protocols presented in other sections we might consider putting both section after the alternative forwarding section.

Yihao: Putting this section behind "changing topology" is a good choice. But still, I recommend that we put the "changing topology" as the second sub-section since geo-based address and forward looks a strong scenarios for us.
While for alternative forwarding architecture, I would suggest that we focus on the real use cases (reasons) for a alternative forwarding architecture, rather than saying Communication with alternative forwarding architecture.

Dirk: I suggest keeping the 'alternative forwarding architecture'. In the other sections, we address the 'aspect' of communication, e.g., changing topology, mobility, ..., not the use cases either. The use case for the sat aspect in 'changing topologies' is plain Internet access, so not particularly 'out there'. Further, the introduction of SDN was not just, if at all, motivated by better handling of streaming scenarios; nor for NIN. Hence, I'd leave it as is.

Dirk: reviewed this section with minor corrections
-->

When packet switching has been first introduced, back in the 60s/70s, it was supposed to replace the rigid circuit switching with a communication infrastructure that was more resilient to failures. As such, the design never really considered communication endpoints as mobile. Even in the pioneering ALOHA {{ALOHA}} system, despite considering wireless and satellite links, the network was considered static (with the exception of failures and satellites, which fall in what is discussed in {SEC:dynamic}). Ever since, a lot of efforts have been devoted to overcome such limitation once that it became clear that endpoint mobility will become a main (if not THE main) characteristic of ubiquitous communication systems.

The IETF has for a long time worked on solutions that would allow to extend the IP layer with mobility support. Because of the topological semantic of IP addresses, endpoints need to change addresses each time they visit a different network. However, because routing and endpoint identification is also IP address based, this leads to a communication disruption.

To cope with such a situation, anchor-based Mobile IP mechanisms have been introduced ({{?RFC5177}}, {{?RFC6626}} {{?RFC5944}}, {{?RFC5275}}). Mobile IP is based on a relatively complex and heavy mechanism that makes it hard to deploy and not very effient. Furthermore, it is even less suitable than native IP in constrained enviromments like the ones discussed in {SEC:constrained}.      

Alternative approaches to Mobile IP often leverage the introduction of some form of overlay. LISP {{?I-D.ietf-lisp-introduction}}, by separating the topological semantic from the identification semantic of IP addresses, is able to cope with endpoint mobility by dynamically mapping endpoint identifiers with routing locators {{I-D.ietf-lisp-mn}}. This comes at the price of an overlay that needs its own additional control plane {{I-D.ietf-lisp-6833bis}}. Similarly, the NVO3 (Network Virtualization Overlays) Working Group, while focusing on Data Center Environments, also explored an overlay-based solution for multi-tenancy purposes, but also resilient to mobility since relocating Virtual Machines (VMs) is common pratice. NVO3 considered for a long time several data planes that implement slightly different flavors of overlays ({{?RFC8926}}, {{?RFC7348}}, {{I-D.ietf-intarea-gue}}), but lack of an efficient control-plane specifically tailored for DCs.     

Alternative mobility architectures have also been proposed in order to cope with endpoint mobility outside the IP layer itself. The Host Identity Protocol (HIP) {{?RFC7401}} introduced a new namespace in order to idenfiy endpoints, namely the Host Identity (HI), while leveraging the IP layer for topological location. On the one hand, such an approach needs revising the way applications interact with the network layer, needing to modifying the DNS (now returning a HI instead of an IP address) as well as modified applications using HIP socket extension. On the other hand, early adopters do not necessarily gain any benefit unless all communicating endpoints upgrade to use HIP. However, such solution may work in the context of a limited domain.

Another alternative approach is adopted by Information-Centric Networking (ICN) {{?RFC7476}}. By making content a first class citizen of the communication architecture, the "what" rather then the "where" becomes the real focus of the communication. However, as explained in the next sub-section, ICN can run either over the IP layer or completely replace it, which in turns can be seen as running the Internet and ICN as logically completely separated limited domains.      

Sometimes, also the transport layer gets involed in mobility solutions, either by introducing explicit in-band signaling to allow for communicating IP address changes (e.g., in SCTP {{?RFC5061}} and MPTCP {{?RFC6182}}), or by introducing some form of connection ID that allows for identifying a communication independently from IP addresses (e.g., the connection ID used in QUIC {{I-D.quic-transport34}}).

Flexible addressing may help in finding a final solution to the mobility issue through augemented semantic that may fufill the mobility requirements {{?RFC7429}}.


## Communication Across Services {#SEC:service}

As a communication infrastructure spanning many facets of life, the Internet integrates services and resources from various aspects such as remote collaboration, shopping, content production as well as delivery, education and many more. Accessing those services and resources directly through URIs has been proposed by methods such as those defined in ICN {{?RFC7476}}, where providers of services and resources can advertise those through unified identifiers without additional planning of identifiers and locations for underlying data and their replicas. Users can access required services and resources by virtue of using the URI-based identification, with an ephemeral relationship built between user and provider, while the building of such relationship may be constrained with user- as well as service-specific requirements, such as proximity (finding nearest provider), load (finding fastest provider), and others.

While systems like ICN provide an alternative to the locator-based addressing of IP, its deployment requires an overlay (over IP) or native deployment (alongside IP), the latter with dedicated gateways needed for translation. Underlay deployments are also envisioned in {{?RFC8763}}, where ICN solutions are being used to facilitate communication between IP addressed network endpoints or URI-based service endpoints, still requiring gateway solutions for interconnection with ICN-based networks as well as IP routing based networks (see {{ICN5G}}{{ICNIP}}).

Although various approaches to combining service and location-based addressing have been devised, the key challenge here is to facilitate a "natural", i.e., direct communication without the need for gateways above the network layer.


<!-- Yihao: 
this section is repeated with the last paragraph of the next sub-section 
SFC is described in both "Communication Across Services" and "Steering Communication Traffic". 
Shall we rephrase it in order to have a storyline for it?
-->


Another aspect of communication across services is that of chaining individual services to a larger service. Here, an identifier could be used that serves as a link to next hop destination within the chain of individual services, as done in the work on Service Function Chaining (SFC). With this, services are identified at the level of Layer 2/3 ({{?RFC7665}}, {{?RFC8754}}, {{?RFC8595}}) or at the level of name-based service identifiers like URLs {{?RFC8677}} although the service chain identification is carried as an NSH header ({{?RFC7665}} separate to the packet identifiers. The forwarding with the chain of services utilizes individual locator-based IP addressing (for L3 chaining) to communicate the chained operations from one Service Function Forwarder {{?RFC7665}} to another, leading to concerns regarding overhead incurred through the stacking of those chained identifiers in terms of packet overhead and therefore efficiency in handling in the intermediary nodes. 


<!-- NOTES: Dirk
Reference to RFC8763 but also ongoing IP-over-NDN as well as the ongoing Internet-over-ICN draft in ICNRG? -> ADDED!

AP: Add some text about SFC regarding communication across service endpoint, i.e., SFC (Dirk) [DONE]
AP: Dirk: change text some more to not look like C&P [DONE]
-->

<!-- NOTES: Add flexible addressing paragraph, i.e., how FA may be useful here
AP: Dirk 
--->

Flexible addressing may allow for incorporating different information, e.g., service as well as chaining semantics, into a single addressing structure.


## Steering Communication Traffic {#SEC:steering}

Steering traffic within a communication scenario may involve at least two aspects, namely (i) limiting certain traffic towards a certain set of communication nodes and (ii) constraining the sending of packets towards a given destination (or a chain of destinations) with metrics that would allow the selection among one or more possible destinations.

One possibility for limiting traffic inside limited domains, towards specific objects, e.g., devices, users, or group of them, is subnet partition with techniques such as VLAN {{?RFC5517}}, VxLAN {{?RFC7348}}, or more evolved solution like Terastream {{TERASTREAM}} realizing such partitioning. Such mechanisms usually involve quite some configuration, and even small changes in network and user nodes could result in a repartition and possibly even more configuration efforts. Another key aspect is the complete lack of correlation of the topological address and any likely more semantic-rich identification that could be used to make policy decision regarding traffic steering. Suitably enriching the semantics of the packet address, either that of the sender or receiver, so that such decision could be made while minimizing the involvement of higher layer mechanisms, is a crucial challenge for improving on network operations and speed of such limited domain traffic.

When making decisions to select one out of a set of possible destinations for a packet, IP anycast semantics can be applied albeit being limited to the locator semantic of the IP address itself. Recent work in {{-dyncast}} suggests utilizing the notion of IP anycast address to encode a "service identifier", which is dynamically mapped onto network locations where service instances fulfilling the service request may be located.
Scenarios where this capability may be utilized are provided in {{-dyncast}} and include, but are not limited to, scenarios such as edge-assisted VR/AR, transportation and digital twins.

The challenge here lies in the possible encoding of not only the service information itself but the constraint information that helps the selection of the "best" service instance and which is likely a service-specific constraint in relation to the particular scenario. The notion of an address here is a conditional (on those constraints) one where this conditional part is an essential aspect of the forwarding action to be taken. It needs therefore consideration in the definition of what an address is, what is its semantic, and how the address structure ought to look like.

As outlined in the previous sub-section, chaining services is another aspect of steering traffic along a chain of constituent services, where the chain is identified through either a stack of individual identifiers, such as in Segment Routing {{?RFC8402}}, or as an identifier that serves as a link to next hop destination within the chain, such as in Service Function Chaining (SFC). The latter can be applied to services identified at the level of Layer 2/3 ({{?RFC7665}}, {{?RFC8754}}, {{?RFC8595}}) or at the level of name-based service identifiers like URLs {{?RFC8677}}. However, the overhead incurred through the stacking of those chained identifiers is a concern in terms of packet overhead and therefore efficiency in handling in the intermediary nodes. 


<!-- NOTES: Dirk
What other references?
-->

<!-- NOTES: Yihao
Shall we put MPLS, SRv6 in here/gap analysis? [LUIGI: added as layer2 and layer 3 SFC encapsulation]
AP: add references also here but discuss gap later (ALL)
-->

<!-- NOTES: Yihao
Shall we spilt this sub-section into two: 1. Communication with traffic permission; 2. Communication with traffic navigation
Dirk: not sure that dividing into explicit sub-section helps. It is steering, one guided by permission and the other by chaining objectives (the latter has a linkage to the previous sub-section on comms across services). Also, the suggested second item is merely another expression for traffic steering (since navigation is close/similar to steering)
-->

<!-- NOTES: Add flexible addressing paragraph, i.e., how FA may be useful here
AP: Dirk
Luigi: I give it a try... [DONE]
--->
Flexible addressing may enable more semantic rich encoding schemes that may help in steering traffic at hardware level and speed, without complex mechanisms usually resulting in handling packets in the slow path of routers.



## Communication with built-in security {#SEC:builtin-sec}

Today, strong security and privacy in the Internet is usually implemented as an overlay based on the concept of Mix Networks ({{TOR}}, {{SPHINX}}). Among the various reasons for such approach is the limited semantic of current IP addresses, which do not allow to natively express security features or trust relationship. Efforts like Cryptographically Generated Addresses (CGA) {{?RFC3972}}, provide some security features by embedding a truncated public key in the last 57-bit of IPv6 address, thereby greatly enhancing authentication and security within an IP network via asymmetric cryptography and IPsec {{?RFC4301}}. The development of the Host Identity Protocol (HIP) {{?RFC7401}} saw the introduction of cryptographic identifiers for the newly introduced Host Identity (HI) to allow for enhanced accountability, and therefore trust. The use of those HIs, however, is limited by the size of IPv6 128bit addresses. 

Within the context of flexible addressing, any security-related key, certificate, or identifier could instead be included in a suitable address structure without any information loss (i.e., as-is, without any truncation or operation as such), avoiding therefore compromises such as those in HIP. Instead, flexible addressing would enable creating CGAs using full length certificates, or being able to support larger HIP addresses in a limited domain that use it.



<!-- NOTES: Add flexible addressing paragraph, i.e., how FA may be useful here
AP: Luigi: Actually the last paragraph of the section is already about FA benefits. I just moved it  here. 
[DONE] 
--->

A flexible addressing semantic could significantly help in constructing a trusted and secure communication at the network layer. Connections provided by such address could be considered as absolute secure (assuming the cryptography involved is secure). Even more, anti-abuse mechanisms and/or DDoS protection mechanisms like the one under discussion in PEARG ({{PEARG}}) Research Group may leverage the ability for a richer and more flexible address semantic to be more effective.  


## Communication in Alternative Forwarding Architectures {#SEC:nin}

<!-- Yihao: 
I feel that the way we narrate this sub-section is somehow weird. 
As this section is talk about use cases/requirement from the real world, like constrained devices, security, traffic steering... However, an Alternative Forwarding Architectures look like requirement from another dimension. For me, Alternative Forwarding Architectures is more like requirement from technical aspect, not the real world. Since user in real world never care about the forwarding architecture, and it's not the use case from users' perspective.

On the other hand, flexible addressing itself could imply the Alternative Forwarding Architectures. For example, "Communication Across Services" should already imply an Alternative Forwarding Architectures.

I suggest that we use the real use cases for these Alternative Forwarding Architectures as we describe here, like video, Deterministic QoS, and what works better under flow-based or path-based stream (instead of packet-based). 

Besides, Sheng Jiang is worrying about NIN, and the way we mention NIN. 
Maybe it is better to talk the "use case" of NIN, instead of Alternative Forwarding Architectures like NIN. Thus we could totally avoid mentioning NIN.
 -->

<!-- AP: Dirk: start this sub-section with a clear goal motivating 'alternative forwarding architecture'. This could be the desired higher efficiency, e.g., for streaming scenarios [DOne: create the starting paragraph, also with reference to MPLS and its motivation to improve on traffic engineering]
AP: Luigi: review that new paragraph and link it to ETSI paragraph  [DONE minor changes]

Yihao: 

-->

The performance of communication networks has long been a focus for optimization due to the immediate impact on cost of ownership for communication service providers. Technologies like MPLS {{?RFC3031}} have been introduced to optimize lower layer communication, e.g., by mapping L3 traffic into aggregated labels of forwarding traffic for the purposes of, e.g., traffic engineering. 

Even further, other works have emerged in recent years that have replaced the notion of packets with other concepts for the same purpose of improved traffic engineering and therefore efficiency gains. One such area is that of Software Defined Networks (SDN) {{?RFC7426}}, which has highlighted how a majority of Internet traffic is better identified by flows, rather than packets. Based on such observation, alternate forwarding architectures have been devised that are flow-based or path-based. With this approach, all data belonging to the same traffic stream is delivered over the same path, and traffic flows are identified by some connection or path identifier rather than by complete routing information, possibly enabling fast hardware based switching.  

On the one hand, such a communication model may be more suitable to real-time traffic like the one considered in the context of Deterministic Networks ({{DETNET}}), where indeed a lot of work has focused on how to "identify" packets belonging to the same detnet flow in order to jointly manage the forwarding within the desired deterministic boundaries.

On the other hand, it may improve the communication efficiency in constrained wireless environments (cf., {{#SEC:constrained}}), by reducing the overhead, hence increasing the number of useful bits per second per Hz. Also, the delivery of information across similar flows may be combined into a multipoint delivery of a single return flow, e.g., for scenarios of requests for a video chunk from many clients being responded to with a single (multi-destination) flow, as outlined in {{BIER-MC}} as an example. Another opportunity to improve communication efficiency is being pursued in ongoing IETF/IRTF work to deliver IP- or HTTP-level packets directly over path-based or flow-based transport network solutions, such as in {{BIER-MC}}, {{ICNIP}}, and {{ICN5G}} with the capability to bundle unicast forward communication streams flexibly together in return path multipoint relations. Such capability is particularly opportune in scenarios such as chunk-based video retrieval or distributed data storage. However, those solutions currently require gateways to "translate" the flow communication into the packet-level addressing semantic in the peering IP networks.

<!-- NOTES: Dirk: I reworded the paragraph here, particularly removing any linkage to TCP and IP but centring the work on the alternative forwarding architectures and the formation of a limited domain through this 
Luigi: Looks OK for me.
-->

Alternative way of forwarding data has also been the motivation for the efforts created in the European Telecommunication Standards Institute (ETSI), who formed a Industry Specification Group (ISG) named Non-IP Networking (NIN) {{ETSI-NIN}}. This group sets out to develop and standardize a set of protocols leveraging an alternative forwarding architecture, such as provided by a flow-based switching paradigm. The deployement of such protocols may be seen to form limited domains, still leaving the need to interoperate with the (packet-based forwarding) Internet; a situation possibly enabled through flexible addressing across Internet-based and alternative limited domains alike. 

<!-- NOTES: Dirk 
Make the addressing angle of NIN here clearer (Dirk, then Luigi to review)
DIRK: changed the NIN paragraph to position NIN solutions as limited domains with the need for flexible addressing for cross-domain comms.
DIRK: simplifed first paragraph since there was repetition in the next one (where the comms model was seen more suitable for real-time traffic)
-->


<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->


# Problems in Addressing {#SEC:problem}
<!-- NOTES Dirk: I tried addressing the sub-section headings as something 'limiting' to some extent, given that it's the "problems" section -->


<!-- AP Dirk -->
## Limiting Alternative Address Semantics {#SEC:pro:semantics}

Many approaches to changing the semantics of communication, e.g., through separating host identification from network node identification {?RFC7401} or through identifying content and services directly {HICN}, are limited by the existing packet size and semantic constraints of IPv6, e.g., in the form of its source and destination network addresses. 

While approaches such as {{ICNIP}} may override the addressing semantics, e.g., by replacing IPv6 source and destination information with path identification, a possible unawareness of endpoints still requires the carrying of other address information as part of the payload, as discussed in Section {{#SEC:pro:efficiency}}.  Also, the expressable service or content semantic may be limited, as in {{HICN}} or the size of supported networks {{REED}} due to relying on the limited bitpositions usuable in IPv6 addresses. 

<!-- Move paragraph to secuirty section since it is more suitable -->

<!-- AP Luigi [DONE] -->
## Hampering Security {#SEC:pro:security}

Fitting any new semantic into existing size constraints may hamper the original objectives for introducing the new semantics in the first place. For instance, host identifiers {{?RFC7401}} or security information may be limited by the IPv6 address size, as discussed in Section {#SEC:builtin-sec} with the example of CGA {{?RFC3972}}. On the one hand, a more flexible addressing would allow to introduce fully featured security in endpoint identification, potentially able to eradicate the spoofing problem. On the other hand, it may be used to include application gateways' certificates in order to provide  more efficiency, e.g.,   using web certificates also used in the addressing of web services.    

While increasing security, also privacy protection can be improved. IP addresses, even temporary ones, have been long recognized as a "Personal Identification Information" that allows even to geolocated the communicating endpoints {{?8280}}. A more flexible addressing scheme may allow to use cryptographically generated anonymous addresses when considered needed, also protecting from geolocation making such addresses topologically independent, potentially allowing to implemet secure architeture like {{TOR}} and {{SPHINX}} at network layer, improving the overall efficiency as described in {{{#SEC:pro:efficiency}}.      

Alternative addressing semantics may also help in (D)DoS mitigation. This can be achieved by changing the service identification model, making it completely orthogonal from network topology semantic. In this way, mounting such type of attacks may become harder, and by not exposing all of the topological information the attack surface, and hence the potential disruptions, may remain limited {{ADDRLESS}}.  



<!-- AP Dirk -->
## Complicating Traffic Engineering {#SEC:pro:traffic}

Efforts in traffic engineering have long shown that the IP address itself is not enough for steering traffic properly, seeing the introduction of differentiated service code points (DSCP), the use of header information of various kinds (such as ports) as flow information and the entirely separate expression of path information, e.g., in the form of MPLS labels or through introducing bitposition-based path identifiers {{BIER-MC}}{{REED}. Newer approaches to IP anycast suggest the use of service identification in combination with a binding IP address model {{dyncast}} as a way to allow for metric-based traffic steering decisions, while approaches for service function chaining {{?RFC7665}} utilize next service header (NSH) information and packet classification to determine the destination of the next packet.

Overall, when it comes to providing capabilities for traffic engineering, the IP address itself is not semantically rich enough to adequately describe the forwarding decision to be taken in the network, not only impacting the WHERE the packet will need to go but also HOW it will need to be sent. Instead, various supplementary information needs to be taken into account for a successful delivery to take place.


<!-- AP Luigi -->
<!-- NOTES Dirk: I suggest folding this under efficiency since this is mainly covered by 'introducing path stretch' -->
<!-- LUIGI: Agreed. I added some mobility-related sentences in the efficiency sub-sections -->
<!-- ## Supporting Mobility {#SEC:pro:mobility} -->


<!-- AP Yihao -->
## Hampering Efficiency {#SEC:pro:efficiency}

### Header proportion

Although fiber and ethernet dominate the Internet infrastructure, numours links, e.g., wireless radio, is expected to improve communication efficiency. As IPv6 header fixedly occupies 40 byte in a packet{{!RFC8200}}, header compression techniques are introduced to shaping payload occupation within a packet. RObust Header Compression (ROHC) {{?RFC5795}}, which customized for cellar network, is being widely adopted in radios like WCDMA, LTE, and 5G. Considering one base station is supposed to serve hundreds of user devices, maximizing the effectiveness for specific spectrum directly improve user quality of experience.

Similar header compression mechanisms are usually adopted for communications among constrained devices. Due to the memory or battery constraint, constrained devices prefer maximize efficiency for each packet they deliver. For personal area network, the IEEE 802.15.4 enabled devices, which occupy the most share of the market, either equipped with customized proprietary protocol, or compress the header utterly as in {{?RFC4944}}. Particular for proprietary protocol, e.g., Zigbee, an application level gateway should be introduced at the edge of the local network. Terminations of the communications by such gateway break the end-to-end principle via uncondiction trust as potential weak point, thus looping back to security crisis in Section {{#SEC:pro:security}}. 

Also, constraints coming from either devices or carrier links would lead to a mixed scenarios and compound requirements for extraordinary header compression. For native IPv6 communications on DECT ULE and MS/TP Networks, dedicated compression mechanisms are specificed in {{?RFC8105}} and {{?RFC8163}}, while the transmission of IPv6 packets over NFC and PLC, specifications are being developed in {{?I-D.ietf-6lo-nfc}} and {{?I-D.ietf-6lo-plc}}. For low power wide-area network, a generic framework for static context header compression is depicted in {{?RFC8724}} for efficiency improvement.


### Introducing Path Stretch

To serve a moving endpoint (described in Section {{#SEC:mobility}}), mechanisms like Mobile IP {{?RFC3775}} are used to the maintainance of connection continuity. As the result of the locator semantic in IP address {{?RFC2101}}, traffic must follow a triangular route before arriving the updated location inevitably affecting  the transmission efficiency as well as latency.  

<!-- NOTES Dirk: didn't really quite get the paragraph below -->
<!-- LUIGI: TOR actually uses path stretch as part of path privacy, in TOR nobody knows how many relays are used and nobody knows all the set of them. SO basically this is a feature not a bug. AKA I miss the point as well ...   -->
Another example for introducing additional path stretch is the routing in TOR (described in Section {{#SEC:builtin-sec}}). As the address indicates identifications to a certain extent {{?RFC2101}}, privacy enhancement mechanisms usually involve the concealment of the source IP address during communications. To achieve high anonymity, traffic must be handovered by 3 intermediate before reaching the destionation. Undoubtlly, frequent relaying enhance the privacy at the cost of lower communication efficiency, no matter how close the destinations are located in.

IP Anycast {{?RFC7094}} is usually adopted for efficient content delivery through extensive replica distribution. In most cases, request packets should be guided to the nearest server in relation to, e.g., geography or network topology, while occasionally, traffic may also be directed to a remote or suboptimal site. Given that Autonomous Systems (AS) always select route according to their own preference, e.g., route of shortest AS path or customer AS path, traffic guidence for the nearset site is hard to be guaranteed (see {{ANYCAST}}), while computing-related metrics are mostly ignored.


### Repetitive encapsulation

Addressing proposals such as those in {{ICNIP}} utilize path identification within an alternative forwarding architecture that acts upon the provided path identification. However, due to the limitation of existing flow-based architectures with respect to the supported header structures (in the form of IPv4 or IPv6 headers), the new routing semantics are being inserted into the existing header structure, while repeating the original, sender-generated header structrure, in the payload of the packet as it traverses the limited domain, effectively doubling the header overhead per packet. 

The problem is also present in number of solutions tackling different issues, e.g., mobility  {{{{?I-D.ietf-lisp-introduction}}}}, DC networking ({{?RFC8926}}, {{?RFC7348}}, {{I-D.ietf-intarea-gue}}), and privacy ({{TOR}}, {{SPHINX}} ). Certainly these solutions are able to avoid other issues, like path stretch or privacy, but they come at the price of multiple encapsulations that reduce the effective payload.     


<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->



# Problem Statement 

This document highlighted that with the emergence of limited domains, novel approaches to addressing in communication scenarios are being developed and deployed within those limited domains. 

While this may be interpreted as a crucial point to the flexibility of addressing in the Internet, evidence does exist (as describe in this document) that the existing Internet addressing structure itself is a potential hinderance in solving key problems for Internet service provisioning, such as supporting new, e.g., service-oriented, use cases more efficiently, with improved security and efficient traffic engineering as well as mobility at large scale in mind. 

As a problem statement, this document's goal is not to propose or promote specific solutions to the problems here portrayed.  Instead, this document aims at stimulating discussion on the emerging needs for addressing at large with the possibility to fundamentally re-think the addressing in the Interrnet beyond the current objectives of IPv6.


# Security Considerations {#SEC:sec}

TBD.


# IANA Considerations {#SEC:iana}

This document does not include an IANA request.





<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->


--- back

# Change Log

**NOTES**: Please remove this section prior to publication of a final version of this document.

## Since draft-jia-intarea-flexible-addressing-use-cases-gap-analysis-00

- Revised all use-cases;
- Added Problems;


# Acknowledgments
{:numbered="false"}

Here is Acknowledgements.










































<!-- AP (ALL): start a bullet item list (with references, if possible) on gaps in solutions for the specific use cases
No fancy wording, just listing things
-->


<!-- # Gap Analysis {#SEC:gap} -->

<!-- WRITE_ME.

- General intro stating what exactly are we focusing on in this section (missing native features of IP??)

- Somewhere after the gap analysis we should state that the design of IP may look limited today because of a lot of technological advances (hardware and software) and an evolution of the needs (the use-cases) but definitely a huge leap forward 30/40 years ago. (similar to the intro of NIN) 
- We have to make really really sure that the gap analysis, and this document in general, is not received as "IP is bad" but rather as "IP can be improved".
  - I agree with the sentiment BUT such statement can only be done (not as a statement itself but as a perception) within the gap analysis itself. For instance, limitations introduced in certain aspects may be pinned down to limitations in HW/SW that have long been overcome. 
  - however, we could state something along those lines in the introduction - I attempted this, as you might have noticed

- I suggest gathering the main points first, then attempting to formulate the main gaps and aspects, then add the evidence in the form of references. -->

<!-- NOTE Luigi: I wonder if we are going in the right direction with the GAP analaysis. Looking at the DMM document https://www.rfc-editor.org/rfc/rfc7429.html#page-19 they do an interesting thing they just list GAPs. May be we could do the same? Appending the list of use cases that may benefit from solving the GAP?
Somthing like:

GAP 1: IP addresses carry a dual semantic, namely topological smeantic and identification semantic. At the same time IP addresses _always_ and _only_ carry these two semantics. Devising a flexible addressing scheme allowing to flexibly modulate the semantic that the addresses carry would be benefitial since there is no need anymore to have new namespaces for eahc new semantics that existing and future use case may need. In particular the following previously dscribe use-cases would benefit:
- Communication with built-in security ({{#SEC:builtin-sec}})
- etc etc    

Thoughts ?

 -->


<!-- ## Communication in Constrained Environments -->
<!-- AP: Luigi -->

<!-- WRITE_ME. -->

<!-- - Header compression/adaptation and different addressing in IoT domains like 6LoPAN etc. -->
<!-- - we need research on overhead here -->



<!-- ## Communication in Dynamically Changing Topologies -->
<!-- AP: Yihao -->

<!-- WRITE_ME.

- LISP Nexagon can be used as example of how having addresses with semantic is useful whereas IP has rigid addressing structure 
- Geo-location could be used for routing. That make the forwarding shift from table lookup based routing to computing based routing. 
- can use Handley {{HANDLEY}} reference here?  -->

<!-- ## Communication Across Services -->
<!-- AP: Dirk [DONE first version] -->

<!-- Solutions like ICN {{ICNRG}} enable the communication between clients and provider of directly addressable content, with recent extensions {{REF to ICN2018 Krol work}}{{ICNIP}} also covering the communication with services. This enables the authentication of content at the network level, delegating the delivery to, e.g., caches or content delivery nodes, as well as not relying on mapping servics like the DNS to map the information or service name semantic onto a topological IP address, thereby reducing the latency introduced through such explicit name mapping. 

As outlined in {{?RFC8763}}, ICN deployments may either exist as native deployments parallel to the IP-based Internet, run as an overlay over existing IP networks or provide the underlay for Internet services (such as in {{ICNIP}}). Solutions such as those in {{HICN}} allow for the provisioning of ICN-based content within existing IP-based networks albeit limited by the need for a separate IPv6 address family and the size limitations of the IPv6 addresses used, while HICN also uses transport layer fields for further encoding name semantics, overall limited (in expressiveness and size) by those fields in the used L3/L4 headers. As pointed out in {{?RFC8763}} as well as the work in {{ICNIP}}, dedicated gateways need often to be introduced for translating not just address structures but protocols between communication originating in an ICN-based domain and terminating in an IP-based one. 

Although the possible replacement of an IP-based internetworking capability has been postulated by works such as {{CCN}} or {{TROSSEN}}, the realization of pure ICN, i.e., no-IP addressing (and routing) environments can only be found in greenfield, mostly edge deployments, as also pointed out by {{?RFC8763}}.  -->



<!-- ## Steering Communication Traffic -->
<!-- AP: Dirk [DONE first version] -->

<!-- The semantic of IP-based addressing is that of a packet delivery between sender and receiver under best effort conditions of the networks providing the delivery. Any steering capability is therefore realized as an overlay or underlay within that semantic. Steering-relevant information is added through new packet fields, e.g., through MPLS labels, stack of IPv6 addresses (for SRv6), next hop headers (NSH) for service function chaining, flow information for DetNet-based forwarding at L3, or path identifiers for utilizing path steering in transport architectures like SDN or BIER {{BIER-MC}}{{ICNIP}}. Alternatively, mapping functions are required to map a service semantic expressed through an IP anycast address to a binding IP address of the selected receiver, as in {{dyncast}}, or using the DNS for load balancing purposes. 

Hence, while this rigidity of IP addressing can be accommodated by such overlays and gateway solutions, it introduces complexity and therefore possible failure points in intermediary network functions.  -->

<!-- ## Communication with built-in security -->
<!-- AP: Luigi -->
<!-- WRITE_ME. -->

<!-- - HIP security Gap Analysis
- Limitation of IPSec w.r.t. to Mix Networks (aka TOR and SPHINX)
- Extended CGA with big addresses that may include a full key/crt -->

<!-- ## Communication in Alternative Forwarding Architectures -->

<!-- AP: Dirk, Luigi to review quickly 
NOTE: Dirk: I avoided NIN entirely below since the discussion is captured IMO in the part on path/flow-based architectures -->

<!-- The aforementined best effort delivery semantic, expressed through the IP address semantic of a source and destination, has seen numerous extensions in the evolution of the Internet. 

Type-of-Service as well as flow information, e.g., for deterministic IP capabilities, have been added to the classical 5-tuple definining the ends of a communication relation. Apart from adding such new information to outline required key capabilities for the end-to-end delivery, approaches such as SDN have used existing packet header information beyond the IP source and destination addresses to allow for programmable forwarding decisions. Approaches such as those in {{REED}} propose to override the IPv6 addresses of packets to realize a path-based forwarding architecture with service-level information (in the form of URLs or IP addresses) carried in the payload {{ICNIP}}. 

While such path-based architectures may provide interesting multicast capabilities, as also outlined in {{BIER-MC}}, they suffer from scalability limitations in terms of supported network size. Equally, flow-based architecture may provide superior traffic engineering capabilities but may suffer scalability limits in terms of supported or flow entries. This combination of superior capability and limitation, however, makes them particularly attractive for the realization in limited domains of often limited scalability but with specific performance requirements that are addressed through the alternative forwarding architecture. On the downside, however, any communication with non-path-based environments, as pointed out in {{?RFC8763}}, requires gateway solutions to 'translate' restore the IP addressing structure. 

Solutions that enable to constrain the delivery towards more than one possible endpoint, such as works proposed in {{dyncast}} or also {{ICNIP}}, require the definition of such constraint outside the existing IP address structure, including the conveyance of such constraint to the intermediary nodes in the network.   -->

<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->

<!-- ## Summary  -->
<!-- NOTES: Dirk: I suggest to add a table here with the main points in the various sub-sections -->

<!-- # Requirements {#SEC:req} -->

<!-- WRITE_ME.

According to the capabilities for scenarios above, this section extracts basic requirements for introducing flexible addressing.
Points below details the basal requirements.

- Multi-Semantics: Since semantics are the core of network routing, multi-semantics compose the main capability of flexible addressing.

- Variable Address Length: As for networks with constrained devices, short address becomes necessary for protocol adoption. While on other hand, address space should be adequate enough to accommodate numerous devices.

- IPv6 Interoperability: Without global reachability, flexible addressing would be the same as an exclusive protocol. In other words, flexible addressing should be valuable only it is inter-operable with IPv6. -->




<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->





<!-- # Security Considerations {#SEC:sec}

WRITE_ME.

- Spoofing: semantics fraud
- Sniffing: privacy leak


# IANA Considerations {#SEC:iana}

This document does not include an IANA request. -->





<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->
<!------------------------------- SECTION DIVISION ------------------------------->

<!-- 
--- back

# Change Log

**NOTES**: Please remove this section prior to publication of a final version of this document.

## Since draft-jia-intarea-flexible-addressing-use-cases-gap-analysis-00

- Revised all use-cases;
- Added gap analysis;
- Added requirements;
- Added security consideration;
- Fixed issue X;
- Fixed issue Y;

## Since draft-jia-intarea-flexible-addressing-use-cases-gap-analysis-00-0121-v2

- moved vlan etc back to traffic steering
- added references to SRv6 and SFC in steering sub-section
- added references to ICN work in NIN sub-section

# Acknowledgments
{:numbered="false"}

Here is Acknowledgements. 
-->

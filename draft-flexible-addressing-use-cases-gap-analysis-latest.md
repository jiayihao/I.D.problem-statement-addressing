---
title: "Flexible Addressing: Use Cases and Gap Analysis"
abbrev: Flexible Addressing Gap Analysis
docname: draft-jia-intarea-flexible-addressing-use-cases-gap-analysis-latest
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




--- abstract

Although RFC8799 {{!RFC8799}} recognizes "limited domains" as exhibiting  domain-specific requirements as well as communication behaviours and semantics, the topological location defined in the IP address structure requires the mapping of those domain-specific concepts onto that single address structure, used across what makes up the Internet as a whole at the networking layer. 

This document describes well-recognized scenarios that exhibit possibly different addressing requirements with the intention to outline gaps in existing solutions as well as requirements for a flexible address structure that could be used instead of the fixed address structure of current IP. 

--- middle



[COMMENTS]: # (Texts in here will be ignored.)



# Introduction {#SEC:intro}

[NOTES]: # (the introduction now captures the whole point of this document, as it should, namely the link to limited domains and the possibility to do flexible addressing instead of relying on some sort of mapping solutions across all those limited domains. I think that such kind of introduction removes any need for the 'scope' section previously included.)

On the one hand, positioned as the unified protocol of the (Internet) network layer, the Internet Protocol (IP) is seen as key to the innovation stemming from Internet-based applications and servicxes. Even more so, with the success of TCP/IP protocol stack, IP is gradually replacing existing domain-specific protocols, evolving into the core protocol of the entire communication system.

On the other hand, the concept of the "Limited domain" was first introduced in {{!RFC8799}}. It refers to a single physical network, attached to or running in parallel with the Internet, or is defined by set of users and nodes distributed over a much wider area, but drawn together by a single virtual network over the Internet. Key to limited domain is that requirements, behaviors, and semantics could be noticeable local and, more importantly, specific to the limited domain.

One key architrectural aspect when communicating within limited domains is that of addressing and, therefore, the address structure as well as semantic that is being used for the routing of packets within such limited domains. The topological location centricity of IP is fundamental when reconciling the often differing semantics for 'endpoint addressing' that can be found in those limited domains. The result of this fundamental role of the single address structure are solutions that are specific to those limited domains, translating/mapping/converting concepts, semantics, and ulitmately, domain-specific address structures into the common IP format.

In this document, we advocate the discussion on devising a flexible address structure instead that allows for those limited domain semantics to be represented directly at the (IP) address structure, reducing or even entirely removing the need for mapping limited domain address semantics onto the current topological location. For this purpose, we describe well-recognized scenarios, analyse the gaps in existing solutions for those scenarios, finally stating requirements for a flexible address structure that would realize those scenarios instead. 


# Conventional Terminology {#SEC:term}

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in BCP 14 {{!RFC2119}} {{!RFC8174}} when, and only when, they appear in all capitals, as shown here.

# Use Cases {#SEC:cases}

[NOTES]: # (I suggest focussing the use cases on various aspects of 'communication' at large, which includes many things, but then honing into the addressing impact of that 'communication')

The following section outlines a number of scenarios, all of which we can see embedded into the concept of "limited domains" {{!RFC8799}}. While a list of use cases may be long, we focussed our use cases on a number of aspects that we can observe in those limited domains, captured in the sub-section titles. For each use case, we point at possible challenges, which we will pick upon in the gap analysis in Section (not sure how to reference) in more detail in relation to in existing technology. 

## Communication in Constrained Environments 

In a number of communication scenarios, such as those encountered in the Internet of Things (IoT), a simple, low-cost communication network is required with limitations for network devices in terms of computational power, memory, and energy availability. In addition to IEEE.802.15.4, link layer technologies such as Z-Wave, BLE, DECT_ULE, MS/TP, NFC, and PLC all require end-to-end IPv6 protocols {{!RFC8200}} to form constrained node networks, where the IP protocol allows those nodes to connect to each other or to other nodes on the Internet. Devices located at the edge of this network can act as gateway devices towards the Internet, where the gateway may be selected for traffic passthrough by the devices on the (limited domain) network. 

Given the constraints imposed on the computational and possibly also communication technology, the usage of a singe addressing semantic in the form of a 128bit endpoint identifier may pose a challenge when operating such networks. 

[NOTES]: # (can we add any references here that evaluated those overheads?)


## Communication in Dynamically Changing Topologies

Communication may occur over networks that exhibit dynamically changing topologies. One such example is that of satellite networks, providing global Internet connections through a combination of inter-satellite and ground station communication. With the convergence of space-based and terrestrial networks, users can experience seamless broadband access, e.g., on cruise ships, flights, and within cars, often complemented by and seamlessly switching between  Wi-Fi, cellular, or satellite based networks at any time. The satellite network service provider will plan the transmission path of user traffic based on the network coverage, satellite orbit, route, and link load, providing potentially high-quality Internet connections for users in areas that are not covered by terrestrial networks. The involved  topologies of the satellite network will be changing constantly while observing a regular flight pattern in relation to other satellite and predictable overflight patterns to ground users. 

Another example is that of vehicular communication, where services may be accessed across vehicles, such as self-driving cars, for the purpose of collaborative objection recognition (e.g., for collision avoidance), road status conveyance (e.g., for pre-warning of road-ahead conditions) and other purposes. Communication may include roadside units (RSU) with the possibility to create ephemeral connections to those RSUs for the purpose of worload offloading, joint computation over multiple (vehicular) inputs and other purposes. Communication here may exhibit a multi-hop nature, not just involving the vehicle and the RSU over a direct link. Those topologies are naturally changing constantly due to the dynamic nature ofthe involved communication nodes. 

In both network technologies, there is a significant difference between the high dynamics of the underlying network topologies, compared to the relative static nature of terrestrial network topology. As a consequence, the notion of a topological network location becomes restrictive in the sense that not only the relation between network nodes and user endpoint may change but also the relation between the nodes that form the network itself. This may lead to the challenge of maintaining and updating the topological addresses in this constantly changing network topology. 

[NOTES]: # (Reference to Handley work here?)

## Communication Between Services

As a communication infrastructure spanning many facets of life, the Internet integrates services and resources from various aspects such as remote collaboration, shopping, content production as well as delivery, education and many more. Accessing those services and resources directly through URIs has been discussed by methods such as those defined in ICN {{?RFC7476}}, where providers of services and resources can publish those through unified identifiers without additional planning of identifiers and locations for underlying data and their replicas. Users can access required services and resources by virtue of using the URI-based identification, with an ephemeral relationship built between user and provider, while the building of such relationship may be constrained with user- as well as service-specific requirements, such as proximity (finding nearest provider), load (finding fastest provider), and others. 

While systems like ICN provide an alternative to the locator-based addressing of IP, its deployment requires an overlay (over IP) or native deployment (alongside IP), the latter with dedicated gateways needed for translation. Underlay deployments are also envisioned in {{!RFC8763}}, where ICN solutions are being used to faciliate communication between IP addressed network endpoints or URI-based service endpoints, still requiring gateway solutions for interconnection with ICN-based networks as well as IP routing based networks. Although various approaches to combining service and location-based addressing have been devised, the key challenge here is to faciliate a "natural", i.e., direct communication without the need for gateways above the network layer.

[NOTES]: # (Reference to RFC8763 but also ongoing IP-over-NDN as well as the ongoing Internet-over-ICN draft in ICNRG?)


## Steering Communication Traffic

Steering traffic within a communication scenario may involve at least two aspects, namely (i) limiting certain traffic towards a certain set of communication nodes and (ii) constraining the sending of packets towards a given destination with metrics that would allow the selection among one or more possible destinations. 

One possibility for limiting traffic towards specific objects, e.g., devices, users, or group of them, is subnet partition with techniques such as VLAN {{?RFC5517}} and VxLAN {{?RFC7348}} realizing such partitioning. Such mechanisms usually involve manual configuration, and even small changes in network and user nodes could result in a repartition and possibly even more manual efforts. Another key aspect is the disconnection from the topological address and any likely more semantic-rich identification that would be used to make any policy decision regarding traffic steering. Suitably enriching the semantics of the packet address, either that of the sender or receiver, so that such decision could be made while minimizing the involvement of higher layer mechanisms, is a crucial challenge for improving on network operations and speed of such limited domain traffic. 

When making decisions to select one out of a set of possible destinations for a packet, IP anycast semantics can be applied albeit being limited to the locator semantic of the IP address itself. Recent work in {{?dyncast}} suggests utilizing the notion of utilizing the IP anycast address to encode a "service identifier", which is dynamically mapped onto a unique network location where one (of the possibly many) service instances fulfilling the service request may be located. Scenarios where this capability may be utilized are provided in {{?dyncast}} and include, but are not limited to, scenarios such as edge-assisted VR/AR, transportation and digital twins. 

This communication use case expands on the previously discussed communication between services by foreseen to constrain the selection of the specific service instance that may realize the service. The challenge here lies in the possible encoding of not only the service information itself but the constraint information that aids the selection of the "best" service instance under the possibly service-specific constraints of the particular scenario.  

[NOTES]: # (what other references?)

## Communication with built-in security

[NOTES]: # (Leaving this mostly to Luigi ;-))
[NOTES]: # (Can we make references here to P:L approaches for securing aspects like service routing, allowing for oblivious routing, stronger than today's IP routing?)

A flexible semantic could be significate in constructing a trust and secure communication.
For example, Cryptographically Generated Addresses (CGA) {{?RFC3972}} embeds a truncated public key in the last 57-bit of IPv6 address. Even with a truncated key, authentication and security is greatly enhanced within a IP network via asymmetric cryptography and IPsec {{?RFC4301}}.
Similarly, Host Identity Protocol (HIP) {{?RFC7401}} refers such methodology and constructs a enhanced TCP/IP stack. 


Within a flexible address structure, any secure-related keys could be intactly included in address structure without any information loss. Under such condition, connection provided by such address could be considered as absolute secure only if the cryptography involved is secure.


# Gap Analysis {#SEC:gap}

WRITE_ME.

## Communication in Constrained Environments

WRITE_ME.

## Communication in Dynamically Changing Topologies

WRITE_ME.

## Communication Between Services

WRITE_ME.

## Steering Communication Traffic

WRITE_ME.

## Communication with built-in security

WRITE_ME.

# Requirements {#SEC:req}


WRITE_ME.

According to the capabilities for scenarios above, this section extracts basic requirements for a flexible address structure.
Points below details the basal requirements.

* Multi-Semantics: Since semantics are the core of network routing, multi-semantics compose the main capability of the flexible address.
  
* Variable Address Length: As for networks with constrained devices, short address becomes necessary for protocol adoption. While on other hand, address space should be adequate enough to accommodate numerous devices.

* IPv6 Interoperability: Without global reachability, a flexible address would be the same as an exclusive protocol. In other words, a flexible address should be valuable only it is inter-operable with IPv6.









# Security Considerations {#SEC:sec}

WRITE_ME.

- Spoofing: semantics fraud
- Sniffing: privacy leak




# IANA Considerations {#SEC:iana}

This document does not include an IANA request.








--- back

# Change Log

**NOTES**: Please remove this section prior to publication of a final version of this document.

## Since draft-jia-intarea-flexible-addressing-use-cases-gap-analysis-00

- Fix issue X.
- Fix issue Y.


# Acknowledgments
{:numbered="false"}

Here is Acknowledgements.

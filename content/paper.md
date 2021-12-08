+++
title = "Paper"
date = "2019-02-09"
+++

## When Parents and Children Disagree: Diving into DNS Delegation Inconsistency

### Raffaele Sommese, Giovane Moura, Mattijs Jonker, Roland van Rijswijk-Deij, Alberto Dainotti, Kimberly Claffy, Anna Sperotto

#### PAM2020 Passive and Active Measurement Conference



The Domain Name System (DNS) is a hierarchical, decentralized, and distributed database. A key mechanism that enables the DNS to be hierarchical and distributed is delegation [7] of responsibility from parent to child zones—typically managed by different entities. RFC1034 [12] states that authoritative nameserver (NS) records at both parent and child should be “consistent and remain so”, but we find inconsistencies for over 13M second-level domains. We classify the type of inconsistencies we observe, and the behavior of resolvers in the face of such inconsistencies, using RIPE Atlas to probe our experimental domain configured for different scenarios. Our results underline the risk such inconsistencies pose to the availability of misconfigured domains.

<a href="https://academia.r4ffy.info/paper/SommesePam2020.pdf">Download</a>

## The Forgotten Side of DNS: Orphan and Abandoned Records

### Raffaele Sommese, Mattijs Jonker, Roland van Rijswijk-Deij, Alberto Dainotti, Kimberly Claffy, Anna Sperotto

#### WTMC2020 5th International Workshop on Traffic Measurements for Cybersecurity 


DNS zone administration is a complex task involving manual work and several entities and can therefore
result in misconfigurations. Orphan records are one of these
misconfigurations, in which a glue record for a delegation
that does not exist anymore is forgotten in the zone file.
Orphan records are a security hazard to third-party domains
that have these records in their delegation, as an attacker
may easily hijack such domains by registering the domain
associated with the orphan. The goal of this paper is to
quantify this misconfiguration, extending previous work by
Kalafut et al., by identifying a new type of glue record
misconfiguration – which we refer to as abandoned records –
and by performing a broader characterization. Our results
highlight how the situation has changed, not always for the
better, compared to a decade-old study.

<a href="https://academia.r4ffy.info/paper/SommeseWTMC2020.pdf">Download</a>

## Manycast2 -- Using Anycast to Measure Anycast
### Raffaele Sommese, Leandro Bertholdo, Gautam Akiwate, Mattijs Jonker, Roland van Rijswijk-Deij, Alberto Dainotti, Kimberly Claffy, Anna Sperotto
#### IMC2020 ACM Internet Measurement Conference


Anycast addressing -- assigning the same IP address to multiple, 
distributed devices -- has become a fundamental approach to improving
the resilience and performance of Internet services, but its conventional 
deployment model makes it impossible to infer from the address itself 
that it is anycast. Existing methods to detect anycast IPv4 prefixes 
present accuracy challenges stemming from routing and latency dynamics, 
and efficiency and scalability challenges related to measurement load. 
We review these challenges and introduce a new technique we call MAnycast2 
that can help overcome them. Our technique uses a distributed measurement 
platform of anycast vantage points as sources to probe potential anycast 
destinations. This approach eliminates any sensitivity to latency dynamics,
and greatly improves efficiency and scalability. We discuss alternatives
to overcome remaining challenges relating to routing dynamics, suggesting
a path toward establishing the capability to complete, in under 3 hours,
a full census of which IPv4 prefixes in the ISI hitlist are anycast."

<a href="https://academia.r4ffy.info/paper/SommeseIMC2020.pdf">Download</a>


## Unresolved Issues: Prevalence, Persistence, and Perils of Lame Delegations
### Gautam Akiwate, Mattijs Jonker, Raffaele Sommese, Ian Foster, Geoffrey M Voelker, Stefan Savage, KC Claffy
#### IMC2020 ACM Internet Measurement Conference


The modern Internet relies on the Domain Name System (DNS) to convert between human-readable domain names and IP addresses. However, the correct and efficient implementation of this function is jeopardized when the configuration data binding domains, nameservers and glue records is faulty. In particular lame delegations, which occur when a nameserver responsible for a domain is unable to provide authoritative information about it, introduce both performance and security risks. We perform a broad-based measurement study of lame delegations, using both longitudinal zone data and active querying. We show that lame delegations of various kinds are common (affecting roughly 14% of domains we queried), that they can significantly degrade lookup latency (when they do not lead to outright failure), and that they expose hundreds of thousands of domains to adversarial takeover. We also explore circumstances that give rise to this surprising prevalence of lame delegations, including unforeseen interactions between the operational procedures of registrars and registries."

<a href="https://academia.r4ffy.info/paper/AkiwateIMC2020.pdf">Download</a>


## Characterization of Anycast Adoption in the DNS Authoritative Infrastructure
### Raffaele Sommese, Gautam Akiwate, Mattijs Jonker, Giovane C. M. Moura, Marco Davids, Roland van Rijswijk-Deij, Geoffrey M. Voelker, Stefan Savage, Kimberly C. Claffy, Anna Sperotto
#### TMA2021 Network Traffic Measurement and Analysis Conference



Anycast has proven to be an effective mechanism to enhance resilience in the DNS ecosystem and for scaling DNS nameserver capacity, both in authoritative and the recursive resolver infrastructure. Since its adoption for root servers, anycast has mitigated the impact of failures and DDoS attacks on the DNS ecosystem. In this work, we quantify the adoption of anycast to support authoritative domain name service for toplevel and second-level domains (TLDs and SLDs). Comparing two comprehensive anycast census datasets in 2017 and 2021, with DNS measurements captured over the same period, reveals that anycast adoption is increasing, driven by a few large operators. While anycast offers compelling resilience advantage, it also shifts some resilience risk to other aspects of the infrastructure. We discuss these aspects, and how the pervasive use of anycast merits a re-evaluation of how to measure DNS resilience.

<a href="http://dl.ifip.org/db/conf/tma/tma2021/tma2021-paper1.pdf">Download</a>



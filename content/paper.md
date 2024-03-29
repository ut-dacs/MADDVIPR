+++
title = "Papers"
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


## Hosting Industry Centralization and Consolidation
### Luciano Zembruzki, Raffaele Sommese, Lisandro Zambenedetti Granville, Arthur Selle Jabocs, Mattijs Jonker, Giovane Moura
#### IEEE/IFIP Network Operations and Management Symposium 2022

There have been growing concerns about the concentration and centralization of Internet infrastructure. In this work, we scrutinize the hosting industry on the Internet by using active measurements, covering 19 Top-Level Domains (TLDs). We show how the market is heavily concentrated: 1⁄3 of the domains are hosted by only 5 hosting providers, all US-based companies. For the country-code TLDs (ccTLDs), however, hosting is primarily done by local, national hosting providers and not by the large American cloud and content providers. We show how shared languages (and borders) shape the hosting market — German hosting companies have a notable presence in Austrian and Swiss markets, given they all share German as official language. While hosting concentration has been relatively high and stable over the past four years, we see that American hosting companies have been continuously increasing their presence in the market related to high traffic, popular domains within ccTLDs — except for Russia, notably.

<a href="https://ris.utwente.nl/ws/files/287285411/10.1109_noms54207.2022.9789881.pdf">Download</a>


## Domain Name Lifetimes: Baseline and Threats
### Antonia Affinito, Raffaele Sommese, Gautam Akiwate, Stefan Savage, Kimberley Claffy, Geoffrey M. Voelker, Alessio Botta, Mattijs Jonker
#### TMA2022 Network Traffic Measurement and Analysis Conference


The domain name system (DNS) is a key componentof the Internet. The DNS is essentially a hierarchical anddistributed database that involves – and is operated by – manyindependent parties that fulfill various roles. Top-level domainssuch as .com and .co.uk are run by registries. Registrants canregister domain names, usually through so-called registrars, butsometimes directly with the TLD registry.Domain names go through a well-defined life-cycle and namesthat are only short-lived in ways break expectation. In thispaper, we study domain name lifetimes at scale and over a tenyear period. We focus on ten prominent TLDs and observe thatunder most, the vast majority of lifetimes (95%) last exactly theminimum registration term of one year. The exception to thisis .com, which sees 40% of lifetimes renewed for at least onemore year. We also identify lifetimes that are suspiciously shortlived (e.g., 80% under .xyz). Using blocklist data we confirmthat about 25% are reportedly malicious and study indicators ifnames are taken down and how quickly. Finally, we empiricallystudy malicious name registration campaigns and show that thisinvolves registrars that offer bulk registration options.

<a href="https://tma.ifip.org/2022/wp-content/uploads/sites/11/2022/06/tma2022-paper32.pdf">Download</a>

## Saving Brian's privacy: the perils of privacy exposure through reverse DNS                                 
### Olivier Isaac van der Toorn, Roland Martijn van Rijswijk - Deij, Raffaele Sommese, Anna Sperotto, Mattijs Jonker
#### IMC2022 ACM Internet Measurement Conference


Given the importance of privacy, many Internet protocols are nowadays designed with privacy in mind (e.g., using TLS for confidentiality). Foreseeing all privacy issues at the time of protocol design is, however, challenging and may become near impossible when interaction out of protocol bounds occurs. One demonstrably not well understood interaction occurs when DHCP exchanges are accompanied by automated changes to the global DNS (e.g., to dynamically add hostnames for allocated IP addresses). As we will substantiate, this is a privacy risk: one may be able to infer device presence and network dynamics from virtually anywhere on the Internet — and even identify and track individuals — even if other mechanisms to limit tracking by outsiders (e.g., blocking pings) are in place.We present a first of its kind study into this risk. We identify networks that expose client identifiers in reverse DNS records and study the relation between the presence of clients and said records. Our results show a strong link: in 9 out of 10 cases, records linger for at most an hour, for a selection of academic, enterprise and ISP networks alike. We also demonstrate how client patterns and network dynamics can be learned, by tracking devices owned by persons named Brian over time, revealing shifts in work patterns caused by COVID-19 related work-from-home measures, and by determining a good time to stage a heist.

<a href="https://ris.utwente.nl/ws/portalfiles/portal/287286621/3517745.3561424.pdf">Download</a>


## Retroactive identification of targeted DNS infrastructure hijacking                                 
### Gautam Akiwate, Raffaele Sommese, Mattijs Jonker, Zakir Durumeric, Kimberley Claffy, Geoffrey M. Voelker, Stefan Savage
#### IMC2022 ACM Internet Measurement Conference 


In 2019, the US Department of Homeland Security issued an emergency warning about DNS infrastructure tampering. This alert, in response to a series of attacks against foreign government websites, highlighted how a sophisticated attacker could leverage access to key DNS infrastructure to then hijack traffic and harvest valid login credentials for target organizations. However, even armed with this knowledge, identifying the existence of such incidents has been almost entirely via post hoc forensic reports (i.e., after a breach was found via some other method). Indeed, such attacks are particularly challenging to detect because they can be very short lived, bypass the protections of TLS and DNSSEC, and are imperceptible to users. Identifying them retroactively is even more complicated by the lack of fine-grained Internet-scale forensic data. This paper is a first attempt to make progress at this latter goal. Combining a range of longitudinal data from Internet-wide scans, passive DNS records, and Certificate Transparency logs, we have constructed a methodology for identifying potential victims of sophisticated DNS infrastructure hijacking and have used it to identify a range of victims (primarily government agencies), both those named in prior reporting, and others previously unknown.

<a href="https://ris.utwente.nl/ws/portalfiles/portal/287286585/3517745.3561425.pdf">Download</a>


## Investigating the impact of DDoS attacks on DNS infrastructure                                 
### Raffaele Sommese, Kimberley Claffy, Roland Martijn van Rijswijk - Deij, Arnab Chattopadhyay, Alberto Dainotti, Anna Sperotto, Mattijs Jonker
#### IMC2022 ACM Internet Measurement Conference


Denial of Service (DDoS) attacks both abuse and target core Internet infrastructures and services, including the Domain Name System (DNS). To characterize recent DDoS attacks against authoritative DNS infrastructure, we join two existing data sets – DoS activity inferred from a sizable darknet, and contemporaneous DNS measurement data – for a 17-month period (Nov. 20 - Mar. 22). Our measurements reveal evidence that millions of domains (up to 5% of the DNS namespace) experienced a DoS attack during our observation window. Most attacks did not substantially harm DNS performance, but in some cases we saw 100-fold increases in DNS resolution time, or complete unreachability. Our measurements captured a devastating attack against a large provider in the Netherlands (TransIP), and attacks against Russian infrastructure. Our data corroborates the value of known best practices to improve DNS resilience to attacks, including the use of anycast and topological redundancy in nameserver infrastructure. We discuss the strengths and weaknesses of our data sets for DDoS tracking and impact on the DNS, and promising next steps to improve our understanding of the evolving DDoS ecosystem.

<a href="https://ris.utwente.nl/ws/files/287286559/3517745.3561458.pdf">Download</a>


## Assessing e-Government DNS Resilience
### Raffaele Sommese, Mattijs Jonker, Jeroen van der Ham, Giovane Moura
#### International Conference on Network and Service Management


Electronic government (e-gov) enables citizens and residents to digitally interact with their government via the Internet. Underpinning these services is the Internet Domain Name Systems (DNS), which maps e-gov domain names to Internet addresses. Structuring DNS with multiple levels of redundancy that can withstand stress events such as denial-of-service (DoS) attacks is a challenging task. While the operator community has established best practices to this end, adopting them all involves expert knowledge and resources. In this work, we obtain and study a list of e-gov domain names used by four countries (The Netherlands, Sweden, Switzerland, and the United States) and measure the DNS structuring of these domains. We show the adoption of best practices, inter-country differences such as the use of anycast, and provide recommendations to improve DNS service robustness.

<a href="https://www.sidnlabs.nl/downloads/1o9vqrKcm29tkpVzTj7a0Y/c20df98380d70905d8659e25400967b9/report-dns-egov.pdf">Download</a>




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


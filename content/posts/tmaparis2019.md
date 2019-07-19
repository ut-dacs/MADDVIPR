---
date: 2019-06-20
linktitle: TMA 2019 Paris
title: TMA 2019 Paris
weight: 10
categories: [ "article", "general" ]
tags: ["work"]
---
<img src="/images/paris.jpg"; width="600" /></a>
This week, Raffaele attended to TMA 2019 Paris PhD School and Conference and presented a poster on DNS Time To Live Mismatch Problem.

It was an amazing experience, with a lot of interesting workshops in the PhD School and interesting papers and posters presented at the conference.

Below you can find the abstract and the poster.

### It’s Time To Lie: The DNS TTL Mismatch Problem
The Domain Name System is a hierarchical decentralized and distributed database. The information
available in the DNS are supposed to be coherent through the whole hierarchy. Nevertheless, it could be
possible to have non-coherent data at various levels of the DNS architecture. This happens due to
misconfiguration or administrative choice of DNS Server owners. In this case, the most authoritative
information should be used.
In this work, we would introduce the problem of information mismatch with the case of TTL value
mismatch on NS records. The Time to Live field suggests to the recursive server or to the local resolver for
how long the record should be kept in cache.
The TTL could be useful in DNS DDoS attack mitigation. With a higher TTL, indeed, we make our system
more resilient against DDoS Attack, because a lack of availability of Authoritative Nameservers, due to a
DDoS Attack, has a minor impact on resolvers that can use the data available in their cache.
Unfortunately, the TTL field advice is not respected in some cases. We are currently studying the mismatch
of TTL between parent TLD delegation and child authoritative delegation in NS Records. Our results show a
mismatch in 95% of the .com domain. Moreover, we are looking to the behavior of the DNS server software
in case of mismatch and we are discovering some unexpected results.
<a href="/poster/tma2019.pdf"><img src="/poster/tma2019.png"; width="200" /></a>


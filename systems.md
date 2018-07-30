---
layout: page
title: Distributed Systems
permalink: /systems/
---


Intro
======

My journey in distributed systems began with Bitcoin in 2016. Bitcoin is a software protocol for internet payments. Why are payments important? Well this billion dollar industry is a corner-stone of the global financial system and is responsible for much of its current structure. I found it compelling that I could download the Bitcoin software and immediately participate in a payment network consisting of thousands of computers around the world. Bitcoin is unique because its security relies on cryptography and an incentive mechanism rather than a trusted party. I believe this is significant because it could be used to create a financial system with a core structure without intermediaries that could be more inclusive and competitive. 

I joined MIT's [Digital Currency Initiative](www.dci.mit.edu) to do research in this area and was a researcher for the group as both an undergraduate and graduate student. Joining the DCI led me to discover the field of distributed systems. This area of computer science studies how multiple computers can collaborate to perform a task. It is an exciting prospect: imagine thousands of computers seamlessly working together to take advantage of their collective resources. I started taking systems courses, reading papers and implementing my own software in Go. I also began to see just how different Bitcoin is from nearly every other system. Broadly speaking, the goal of protocols in this field is to allow for one to increase the performance (fault tolerance, availability, throughput, etc.) of the system by adding more machines. A great example is [FaRM](https://dl.acm.org/citation.cfm?id=2815425). FaRM achieves a transnational throughput so great that it could handle the entire world email throughput several times over. Bitcoin, on the other hand, is a different beast. It removes the need for a trusted party - a very hard problem - but this comes at a cost to performance and scalability. Adding more computers to the Bitcoin network, unlike other systems, does not improve performance.

I'm still excited, albeit more realistically, about Bitcoin and cryptocurrencies. Projects such as [Lightening Network](https://github.com/mit-dci/lit) can help Bitcoin scale. I'm also interested in working on other kinds of distributed systems in the future. My work in this space has shown me the promise of using technology as a lever for changing a system, as well as the formidable legal, cultural and technical obstacles that stand in the way. I've described a few of my favorite previous projects from my time at the DCI and MIT below.      

b_verify
======

b_verify is a protocol that I designed and implemented for verifiable management of data using a public ledger. Previous protocols for managing data using public ledgers are expensive, do not provide a convenient interface for building applications and cannot scale. b_verify solves the technical problem of _equivocation_, which allows attackers to present inconsistent data to users. b_verify prevents equivocation efficiently using a carefully chosen data structure and Bitcoin witnessing that allows clients to maintain small cryptographic proofs they have not equivocated.

An important type of application that can be build with b_verify are _publicly verifiable registries_. A registry is a key/value map in which each entry is controlled by a specific set of users. We implement an application for creating trade-able commodity receipts that does not require a trusted thyroid party. b_verify can scale to millions of users with tens of millions of receipts. 

This project started in collaboration with Mark Weber, another student, at the DCI. We were interested in the creating verifiable and trade able receipts, and collaborated with the Inter-American Development Bank to try and explore creating a new protocol. b_verify ultimately became my Master's thesis, and we are currently writing several papers, both technical and high-level about the system. 

Here's my thesis:

[b_verify: Scalable Non-Equivocation for Verifiable Management of Data](/files/dci_thesis.pdf)

A higher-level paper describing one use case: 

[Blockchain and the Value of Operational Transparency](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3078945)


Cryptocurrency
======

For the 6.824 (distributed systems) final project, I decided to work on a new consensus algorithm with my DCI colleague James Lovejoy. We designed and implemented our own proof-of-stake protocol called ECTO that improved on technical problems with previous systems. This project was for fun and academic purposes rather than any sort of money making, and we have open-sourced all of the code.

[ECTO - A Novel Proof-of-Stake Algorithm and Implementation](/files/ecto_paper.pdf)
              

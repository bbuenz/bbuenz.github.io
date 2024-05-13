---
layout: page
permalink: /teaching/
title: Teaching
tags: [teaching]
modified: 8-11-2017
comments: false
---

## CSCI-GA.3033-​107: Cryptography of Blockchains

### Readings:

A Graduate Course in Applied Cryptography, Boneh Shoup (BS) https://toc.cryptobook.us/

Bitcoin and Cryptocurrency Technologies, Narayanan, Bonneau, Felten, Miller, Goldfeder (NBFMG)

https://d28rh4a8wq0iu5.cloudfront.net/bitcointech/readings/princeton_bitcoin_book.pdf

### Homework

[Homework 1](hw/hw1.pdf)
[Homework 2](hw/hw2.pdf)

### Syllabus

- Lecture 1 (1/22): Intro to Blockchains
    - [Slides](lectures/cofb/lecture1.pptx)
    - What are blockchains
    - Signatures and Hash Functions
    - Building a simple blockchain from simple primitives
    - SHA256
    - Schnorr signatures
    - BLS signatures
    - Class overview
    - Reading: BS Chapter 8,13; NBFMG Chapter 1
- Lecture 2 (1/29) Merkle Trees, Vector Commitments, Accumulators and Proof of Storage
    - [Slides](lectures/cofb/lecture2.pptx)
    - BLS signatures (reading last lecture)
    - UTXO vs Account model (transaction format)
    - State Commitments
    - Merkle Tree Inclusion Proofs
    - Merkle Tree Updates
    - Patricia Trees and exclusion proofs
    - UTXO commitment
    - Reading: BS 8.9 NBFMG Chapter 3
- Lecture 3: 2/5 Consensus, Aggregate signatures
    - [Slides](lectures/cofb/lecture3.pptx)
    - RSA accumulators
    - Proof of Work
    - Proof of Stake
    - Randomness
    - Quorum Certificates
    - Aggregate BLS for reducing communication
    - Rouge Key Attacks
    - Reading BS 15.5, [BFS20 (Chapter 4 mainly)](https://eprint.iacr.org/2018/1188), [Compact certificates](https://eprint.iacr.org/2020/1568)
- Lecture 4 (23/4): Aggregate signatures part 2, VDFs and Beacons
	- [Slides](lectures/cofb/lecture4.pptx)
	- BLS rouge key defenses
	- Hash-based certificate of quorum
	- Committee sampling 
	- Randomness beacons
	- Strawman construction
	- VDFs abstractly
	- Group based VDFs
	- Reading [Verifiable Delay Functions](https://eprint.iacr.org/2018/601) Sections 1-3, [Survey of 2 VDFs](https://eprint.iacr.org/2018/712.pdf) 
- 2/19 President's day
- Lecture 5: 2/26 Optimistic Rollups and VID
    - [Slides](lectures/cofb/lecture5.pptx)
    - Fraud proofs
    - Data Availability
    - Error Correcting Codes
    - Polynomial Commitments
    - Verifiable Information Dispersal
    - Reading: [KZG](https://www.iacr.org/archive/asiacrypt2010/6477178/6477178.pdf) 
- Lecture 6: 3/4 KZG, and Light Clients
    - [Slides](lectures/cofb/lecture6.pptx)
    - KZG commitment
    - Light client sampling (Danksharding)
    - Sync committee
    - Long range attacks
    - SVP client
    - Flyclient
    - Reading: [KZG](https://www.iacr.org/archive/asiacrypt2010/6477178/6477178.pdf), [Flyclient](https://eprint.iacr.org/2019/226.pdf) 
- Lecture 7: 3/11 Threshold Cryptography and key security
    - [Slides](lectures/cofb/lecture7.pptx)
    - Flyclient
    - Key security
    - HD Wallets
    - Shamir Secret Sharing
    - Threshold signatures
- Spring break
- Lecture 8: 3/25 Private Blockchains and Zero-Knowledge
    - [Slides](lectures/cofb/lecture8.pptx)
    - Privacy on Blockchains
    - Mixers
    - Defining Zero-Knowledge
    - Defining SNARKs
    - Tornado Cash
- Lecture 9: 4/1 Zero-Knoledge Proofs part 1 (Sigma Protocols)
    - [Slides](lectures/cofb/lecture9.pptx)
    - ZK-applications
    - ZK-definitions
    - Special Soundness
    - Simulation
    - Sigma protocols for circuits
    - Reading: BS Chapter 19 and 20
- Lecture 10: 4/10 SNARKs part 2
    - [Slides](lectures/cofb/lecture10.pptx)
    - ZK-Rollups
    - Poly IOPs
    - Plonk 
- Lecture 11: 4/15 Post-quantum cryptography for blockchains (Guest lecture Nick Spooner)
- Lecture 12: 4/22 Recursive proofs and succinct blockchains
    - [Slides](lectures/cofb/lecture12.pptx)
    - FRI
    - Recursive proofs
    - Succinct blockchains
- Lecture 13: 4/29 Recursive proofs part 2
    - [Slides](lectures/cofb/lecture13.pptx)
    - zkEVM
    - Circuit friendly hash functions
    - Lookup arguments
    - Memory checking
    - Folding
    - Reading: [Vitalik Blog](https://vitalik.eth.limo/general/2022/08/04/zkevm.html), [Poseidon Hash](https://www.poseidon-hash.info/), [Lookup](https://eprint.iacr.org/2022/1530.pdf), [Memory Checking](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=185352), [Folding 1](https://eprint.iacr.org/2020/1618), [Folding 2](https://eprint.iacr.org/2021/370)
- Lecture 14: 5/6 Optional topic: Folding, MPC and future crypto
    - [Slides](lectures/cofb/lecture14.pptx)
    - Accumulation/Folding
    - MPC
    - Reading: BS Chapter 23.1-23.3, [Nova](https://eprint.iacr.org/2021/370), [ProtoStar](https://eprint.iacr.org/2023/620)

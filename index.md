---
layout: home2
description: "Benedikt Bünz's website"
tags: [Jekyll, theme, responsive, blog, template]
image:
  feature: road.jpg
modified: 8-7-2014
comments: false
---
# About Me:
--I am a second-year PhD student in the [Applied Crypto Group](https://crypto.stanford.edu) and am advised by [Dan Boneh](https://crypto.stanford.edu/~dabo)

--My main reserach interests are in cryptography, game theory and cryptocurrencies.

--I am an avid runner and train and compete for [Strava Track Club](http://stravatrackclub.com)

# Publications [Google Scholar](http://scholar.google.es/citations?user={{ site.owner.google_scholar }}):
{: #publications }

<h2>Cryptography and Cryptocurrencies</h2>
<h3>Bulletproofs: Short Proofs for
Confidential Transactions and More</h3>
Authors: B. Bünz, [J. Bootle](http://www0.cs.ucl.ac.uk/staff/J.Bootle/), [D. Boneh](https://crypto.stanford.edu/~dabo), [Andrew Poelstra](https://www.wpsoftware.net/andrew/), [Pieter Wuille](https://blockstream.com/team/pieter-wuille/) and [Greg Maxwell](https://blockstream.com/team/greg-maxwell/)

Published at Oakland 2018

[Paper](https://eprint.iacr.org/2017/1066)

[Talk at BPASE 18](https://www.youtube.com/watch?v=gZjDKgR4dw8)

[Slides](https://cyber.stanford.edu/sites/default/files/bpase18.pptx)

[Java reference implementation](https://github.com/bbuenz/BulletProofLib)

[libsecp256k1 implementation by Andrew Poelstra](https://github.com/apoelstra/secp256k1-mw/tree/bulletproofs)

TLDR: Confidential transactions are Bitcoin transactions which are publicly verifiable but do not reveal the amounts that are transferred. They rely on cryptographic commitments and so called zero-knowledge proofs of knowledge. We present a new kind of zero-knowledge proof which is much more efficient and can be used to drastically reduce the size of confidential transactions. On a more technical note bulletproofs are non-interactive zero knowledge proofs without trusted setup and
with only logarithmic proof size. Proving and verification cost are linear with low constant overhead.

<h3>Provisions: Privacy-preserving proofs of solvency for Bitcoin exchanges</h3>
Authors: [G. Dagher](http://cs.boisestate.edu/~gdagher/), B. Bünz, [J.Bonneau](http://www.jbonneau.com/), [J.Clark](https://users.encs.concordia.ca/~clark/) and [D. Boneh](https://crypto.stanford.edu/~dabo)

Published at CCS 2015

[Paper](https://eprint.iacr.org/2015/1008.pdf)

[Code](https://github.com/bbuenz/provisions)

[Blog by Joseph Bonneau](https://freedom-to-tinker.com/2015/10/26/provisions-how-bitcoin-exchanges-can-prove-their-solvency/)

[Talk at Next Context Conference](https://youtu.be/-zku26GNCa4?t=28m52s)

TLDR: How can a Bitcoin exchange proof that they have enough funds to satisfy all their customers demands without revealing the customers balances, the bitcoin addresses they control or even the total amount of bitcoin they have.

<h3>Proofs-of-delay and randomness beacons in Ethereum</h3>
Authors: B. Bünz, [S. Goldfeder](http://www.stevengoldfeder.com), [J. Bonneau](http://www.jbonneau.com)

Presented at [IEEE S&B Workshop](http://prosecco.gforge.inria.fr/ieee-blockchain2016)

[Paper](http://www.jbonneau.com/doc/BGB17-IEEESB-proof_of_delay_ethereum.pdf)

[Code](https://github.com/bbuenz/VerifiableBeacon)

[Talk at CESC](https://www.youtube.com/watch?v=kK4qN2K44Ms)

[Slides](https://drive.google.com/file/d/0B5PcPC6ZC_Gyb3V6NnRMZ2VZMFU/view)

TLDR: We show how one can generate an unpredictable randomness beacon that is publicly verifiable using a blockchain. The beacon can be used to verify the correct execution of randomized algorithms such as lotteries. The novel property of the beacon is that it is publicly verifiable in that a verifier is convinced that the beacon was unpredictable even if she did not partake in the generation of the beacon and without any trust assumptions. We also show how we can enable interactive verification using an efficient smart contract.

<h2>Game Theory (Combinatorial Auctions)</h2>
<h3>Designing Core-Selecting Payment Rules: A Computational Search Approach</h3>
Authors: B. Bünz, [B. Lubin](http://people.bu.edu/blubin/), [S. Seuken](https://www.ifi.uzh.ch/en/ce/people/seuken.html)

Published at [EC 2018](http://www.sigecom.org/ec18/)

[Paper](https://ssrn.com/abstract=3178454)

<h3>A Faster Core Constraint Generation Algorithm for Combinatorial Auctions</h3>
Authors: B. Bünz, [B. Lubin](http://people.bu.edu/blubin/), [S. Seuken](https://www.ifi.uzh.ch/en/ce/people/seuken.html)

Published at [AAAI 2015](www.aaai.org)

[Paper](https://aaai.org/ocs/index.php/AAAI/AAAI15/paper/view/10033/9376)

[Slides]({{ site.url }}/papers/aaaipresentation.pptx)

TLDR: We significantly improve on the current state of the art algorithm for computing combinatorial auctions. These auctions were multiple related goods are sold in the same auction are for example used to allocated spectrum to cellular companies around the world. These auctions often generate billions of dollars in revenue but are often limited to a small number of bidders and goods. Faster algorithms for computing their outcome will enable larger scale applications.
<h3>Computing Bayes-Nash Equilibria in Combinatorial Auctions with Continuous Value and Action Spaces</h3>
Authors: [V. Bosshard](http://www.ifi.uzh.ch/en/ce/people/bosshard.html), B. Bünz, [B. Lubin](http://people.bu.edu/blubin/), [S. Seuken](https://www.ifi.uzh.ch/en/ce/people/seuken.html)

Published at IJCAI 2017

[Paper](https://www.ijcai.org/proceedings/2017/18)

<h3>LLG BNEs (Working Paper)</h3>

Authors: [B. Lubin](http://people.bu.edu/blubin/), B. Bünz, [S. Seuken](https://www.ifi.    uzh.ch/en/ce/people/seuken.html)

[Extended abstract published at AMMA 2015](http://eudl.eu/proceedings/AMMA/2015)

[Working Paper](http://www.ifi.uzh.ch/ce/publications/Fairness_and_Incentives.pdf)

<br>

<h2>Artificial Intelligence</h2>
<h3>Learning a SAT Solver from Single-Bit Supervision</h3>
Authors: [D. Selsam](http://stanford.edu/~dselsam/), M. Lamm, B. Bünz, [P. Liang](https://cs.stanford.edu/~pliang/), [L. de Moura](http://leodemoura.github.io/),[D. Dill](https://profiles.stanford.edu/david-dill)

[Paper](https://arxiv.org/abs/1802.03685)

[Talk by Daniel Selsam at Microsoft Research](https://www.youtube.com/watch?v=EqvzIGY_bI4)

TLDR: We develop a neural network based solver for finding satisfying assingments to boolean formulas (SAT solver). At training time the network is given satisfying formulas and only the information of whether the formula has a solution or not. Despite this minimal supervision we are able to directly read of satisftying assignments from the activations of the network if it classifies a formula as satisfiable. Additionally we can even find contradictions if the formula is unsatisfiable. Given
that classifying boolean formulas is an NP-complete problem this an interesting exploration into the abilities and flexibilities of neural network and also raises interesting possibilities of using neural networks in the development of state of the art SAT solvers.

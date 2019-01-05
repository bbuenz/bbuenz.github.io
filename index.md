---
layout: home2
description: "Benedikt Bünz's website"
tags: [Jekyll, theme, responsive, blog, template]
image:
  feature: road.jpg
modified: 8-7-2018
comments: false
---
# About Me:
--I am a third-year PhD student in the [Applied Crypto Group](https://crypto.stanford.edu) and am advised by [Dan Boneh](https://crypto.stanford.edu/~dabo)

--My main research interests are in cryptography, game theory and cryptocurrencies.

--I am an avid runner and train and compete for [Strava Track Club](http://stravatrackclub.com)

# Publications ([Google Scholar](http://scholar.google.es/citations?user={{ site.owner.google_scholar }})):
{: #publications }
<h2>Cryptography and Cryptocurrencies</h2>

<p>
<div id="cryptoacordion" role="tablist">
  <div class="card">
<div class="card-header" role="tab" id="accumulatorsHeading">
<h5 class="mb-0">
  <a  data-toggle="collapse" href="#accumulators" aria-expanded="false" aria-controls="collapseOne">
  Batching Techniques for Accumulators with Applications to IOPs and Stateless Blockchains
  </a>
</h5>
</div>
<div id="accumulators" class="collapse show" role="tabpanel" aria-labelledby="accumulatorsHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
[D. Boneh](https://crypto.stanford.edu/~dabo),  B. Bünz and [B.Fisch](https://sites.google.com/site/benafisch/)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2018/1188)
</dt>
<dt markdown="1">
[Talk at Scaling Bitcoin 18](https://youtu.be/IMzLa9B1_3E?t=3515)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/accumulators.pptx)
</dt>
<dt>TLDR</dt>
<dd>
Accumulators are short commitment to a set that support efficient inclusion and exclusion proofs. We present several new batching techniques for accumulators and positional vector commitments in group of unknown order. Our techniques can be used in a stateless blockchain design where all users and miners only require a constant amount of storage. We also present a new vector commitment which can significantly reduce the proof size of IOP instantiations, such as STARKs.
</dd>

</dl>
</div>
</div>
</div>

<div class="card">
<div class="card-header" role="tab" id="zetherHeading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#zether" aria-expanded="false" aria-controls="collapseOne">
  Zether: Towards Privacy in a Smart Contract World
  </a>
</h5>
</div>
<div id="zether" class="collapse" role="tabpanel" aria-labelledby="zetherHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
B. Bünz, [S. Agrawal](https://shashank-agrawal.com/), [M. Zamani](http://mahdiz.com/) and [D. Boneh](https://crypto.stanford.edu/~dabo)
</dd>
<dt markdown="1">
[Paper]({{ site.url }}/papers/zether.pdf)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/zether.pptx)
</dt>
<dt>TLDR</dt>
<dd>
We propose Zether, a private payment mechanism that is compatible with Ethereum and other account-based payment systems. Zether can provide both confidentiality (by hiding payment amounts) and anonymity (by hiding the identities of senders and recipients).  Zether is designed to be inter-operable with arbitrary smart contracts to support applications such as sealed-bid auctions, private payment channels, stake voting, and confidential proof-of-stake. Zether uses an extension to Bulletproofs called Sigma-Bullets which combines Bulletproofs with Sigma protocols.
</dd>

</dl>
</div>
</div>
</div>
<div class="card">
<div class="card-header" role="tab" id="vdfsurveyHeading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#vdfsurvey" aria-expanded="false" aria-controls="collapseOne">
  A Survey of 2 Verifiable Delay Functions
  </a>
</h5>
</div>
<div id="vdfsurvey" class="collapse" role="tabpanel" aria-labelledby="vdfsurveyHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
[D. Boneh](https://crypto.stanford.edu/~dabo),  B. Bünz and [B.Fisch](https://sites.google.com/site/benafisch/)
</dd>
<dt markdown="1">
[Paper](https://crypto.stanford.edu/~dabo/pubs/papers/VDFsurvey.pdf)
</dt>
<dt>TLDR</dt>
<dd>
We briefly survey two beautiful VDF constructions by Wesolowski and Pietrzak. We give a new computational security proof for one of them and compare their security assumptions.
</dd>

</dl>
</div>
</div>
</div>
<div class="card">
<div class="card-header" role="tab" id="vdfHeading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#vdf" aria-expanded="false" aria-controls="collapseOne">
  Verifiable Delay Functions
  </a>
</h5>
</div>
<div id="vdf" class="collapse" role="tabpanel" aria-labelledby="vdfHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
[D. Boneh](https://crypto.stanford.edu/~dabo), [J.Bonneau](http://www.jbonneau.com/), B. Bünz and [B.Fisch](https://sites.google.com/site/benafisch/)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2018/601) (Published at CRYPTO 2018)
</dt>
<dt>
<a href="https://www.youtube.com/watch?v=_-feyaZZjEw">Talk by Ben Fisch at Crypto 2018</a>
</dt>
<dt>TLDR</dt>
<dd>
We introduce verifiable delay functions (VDFs) which have 3 key properties: They are a functions so for every input there is a unique output. Evaluation incurs a delay, i.e. it takes a significant amount of time even on a highly parallel machine. VDFs are verifiable such that given a proof a verifier can efficiently check that the VDF was evaluated correctly. VDFs have many applications from randomness beacons to proofs of replication and cointossing.
</dd>

</dl>
</div>
</div>
</div>
<div class="card">
<div class="card-header" role="tab" id="bpHeading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#bulletproofs" aria-expanded="false" aria-controls="collapseOne">
Bulletproofs: Short Proofs for
Confidential Transactions and More
  </a>
</h5>
</div>
<div id="bulletproofs" class="collapse" role="tabpanel" aria-labelledby="bpHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
B. Bünz, [J. Bootle](http://www0.cs.ucl.ac.uk/staff/J.Bootle/), [D. Boneh](https://crypto.stanford.edu/~dabo), [Andrew Poelstra](https://www.wpsoftware.net/andrew/), [Pieter Wuille](https://blockstream.com/team/pieter-wuille/) and [Greg Maxwell](https://blockstream.com/team/greg-maxwell/)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2017/1066) (Published at IEEE S&P (Oakland) 2018)
</dt>
<dt markdown="1">
[Talk at IEEE S&P](https://www.youtube.com/watch?v=Adrh6BCc_Ao)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/bulletproofs.pptx)
</dt>
<dt markdown="1">
Implementations
</dt>
<dd markdown="1">
[Java reference implementation](https://github.com/bbuenz/BulletProofLib)

[libsecp256k1 implementation by Andrew Poelstra](https://github.com/apoelstra/secp256k1-mw/tree/bulletproofs)
</dd>
<dt>TLDR</dt>

<dd>
Confidential transactions are Bitcoin transactions which are publicly verifiable but do not reveal the amounts that are transferred. They rely on cryptographic commitments and so called zero-knowledge proofs of knowledge. We present a new kind of zero-knowledge proof which is much more efficient and can be used to drastically reduce the size of confidential transactions. On a more technical note bulletproofs are non-interactive zero knowledge proofs without trusted setup and
with only logarithmic proof size. Proving and verification cost are linear with low constant overhead.
</dd>

</dl>
</div>
</div>
</div>
<div class="card">
<div class="card-header" role="tab" id="provisionsheading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#provisions" aria-expanded="true" aria-controls="collapseOne">
Provisions: Privacy-preserving proofs of solvency for Bitcoin exchanges
  </a>
</h5>
</div>
<div id="provisions" class="collapse" role="tabpanel" aria-labelledby="provisionsheading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
[G. Dagher](http://cs.boisestate.edu/~gdagher/), B. Bünz, [J.Bonneau](http://www.jbonneau.com/), [J.Clark](https://users.encs.concordia.ca/~clark/) and [D. Boneh](https://crypto.stanford.edu/~dabo)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2015/1008) (Published at CCS 2015)
</dt>
<dt markdown="1">
[Talk at Next Context Conference](https://youtu.be/-zku26GNCa4?t=28m52s)
</dt>
<dt markdown="1">
Implementations
</dt>
<dd markdown="1">
[Java reference implementation](https://github.com/bbuenz/provisions)
</dd>
<dt markdown="1">
[Blog by Joseph Bonneau](https://freedom-to-tinker.com/2015/10/26/provisions-how-bitcoin-exchanges-can-prove-their-solvency/)
</dt>
<dt>TLDR</dt>

<dd>
How can a Bitcoin exchange proof that they have enough funds to satisfy all their customers demands without revealing the customers balances, the bitcoin addresses they control or even the total amount of bitcoin they have.
</dd>

</dl>
</div>
</div>
</div>

<div class="card">
<div class="card-header" role="tab" id="delayheading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#delay" aria-expanded="false" aria-controls="collapseOne">
  Proofs-of-delay and randomness beacons in Ethereum
  </a>
</h5>
</div>
<div id="delay" class="collapse" role="tabpanel" aria-labelledby="delayheading" data-parent="#cryptoacordion">
      <div class="card-body" >

Presented at <a href="http://prosecco.gforge.inria.fr/ieee-blockchain2016">IEEE S&B Workshop</a>
<dl>
<dt>Authors</dt>
<dd markdown="1">
B. Bünz, [S. Goldfeder](http://www.stevengoldfeder.com), [J. Bonneau](http://www.jbonneau.com)
</dd>
<dt markdown="1">
[Paper](http://www.jbonneau.com/doc/BGB17-IEEESB-proof_of_delay_ethereum.pdf)
</dt>
<dt markdown="1">
[Talk at CESC](https://www.youtube.com/watch?v=kK4qN2K44Ms)
</dt>
<dt markdown="1">
[Slides](https://drive.google.com/file/d/0B5PcPC6ZC_Gyb3V6NnRMZ2VZMFU/view)
</dt>
<dt markdown="1">
[Code](https://github.com/bbuenz/VerifiableBeacon)
</dt>

<dt>TLDR</dt>

<dd>
We show how one can generate an unpredictable randomness beacon that is publicly verifiable using a blockchain. The beacon can be used to verify the correct execution of randomized algorithms such as lotteries. The novel property of the beacon is that it is publicly verifiable in that a verifier is convinced that the beacon was unpredictable even if she did not partake in the generation of the beacon and without any trust assumptions. We also show how we can enable interactive verification using an efficient smart contract.
</dd>

</dl>
</div>
</div>
</div>

  </div>
  </p>

  <h2>Game Theory (Combinatorial Auctions)</h2>
<p>
 <div id="gameacordion" role="tablist">
  <div class="card">
<div class="card-header" role="tab" id="cabneheading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#cabne" aria-expanded="false" aria-controls="collapseOne">
Designing Core-Selecting Payment Rules: A Computational Search Approach  </a>
</h5>
</div>
<div id="cabne" class="collapse" role="tabpanel" aria-labelledby="cabneheading" data-parent="#gameacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
B. Bünz, [B. Lubin](http://people.bu.edu/blubin/), [S. Seuken](https://www.ifi.uzh.ch/en/ce/people/seuken.html)
</dd>
<dt markdown="1">
[Paper](https://ssrn.com/abstract=3178454) (Published at [EC 2018](http://www.sigecom.org/ec18/))
</dt>

<dt>TLDR</dt>
<dd>
We systematically look for and evaluate payment rules for combinatorial auctions. Our evaluation is done by computing BNEs for the payment rule in various domains. We find new payment rules that performe significantly better than the currently used ones.
</dd>

</dl>
</div>
</div>
</div>

 <div class="card">
<div class="card-header" role="tab" id="ccgheading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#ccg" aria-expanded="false" aria-controls="collapseOne">
A Faster Core Constraint Generation Algorithm for Combinatorial Auctions </a>
</h5>
</div>
<div id="ccg" class="collapse" role="tabpanel" aria-labelledby="ccgheading" data-parent="#gameacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
B. Bünz, [B. Lubin](http://people.bu.edu/blubin/), [S. Seuken](https://www.ifi.uzh.ch/en/ce/people/seuken.html)
</dd>
<dt markdown="1">
[Paper](https://aaai.org/ocs/index.php/AAAI/AAAI15/paper/view/10033/9376) (Published at AAAI 2015)
</dt>
<dt markdown="1">
	[Slides]({{ site.url }}/papers/aaaipresentation.pptx)
</dt>

<dt>TLDR</dt>
<dd>
	We significantly improve on the current state of the art algorithm for computing combinatorial auctions. These auctions were multiple related goods are sold in the same auction are for example used to allocated spectrum to cellular companies around the world. These auctions often generate billions of dollars in revenue but are often limited to a small number of bidders and goods. Faster algorithms for computing their outcome will enable larger scale applications.
</dd>
</dl>
</div>
</div>
</div>


 <div class="card">
<div class="card-header" role="tab" id="fastbneHeading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#fastbne" aria-expanded="false" aria-controls="collapseOne">
Computing Bayes-Nash Equilibria in Combinatorial Auctions with Continuous Value and Action Spaces</a>
</h5>
</div>
<div id="fastbne" class="collapse" role="tabpanel" aria-labelledby="fastbneHeading" data-parent="#gameacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
[V. Bosshard](http://www.ifi.uzh.ch/en/ce/people/bosshard.html), B. Bünz, [B. Lubin](http://people.bu.edu/blubin/), [S. Seuken](https://www.ifi.uzh.ch/en/ce/people/seuken.html)
</dd>
<dt markdown="1">
[Paper](https://www.ijcai.org/proceedings/2017/18) (Published at IJCAI 2017)
</dt>


<dt>TLDR</dt>
<dd>
We design several new techniques for quickly computing bayes nash equilibria for combinatorial auctions.
</dd>

</dl>


</div>
</div>
</div>


 <div class="card">
<div class="card-header" role="tab" id="fairnessHeading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#fairness" aria-expanded="false" aria-controls="collapseOne">
New Core-Selecting Payment Rules
with Better Fairness and Incentive Properties</a>
</h5>
</div>
<div id="fairness" class="collapse" role="tabpanel" aria-labelledby="fairnessHeading" data-parent="#gameacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
[B. Lubin](http://people.bu.edu/blubin/), B. Bünz, [S. Seuken](https://www.ifi.uzh.ch/en/ce/people/seuken.html)
</dd>
<dt markdown="1">
	[Working Paper](http://www.ifi.uzh.ch/ce/publications/Fairness_and_Incentives.pdf)
</dt>
<dt markdown="1">
[Extended abstract published at AMMA 2015](http://eudl.eu/proceedings/AMMA/2015)
</dt>



</dl>
</div>
</div>
</div>

</div>
</p>







<h2>Artificial Intelligence</h2>
<p>
 <div class="card">
<div class="card-header" role="tab" id="neurosatheader">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#neurosat" aria-expanded="false" aria-controls="collapseOne">
Learning a SAT Solver from Single-Bit Supervision
</a>
</h5>
</div>
<div id="neurosat" class="collapse" role="tabpanel" aria-labelledby="neurosatheader" >
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
[D. Selsam](http://stanford.edu/~dselsam/), M. Lamm, B. Bünz, [P. Liang](https://cs.stanford.edu/~pliang/), [L. de Moura](http://leodemoura.github.io/),[D. Dill](https://profiles.stanford.edu/david-dill)
</dd>
<dt markdown="1">
[Paper](https://arxiv.org/abs/1802.03685) (To appear at ICLR 2019)
</dt>
<dt markdown="1">
[Talk by Daniel Selsam at Microsoft Research](https://www.youtube.com/watch?v=EqvzIGY_bI4)
</dt>

<dt>
	[Code](https://github.com/dselsam/neurosat)
</dt>
<dt>TLDR</dt>
<dd>
	We develop a neural network based solver for finding satisfying assignments to boolean formulas (SAT solver). At training time the network is given satisfying formulas and only the information of whether the formula has a solution or not. Despite this minimal supervision we are able to directly read of satisfying assignments from the activations of the network if it classifies a formula as satisfiable. Additionally we can even find contradictions if the formula is unsatisfiable. Given
that classifying boolean formulas is an NP-complete problem this an interesting exploration into the abilities and flexibilities of neural network and also raises interesting possibilities of using neural networks in the development of state of the art SAT solvers.
</dd>


</dl>
</div>
</div>
</div>
</p>

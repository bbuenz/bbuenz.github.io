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

--My main research focusses on the science of blockchains using tools from applied cryptography, game theory and consensus. I get most excited about problems that both require novel theoretical insights and also have real-world applications.

--I am a cofounder and chief scientist of [Espresso Systems](https://espressosys.com).

--I'll be joining NYU Courant as an Assistant Professor in Computer Science starting in the Fall of 2023.

# Teaching
--I co-instruct a course on Cryptocurrencies and Blockchain Technologies [CS 251](https://cs251.stanford.edu/).

# Publication Highlights

--[Ph.D. Thesis](/papers/thesis-benedikt.pdf) Improving the Privacy, Scalability, and Ecological Impact.

--[Bulletproofs](#bpHeading) is a zero-knowlede proof system that has extremly short proofs while requiring minimal trust assumptions. It is general purpose but specificially designed for confidential blockchain transactions. Bulletproofs is deployed on multiple blockchains and secures tens of thousands of private transactions on blockchains like Monero or Mobilecoin. 

--[Verifiable Delay Functions](#vdfHeading) or VDFs are functions that take a long time to evaluate but are efficient to verify. VDFs have many applications and are a key building block for enviormentally friendly consensus mechanisms. They are being used in blockchain systems like Chia and Filecoin and are a part of the Ethereum 2.0 design. The [VDF alliance](vdfalliance.org) is an industry alliance focussed on building VDF hardware. 

--[HyperPlonk](#hpHeading) is a SNARK that is specifically designed for proving large complex statements. It removes the requirment for FFTs which makes HyperPlonk more scalable and parallelizable. It also enables high-degree custom gates for complex circuits, such as ZKEVMs.

# Publications ([Google Scholar](http://scholar.google.es/citations?user={{ site.owner.google_scholar }})):
{: #publications }
<h2>Cryptography and Cryptocurrencies</h2>

<p>
<div id="cryptoacordion" role="tablist">
  <div class="card">
<div class="card-header" role="tab" id="psHeading">
<h5 class="mb-0">
  <a   data-toggle="collapse" href="#protostar" aria-expanded="true" aria-controls="collapseOne">
  ProtoStar: Generic Efficient Accumulation/Folding for Special Sound Protocols

  </a>
</h5>
</div>
<div id="protostar" class="collapse show" role="tabpanel" aria-labelledby="psHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
B. Bünz, Binyi Chen
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2023/620)  
</dt>
<dt>TLDR</dt>
<dd>
ProtoStar is an Incrementale Verifiable Computation Scheme based on the [accumulation](#wacc)/folding approach. It is constructed using a general, but highly efficient recipe for constructing accumulation schemes from any special-sound, algebraic protocol. It enables the use of high-degree gates and lookups, all while requiring only 3 elliptic curve scalar multiplication inside the recursive circuit. 
</dd>

</dl>
</div>
</div>
</div>

  <div class="card">
<div class="card-header" role="tab" id="hpHeading">
<h5 class="mb-0">
  <a class="collapsed"  data-toggle="collapse" href="#hp" aria-expanded="false" aria-controls="collapseOne">
 HyperPlonk: Plonk with Linear-Time Prover and High-Degree Custom Gates 
  </a>
</h5>
</div>
<div id="hp" class="collapse" role="tabpanel" aria-labelledby="hpHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
Binyi Chen, B. Bünz, [Dan Boneh](https://crypto.stanford.edu/~dabo/), and [Zhenfei Zhang](https://zhenfeizhang.github.io/)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2022/1355.pdf) (Published at EUROCRYPT 2023) 
</dt>
<dt markdown="1">
[Talk at ZK Summit](https://www.youtube.com/watch?v=2JDBD5oMS0w)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/hp.pptx)
</dt>
<dt>TLDR</dt>
<dd>
Plonk is a recently developed proof system that has received a lot of attention due to its efficienct, low trust assumption, and customizability. We significantly improve on Plonk by building Hyperplonk. Hyperplonk removes the costlies component of Plonk (Fast Fourier Transforms). It also adds the ability to build proofs for circuits with high-degree custom gates.
</dd>

</dl>
</div>
</div>
</div>

  <div class="card">
<div class="card-header" role="tab" id="vzexeHeading">
<h5 class="mb-0">
  <a class="collapsed"  data-toggle="collapse" href="#vzexe" aria-expanded="false" aria-controls="collapseOne">
  VERI-ZEXE: Decentralized Private Computation with Universal Setup
  </a>
</h5>
</div>
<div id="vzexe" class="collapse" role="tabpanel" aria-labelledby="vzexeHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
Alex Xiong, Binyi Chen, Zhenfei Zhang, B. Bünz, B. Fisch, Fernando Krell, and Philippe Camacho
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2022/802) (To appear at CCS 2023) 
</dt>
<dt>TLDR</dt>
<dd>
Traditional blockchain systems execute program state transitions on-chain, requiring each network node participating in state-machine replication to re-compute every step of the program when validating transactions. This limits both scalability and privacy. Recently, Bowe et al. introduced a primitive called decentralized private computation (DPC) and provided an instantiation called ZEXE, which allows users to execute arbitrary computations off-chain without revealing the program logic to the network. Moreover, transaction validation takes only constant time, independent of the off-chain computation. However, ZEXE required a separate trusted setup for each application, which is highly impractical. Prior attempts to remove this per-application setup incurred significant performance loss.
We propose a new DPC instantiation VERI-ZEXE that is highly efficient and requires only a single universal setup to support an arbitrary number of applications. Our benchmark improves the state-of-the-art by 9x in transaction generation time and by 3.4x in memory usage. Along the way, we also design efficient gadgets for variable-base multi-scalar multiplication and modular arithmetic within the plonk constraint system, leading to a Plonk verifier gadget using only ∼ 21k plonk constraints.
</dd>

</dl>
</div>
</div>
</div>

  <div class="card">
<div class="card-header" role="tab" id="cszHeading">
<h5 class="mb-0">
  <a class="collapsed"  data-toggle="collapse" href="#csz" aria-expanded="false" aria-controls="collapseOne">
  Schwartz-Zippel for multilinear polynomials mod N
  </a>
</h5>
</div>
<div id="csz" class="collapse" role="tabpanel" aria-labelledby="cszHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
B. Bünz, Ben Fisch
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2022/458.pdf) 
</dt>
<dt>TLDR</dt>
<dd markdown="1">
The famous Schwartz-Zippel Lemma bounds the probability that a non-zero multi-variate polynomial over a field evaluates to 0 at a random point. We proof an extension of the lemma that holds modulo a composite. The lemma applies to multi-linear polynomials that are co-prime with the modulus. We then use the lemma to prove that a lattice version of [Bulletproofs](#bulletproofs) is secure and the same proof also closes a crucial gap in the security proof of [DARK](#darks).
</dd>

</dl>
</div>
</div>
</div>
  <div class="card">
<div class="card-header" role="tab" id="nidarHeading">
<h5 class="mb-0">
  <a  class="collapsed" data-toggle="collapse" href="#nidar" aria-expanded="false" aria-controls="collapseOne">
Non-Interactive Differentially Anonymous Router
  </a>
</h5>
</div>
<div id="nidar" class="collapse" role="tabpanel" aria-labelledby="nidarHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
B. Bünz, [Y. Hu](https://huyuncong.com/),[Shin’ichiro Matsuo](https://people.cs.georgetown.edu/matsuo/), [E. Shi](http://elaineshi.com/) 
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2021/1242) (preprint) 
</dt>
<dt>TLDR</dt>
<dd>
We built upon the recent work by Shi and Wu to build a non-interactive anonymour router. A non-interactive untrusted router receives n encrypted ciphertexts and converts them to n transformed ciphertexts that can be decrypted by a set of receivers. The ciphertexts are shuffled according to a permutation that is determined in a one-time trusted setup. 
We show that with a relaxed differentially private security notion a non-interactive router can be achieved with sub-quadratic router work.
</dd>

</dl>
</div>
</div>
</div>
  <div class="card">
<div class="card-header" role="tab" id="waccHeading">
<h5 class="mb-0">
  <a class="collapsed"  data-toggle="collapse" href="#wacc" aria-expanded="false" aria-controls="collapseOne">
  Proof-Carrying Data without Succinct Arguments
  </a>
</h5>
</div>
<div id="wacc" class="collapse" role="tabpanel" aria-labelledby="waccHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
B. Bünz, [A. Chiesa](https://people.eecs.berkeley.edu/~alexch/), W. Lin, [P. Mishra](http://people.eecs.berkeley.edu/~pratyushmishra/) and [N. Spooner](http://people.eecs.berkeley.edu/~spooner/)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2020/1618) (Published at CRYPTO 2021) 
</dt>
<dt markdown="1">
[Talk at CRYPTO](https://www.youtube.com/watch?v=hdmR4wSwryQ)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/wacc.pptx)
</dt>
<dt>TLDR</dt>
<dd>
Proof-carrying data (PCD) is a powerful cryptographic primitive that enables mutually distrustful
parties to perform distributed computations that run indefinitely. Known approaches to construct PCD are
based on succinct non-interactive arguments of knowledge (SNARKs) that have a succinct verifier or a
succinct accumulation scheme for their proofs.
In this paper we show how to obtain PCD without relying on SNARKs. We construct a PCD
scheme given any non-interactive argument of knowledge (e.g., with linear-size proofs) that has a split
accumulation scheme, which is a weak form of accumulation that we introduce.
We additionally construct a transparent non-interactive argument of knowledge for R1CS whose
accumulation is verifiable via a constant number of group and field operations. This leads, via the random
oracle heuristic and our result above, to efficiency improvements for PCD. Along the way, we construct a
split accumulation scheme for a simple polynomial commitment scheme based on Pedersen commitments.
Our results are supported by a modular and efficient implementation.
</dd>

</dl>
</div>
</div>
</div>
  <div class="card">
<div class="card-header" role="tab" id="ippHeading">
<h5 class="mb-0">
  <a  class="collapsed" data-toggle="collapse" href="#ipp" aria-expanded="false" aria-controls="collapseOne">
  Proofs for Inner Pairing Products and Applications
  </a>
</h5>
</div>
<div id="ipp" class="collapse" role="tabpanel" aria-labelledby="ippHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
B. Bünz, M. Maller, [P. Mishra](http://people.eecs.berkeley.edu/~pratyushmishra/), [Nirvan Tyagi](https://www.cs.cornell.edu/~tyagi/) and Psi Vesely
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2019/1177) (Published at ASIACRYPT 2021) 
</dt>
<dt markdown="1">
[Talk at Simons Institute](https://www.youtube.com/watch?v=slm5sL3IgGo)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/InnerPairingProducts.pptx)
</dt>
<dt markdown="1">
[Implementation](https://github.com/arkworks-rs/ripp)
</dt>
<dt>TLDR</dt>
<dd>
We present several proof systems (innner pairing products) for proving algebraic relations over pairing equations. These proof systems efficiently allow a prover to show that committed group elements satisfy certain bilinear (pairing) equalities. We present them as a generalization of the inner-product argument of Bulletproofs. We specialize and optimize them for several highly relevant applications. 
Firstly, we built the first succinct polynomial commitment scheme where the evaluation prover only has <b>additive</b> overhead over evaluating the polynomial. The commitment scheme has both a transparent variant with square root verifier time and one with universal updatable setup with logarithmic verifier time. 
As described in the <a href="#darks">DARK paper</a> polynomial commitments can be used to build general purpose SNARKS.
Additionally, we show that the inner pairing product can be used to efficiently outsource the verification of pairing equations such as BLS signatures. A prover can give a short proof that n BLS signatures are correct and the verifier can check this proof using 2n group exponentiations but only <b>one</b> expensive pairing. This protocol can be used in a blockchain where a block contains many signatures and fast verification of the block is vital. 
Finally, we use a variant of the inner pairing product to aggregate n pairing based SNARKs such as <a href="https://eprint.iacr.org/2016/260.pdf">Groth 16</a> into a logarithmic sized proof. Verifiying this batched proof only takes O(log(n)) time. Aggregating SNARKs could only previously be achieved through expensive recursive proof techniques and NP reductions. The Inner Pairing Product on the other hand is fully algebraic and does not rely on expensive NP reductions.
</dd>

</dl>
</div>
</div>
</div>

  <div class="card">
<div class="card-header" role="tab" id="nestaHeading">
<h5 class="mb-0">
  <a  class="collapsed" data-toggle="collapse" href="#nesta" aria-expanded="false" aria-controls="collapseOne">
  Proof-Carrying Data from Accumulation Schemes
  </a>
</h5>
</div>
<div id="nesta" class="collapse" role="tabpanel" aria-labelledby="nestaHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
B. Bünz, [A. Chiesa](https://people.eecs.berkeley.edu/~alexch), [P. Mishra](https://people.eecs.berkeley.edu/~pratyushmishra) and [N. Spooner](https://people.eecs.berkeley.edu/~spooner/)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2020/499) (Published at TCC 2020)
</dt>
<dt markdown="1">
[Talk by Nick at BU](https://www.youtube.com/watch?v=UNwlBq1FQ3E)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/nesta.pptx)
</dt>
<dt>TLDR</dt>
<dd>
We present a new cryptographic tool called an accumulation scheme for proof systems (unrelated to set accumulators). An accumulation scheme for a predicate (such as proof verification) enables the accumulation of multiple invocations of the predicate and old accumulators into a new accumulator. Checking that the accumulation was done correctly is ideally much cheaper than deciding the predicate itself. In the end a decider can determine whether the final accumulator is valid
and if so this implies that all accumulated predicate checks were valid. Together this enables delaying and combining expensive checks.
This is particularly useful as we show that accumualtion schemes can be used to build very efficient recursive proofs. This approach was proposed by Bowe, Grigg and Hopwood in recent work called [Halo](eprint.iacr.org/2019/1021). We formalize and prove correctness of this approach. We also show that a variant of the accumulation scheme from Halo and an accumulation scheme based on bilinear maps satisfy our definitions and are secure. The resulting recursive proof constructions have
significant new efficiency and security features.
</dd>

</dl>
</div>
</div>
</div>

  <div class="card">
<div class="card-header" role="tab" id="darksHeading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#darks" aria-expanded="false" aria-controls="collapseOne">
  Transparent SNARKs from DARK Compilers
  </a>
</h5>
</div>
<div id="darks" class="collapse" role="tabpanel" aria-labelledby="darksHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
B. Bünz, [B. Fisch](https://sites.google.com/site/benafisch/) and [A. Szepieniec](https://asz.ink)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2019/1229) (Published at Eurocrypt 2020)
</dt>
<dt markdown="1">
[Talk at Simons Institute](https://www.youtube.com/watch?v=m3Cc0kuzhfg)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/darks.pptx)
</dt>
<dt>TLDR</dt>
<dd>
We present a new polynomial commitment scheme from groups of unknown order with logarithmic proof size and logarithmic verifier time. Plugged into proof systems like Sonic, Plonk or Marlin this leads to SuperSonic a SNARK with 10KB proofs and <b>without</b> trusted setup! This is the shortest practical SNARK without trusted setup today. We also provide an abstraction for proof systems like Sonic et al. called polynomial IOPs. We show that using a polynomial commitment scheme (such as DARKs) they can be compiled to SNARKs. Moreover all of the cryptographic assumptions and trusted setup assumptions (or lack thereof) are in the polynomial commitment scheme.
</dd>

</dl>
</div>
</div>
</div>

  <div class="card">
<div class="card-header" role="tab" id="flyclientHeading">
<h5 class="mb-0">
  <a  class="collapsed" data-toggle="collapse" href="#flyclient" aria-expanded="false" aria-controls="collapseOne">
 Flyclient: Super-Light Clients for Cryptocurrencies
  </a>
</h5>
</div>
<div id="flyclient" class="collapse" role="tabpanel" aria-labelledby="flyclientHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors</dt>
<dd markdown="1">
B. Bünz, [L. Kiffer](https://www.khoury.northeastern.edu/people/lucianna-kiffer/) , [L. Luu](https://loiluu.com/) and [M. Zamani](http://mahdiz.com/)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2019/226) (Published at IEEE S&P (Oakland) 2020)
</dt>
<dt markdown="1">
[Talk at Zcon](https://www.youtube.com/watch?v=vuzYwutBqjY)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/flyclient.pptx)
</dt>
<dt>TLDR</dt>
<dd>
We present Flyclient which is a protocol that lets a super-light client determine which is the correct (longest) proof of work chain. The client only needs to download a logarithmic number of block headers (say 200 instead of 1 million). The protocol is a non-interactive proof of proof of work (NiPoPoW) that shows that a chain has at least x amount of work put into it. It uses a random sampling of block headers to ensure that an adversary with limited mining power could not have produced this chain.
</dd>

</dl>
</div>
</div>
</div>

 <div class="card">
<div class="card-header" role="tab" id="accumulatorsHeading">
<h5 class="mb-0">
  <a class="collapsed" data-toggle="collapse" href="#accumulators" aria-expanded="false" aria-controls="collapseOne">
  Batching Techniques for Accumulators with Applications to IOPs and Stateless Blockchains
  </a>
</h5>
</div>
<div id="accumulators" class="collapse" role="tabpanel" aria-labelledby="accumulatorsHeading" data-parent="#cryptoacordion">
      <div class="card-body">
<dl>
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
[D. Boneh](https://crypto.stanford.edu/~dabo),  B. Bünz and [B. Fisch](https://sites.google.com/site/benafisch/)
</dd>
<dt markdown="1">
[Paper](https://eprint.iacr.org/2018/1188) (Published at Crypto 2019)
</dt>
<dt markdown="1">
[Talk at Scaling Bitcoin 18](https://youtu.be/IMzLa9B1_3E?t=3515)
</dt>
<dt markdown="1">
[Slides]({{ site.url }}/presentations/accumulators.pptx)
[Technical Slides]({{ site.url }}/presentations/accumulatorcryptoday.pptx)
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
[Paper]({{ site.url }}/papers/zether.pdf) (Published at FC 2020)
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
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
[D. Boneh](https://crypto.stanford.edu/~dabo),  B. Bünz and [B. Fisch](https://sites.google.com/site/benafisch/)
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
<dt>Authors (alphabetical)</dt>
<dd markdown="1">
[D. Boneh](https://crypto.stanford.edu/~dabo), [J.Bonneau](http://www.jbonneau.com/), B. Bünz and [B. Fisch](https://sites.google.com/site/benafisch/)
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
  <a class="collapsed" data-toggle="collapse" href="#bulletproofs" id="bpbutton"  aria-expanded="false" aria-controls="collapseOne">
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
  <a class="collapsed" data-toggle="collapse" href="#provisions" aria-expanded="false" aria-controls="collapseOne">
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

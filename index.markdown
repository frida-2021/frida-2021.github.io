---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# The 8th Workshop on Formal Reasoning in Distributed Algorithms

Dates: October 4th and October 8th 2021

Online workshop from 4pm to 8pm CEST (time in Freiburg, Germany).

The workshop is organized as part of [DISC 2021](http://www.disc-conference.org/wp/disc2021/).

## News

* September 7th: website created!
* September 21st: [Registration to DISC](http://www.disc-conference.org/wp/disc2021/registration/) is open and free for online participants

## Program (tentative)

* Monday, October 4th
  * 4pm to 5pm: Keynote by [Julian Loss](https://www.julianloss.com/)
    <details>
    <summary>Formal Security Guarantees for Distributed Consensus Algorithms (click to expand the abstract)</summary>
      <br>
      <p>
      Distributed Consensus is the fundamental problem of agreeing on a common output in a network of pairwise connected parties. It can be studied under various network and setup assumptions that determine the parameters for which a solution exists. Proving security and correctness of consensus algorithms is known to be a subtle and error-prone task. In this talk, we will focus on recent advances in the area of distributed consensus and explain some of the key challenges that arise. We also discuss how tools from formal verification could be helpful to address them.
      </p>
    </details>
  * 5pm to 5:40pm: [Joseph Tassarotti](http://www.cs.bc.edu/~tassarot/)
    <details>
    <summary>Modular Verification of Distributed Systems with Grove (click to expand the abstract)</summary>
      <br>
      <p>
      Grove is a Concurrent Separation Logic (CSL) framework for distributed systems, with a focus on modular verification of servers and client-side libraries. To enable this, Grove uses the CSL idea of ownership of resources. We introduce a duplicable ownership specification for unreliable remote procedure calls and an escrow pattern for proving ownership transfer over unreliable networks. Using Grove we developed and verified an example system written in Go consisting of an RPC library, a sharded key-value store with support for dynamically adding new servers and rebalancing shards, a lock service, and a bank application that supports atomic transfers across accounts that live in different shards. The proofs are mechanized in the Coq proof assistant using the Iris library and Goose tool for verifying Go.
      </p>
    </details>
  * 5:40pm to 5:50pm: break
  * 5:50pm to 6:30pm: [Christopher Goes](https://pluranimity.org/about/)
  * 6:30pm to 7:10pm: [Bernhard Kragl](https://bkragl.github.io/)
  * 7:10pm to 8:00pm: discussion, maybe in breakout rooms
* Friday, October 8th
  * 4pm to 5pm: Keynote by [Andreas Podelski](https://swt.informatik.uni-freiburg.de/staff/podelski)
    <details>
    <summary>Proof Spaces and Operational Correctness Arguments <br> (joint work with Azadeh Farzan and Zachary Kincaid)</summary>
    </details>
  * 5pm to 5:40pm: [Sreeja S Nair](https://sreeja.github.io/), LIP6, Sorbonne Université, and Inria, Paris, France
    <details>
    <summary>Exploring the coordination lattice  (click to expand the abstract)</summary>
      <br>
      <p>
      Distributed applications support concurrent operations on their replicas to ensure high availability and low latency. Too much concurrency might violate an application invariant. Verification can say if a distributed application with the given coordination is safe. The required coordination can be implemented in many ways, trading overhead against parallelism. This talk will focus on capturing different dimensions of the subclass of coordination, distributed locks, into a Coordination Lattice. In particular, for a given workload, we look into the impact of a coordination configuration, with granularity, mode, and placement dimensions, on the performance of a distributed application.
      </p>
    </details>
  * 5:40pm to 5:50pm: break
  * 5:50pm to 6:30pm: [Karem Sakallah](https://web.eecs.umich.edu/~karem/)
    <details>
    <summary>Regularity, Quantification, and Hierarchical Strengthening: A New Approach to Verify Distributed Protocols (click to expand the abstract)</summary>
      <br>
      <p>
      Finite-state model checking has made significant advances in the last few years. For example, our AVR hardware model checker for safety properties successfully handled an industrial design containing over 60,000 state bits and was the overall winner in last year's hardware model checking competition. Three main ingredients made this possible: a) highly-scalable SAT and SMT solvers, b) approximate reachability algorithms based on IC3-style incremental induction, and c) equality abstraction of data.
      </p>
      <p>
      Inspired by our work on hardware model checking with AVR, we developed IC3PO, a new verifier that automatically produces quantified inductive invariants proving the correctness of unbounded distributed protocols. IC3PO takes advantage of the spatial and temporal regularity of unbounded protocols to reduce the unbounded verification problem to a sequence of small finite protocol instances (up tp a cutoff size) that incrementally reveal the quantified strengthening assertions needed to establish inductiveness and prove safety.
      </p>
      <p>
      The talk will sketch the IC3 finite incremental induction algorithm and show how it is modified in IC3PO to automatically infer and generalize the quantifier prefixes in the finite strengthening assertions by taking  advantage of spatial and temporal regularity. 
      </p>
      <p>
      IC3PO also takes advantage of the hierarchical specification of complex protocols, such as Lamport's Paxos, using a top-down stepwise invariant strengthening procedure. Using a four-level hierarchy, the talk will conclude by describing how IC3PO automatically produced the same inductive invariant for Paxos as its manually-written proof.
      </p>
      <p>
      There is still much to explore in extending automatic verification to the domain of unbounded protocols. We believe this is a promising first step.
      </p>
    </details>
  * 6:30pm to 7:10pm: [Roopsha Samanta](https://www.cs.purdue.edu/homes/roopsha/), Purdue University
    <details>
    <summary>Taming Unbounded Distributed Systems with Modular, Bounded Verification (click to expand the abstract)</summary>
      <br>
      <p>
      Modern distributed services are typically built in a modular fashion using core distributed protocols as building blocks. The ubiquity of some of these building blocks has sparked several valiant verification efforts for them in the last decade. Oddly, there have been far fewer verification efforts that go beyond core protocols and target distributed services built on top of such core protocols.  In our Discover[i] project, we seek to develop modular, scalable, fully-automated verification approaches for distributed systems that mimic their modular design. In particular, we advocate an approach based on assuming that the underlying core protocols are verified separately and encapsulating their complexities within cleanly-defined abstractions.
      </p>
      <p>
      In this talk, I will present QuickSilver, a modeling and verification framework for distributed systems built on top of verified distributed agreement protocols such as consensus. I will show how our encoding of agreement protocols facilitates decidable and scalable verification for a broad class of systems including a datastore, a lock service, a surveillance system, and several other interesting case studies adapted from real-world applications.
      </p>
    </details>
  * 7:10pm to 8:00pm: discussion, maybe in breakout rooms


## Summary of the workshop

Distributed algorithms is an active research field; their applications range
from Internet applications over cloud computing to safety-critical control
systems. Whereas many applications are of critical importance, the correctness
of distributed algorithms is usually based on very subtle mathematical
arguments. Consequently, one easily can make mistakes with hand-written proofs,
which reduces the trust in the correctness of these systems.

In the last decades, formal methods were proven to be useful for the
verification of many hardware and software systems. For distributed algorithms,
the application of formal methods was limited: formal methods have been used
for finding bugs in distributed algorithms, and to a much smaller extent formal
methods were used in computer-aided verification of simple distributed
algorithms. However, to verify more involved distributed algorithms, one cannot
easily apply existing verification tools. To be eventually able to do this, an
interdisciplinary effort from the concerned fields of formal methods, logic in
computer science, and distributed algorithm theory is required.

The topics of interest for the FRIDA workshop include the following topics, as
they apply to distributed algorithms and systems:

* formal modeling
* model checking
* interactive theorem proving
* parameterized model checking
* integration of different verification techniques
* benchmarking
* synthesis
* run-time verification
* testing
* invariant inference


## Organizers

* Swen Jacobs
* Igor Konnov
* Joseph Widder
* Stephan Merz
* [Marijana Lazić](https://www7.in.tum.de/~lazic/) [(email)](mailto:lazic@in.tum.de)
* [Giuliano Losa](https://www.losa.fr/) [(email)](mailto:giuliano@galois.com)

## Previous editions

Starting a productive dialogue between distributed algorithms and verification
communities was the goal of a successful [Dagstuhl Seminar “Formal Verification
of Distributed Algorithms”](https://www.dagstuhl.de/en/program/calendar/semhp/?semnr=13141)
which was held in April 2013. During this seminar,
the participants agreed that a series of workshops should be held in order to
strengthen the community that does research on these issues.

The [1st workshop on Formal Reasoning in Distributed
Algorithms](https://easychair.org/smart-program/VSL2014/FRIDA-index.html) took
place in Vienna as part of the Vienna Summer of Logic’14 and Federated Logic
Conference’14. The [2nd FRIDA
workshop](http://discotec2015.inria.fr/workshops/frida-2015/) took place in
Grenoble as part of FORTE’15. The [3rd FRIDA
workshop](https://forsyte.at/events/frida2016/) was organized in Marrakech as
part of NETYS’16. The [4th FRIDA
workshop](https://forsyte.at/events/frida2017/) took place in Vienna as part of
DISC 2017. The [5th FRIDA workshop](https://forsyte.at/events/frida2018/) was
co-located with CAV 2018, which was held as part of the Federated Logic
Conference (FLoC). The [6th
workshop](https://team.inria.fr/veridis/events/frida2019/) was co-located with
DISC 2019 in Budapest, Hungary. Finally, last year, [FRIDA
2020](https://frida2020.galois.com/) took place as an online workshop at
QONFEST 2020.

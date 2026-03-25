---
layout: page
title: Program
---

## Workshop

Schedule: TBA

## Talks

#### Matt Cuffaro: *More flexible interfaces for specifying simulations of systems in [CatColab](https://catcolab.org)*

CatColab distinguishes between a theory, its model, instances of such
models, and analyses, which are “things which you can do on a model or
its instance.” One effect of this design is that it separates two
modeling concerns–model specification and model simulation–and avoids
hard-coding assumptions in the model for how it should be
simulated. Instead, models are treated as data which are compiled to
valid simulation objects in the target domain, and the user is only
expected to set the initial conditions and geometry for the simulation
through simple dropdown interfaces specified by the developer. However
more complicated analyses such as multiphysics simulations are
difficult to specify using “no-code” interfaces, e.g., having more
complicated initial/boundary conditions that require bespoke code
provided by a user with advanced programming experience. This
presentation will demonstrate progress in CatColab towards more
granular, flexible interfaces for specifying analyses, specifically
for multiphysics simulations.

#### Bruno Gavranović: *[TensorType](https://github.com/bgavran/TensorType): Implementing and extending Deep Learning with Types*

Category theory has seen a rise in applications in deep learning,
bringing with it ideas and tools from functional programming and
dependent type theory. However, practical implementations of these
ideas face significant friction. Successful neural network frameworks
only exist in dynamically typed languages such as Python, and attempts
to implement these ideas in statically-typed languages have struggled
with expressiveness and ergonomics, typically only replicating what
exists without imagining what can be.

In this talk, I will introduce TensorType, a tensor processing
framework implemented in Idris 2 aiming to demonstrate that ergonomics
and rigor need not be at odds. TensorType provides tensor operations
checked at compile-time while enabling fundamentally new capabilities:
tensors that branch and recurse instead of being confined to
rectangular shapes. I will walk through the design choices behind
TensorType, showcase how containers power its core abstractions, and
explore strange new worlds it enables.

#### Tom Kuhmichel: *Equivariant Orlik-Solomon Algebras*

Let $k$ be a commutative ring.  For every finite geometric lattice $L$
one can construct the Orlik-Solomon algebra $OS_k(L)$.  It is a
quotient of the exterior algebra $E_k(L)$ build from the atoms of $L$
and in particular an acyclic differential $\mathbb{Z}$-graded
$k$-algebra.  For computing the algebra structure, simple numerical
calculations show, that the structure morphisms $OS_k^1(L) \otimes
OS_k^p(L) \rightarrow OS_k^{p+1}(L)$ quickly explode.  Since each
graded part $OS_k^p(L)$ is direct sum of induced representations of
subgroups of the automorphism group $\mathrm{Aut}(L)$, one strategy to
slow down this explosion is to exploit the equivariance of $OS_k(L)$
under subgroups of $\mathrm{Aut}(L)$.  This can be realised by
considering $OS_k(L)$ as an object in the category of
$E_k(L)$-$Mod({sRep_k(G)}_\bullet)$ of $E_k(L)$-modules internal to
the finitely graded closure of the skeleton of the category of finite
dimensional $k$-linear representations of $G$ (where $k$ is now chosen
such that $sRep(G)$ is semisimple).  The category ${sRep_k(G)}$ serves
thus as a foundation for all our computations, the most challenging
part of it being its tensor structure, which goes far beyond the
character table of $G$.  We will demonstrate the current state of an
implementation of these ideas inside the [CAP](https://homalg-project.github.io/docs/CAP_project-based/) project.

#### Alexanna (Xanna) Little: *Categorical Message Passing Language ([CaMPL](https://campl-ucalgary.github.io)) and its Semantics*

Categorical Message Passing Language (CaMPL) is a functional-style
concurrent programming language whose semantics is in category
theory. Its core programming feature is message passing along typed
communication channels between concurrent processes. CaMPL also
supports controlled non-determinism via 'races' which allow processes
to adapt dynamically while they are running, higher-order processes
which pass other processes as messages, and custom channel datatypes
called protocols and coprotocols which allow one to define infinite
channel types or implement session types.  Similar to the
Curry-Howard-Lambek correspondence in sequential programming, the
existence of a three-way correspondence between message passing,
linear actegories, and poly-actegories has been established. The
semantics of core CaMPL is defined using this correspondence. The type
system given by the semantics ensures that a formal CaMPL program,
i.e. one which does not allow general recursion, will never become
deadlocked or livelocked.  We will briefly explore the categorical
semantics of CaMPL, and the focus of this presentation will be on code
demonstrations to showcase the above features.

#### Yoshihiro Maruyama and Ryo Nasu: *Category-Equivariant Neural Networks: Equivariant Learning beyond Group Symmetries*

Category-equivariant neural networks (CENNs) generalize classical
equivariant architectures from group symmetries to categorical
symmetries. CENNs provide a unified framework for equivariant learning
on structured domains, encompassing graph neural networks and
group-equivariant neural networks as special instances. Under suitable
conditions, we can prove category-equivariant universal approxima-
tion theorems, which show that CENNs are dense in spaces of continuous
category-equivariant transformations, extending the mathematical
foundations of symmetry-aware learning beyond group equivariance. We
present proof-of-concept experiments to demonstrate the advantage of
CENNs over existing neural architectures.

#### Nelson Martins-Ferreira: *Categorical Structures in MATLAB and Octave Programming*

In this talk, we investigate how categorical concepts can be
identified and implemented within the programming environments of
MATLAB and Octave, where complex-valued matrices serve as fundamental
data structures. We examine how common programming operations can be
interpreted through a categorical perspective, highlighting how
index-based manipulation of arrays corresponds naturally to function
composition and morphisms between finite sets.  We analyze the
categorical behavior of several built-in functions, including unique,
ismember, sortrows, and sparse, showing how they implicitly encode
constructions related to images, factorization, and relational
structures. Building on this perspective, we present a method for
representing directed graphs as pairs of complex-valued matrices and
describe a procedure that reorganizes these representations into
indexed forms where the domain component admits a surjective index.
Finally, we introduce the implementation of a programming function
that models a categorical construction analogous to a coequalizer,
illustrating how abstract categorical ideas can guide the design of
computational procedures in MATLAB and Octave. The approach is
inspired by recent developments in internal categorical structures and
their applications as described in [1,2,3].

References

[1] N. Martins-Ferreira, Internal Categorical Structures and Their Applications, Mathematics (2023) 11(3), 660. [https://doi.org/10.3390/math11030660](https://doi.org/10.3390/math11030660)

[2] N. Martins-Ferreira, On the Structure of an Internal Groupoid, Applied Categorical Structures (2023) 31:39. [https://doi.org/10.1007/s10485-023-09](https://doi.org/10.1007/s10485-023-09).

[3] N. Martins-Ferreira, From Matrices to Morphisms: Categorical Programming in MATLAB and Octave, Scripta-Ingenia, Issue14, December 2025, pp9--17.

#### Evan Patterson: *[CatColab](https://catcolab.org): Formal collaborative modeling based on category theory*

CatColab is a collaborative environment for building formal models in
various domains of science and engineering. It is designed following
category-theoretic principles, though it is intended to be usable
without any specialized mathematical knowledge. Category theory
appears in CatColab in three guises. First, CatColab aims to adapt
itself to the conceptual structure of different domains through
domain-specific categorical logics. Such logics are uniformly
specified via a meta-logic based on double categories. Second,
CatColab supports modular and hierarchical composition of models,
using techniques from applied category theory. Finally, many models in
CatColab are themselves categorical structures; for example, causal
loop diagrams are viewed as free signed categories and Petri nets as
free symmetric monoidal categories. Such models admit richer notions
of motif finding and model refinement than they would if described
purely combinatorially. In this talk, we give a brief demonstration of
CatColab, describe the system's mathematical and software
architecture, and survey current capabilities as well as future
directions.

#### Kamal Saleh: *Transpiling [CAP](https://homalg-project.github.io/docs/CAP_project-based/) from GAP to Julia: Bridging Two Worlds of Computational Algebra*

CAP (Categories, Algorithms, Programming) is a framework for
constructive category theory implemented in the computer algebra
system GAP. In my PhD thesis, I developed several CAP-based packages
for constructive homological algebra. These packages provide
algorithmic implementations of homotopy categories, derived
categories, and triangulated tilting equivalences, and now form the
core of the HigherHomologicalAlgebra project.

Because of the remarkable syntactic similarity between GAP and the
Julia programming language, Julia suggests itself as a natural target
for an automatic transpilation of CAP and its ecosystem of
packages. Despite their syntactic resemblance, the two systems differ
in their object models, type systems, and method dispatch
mechanisms. The central challenge therefore lies in preserving the
mathematical meaning and behavior of the code when moving between the
two languages. Our approach proceeds along two complementary
lines. First, we reduce reliance on GAP-specific features that have no
direct analogue in Julia. Second, we explore targeted extensions in
Julia that support the structural features of GAP on which CAP
depends. This talk presents the ongoing transpilation effort,
discussing obstacles involved and potential gains of embedding the
project into the Julia ecosystem.

#### Marc Talleux: *Implementing bisets for groups in [CAP](https://homalg-project.github.io/docs/CAP_project-based/)*

I will present an implementation of the biset category of groups in
CAP.  After introducing the basic definitions of bisets and their
composition, I will explain why and how a (G,H)-biset can be encoded
as a functor from the group G (considered as a category) to PSh(H),
the presheaf category on H, which is equivalent to the category of
H-sets. This approach allows us to describe biset composition in an
elegant and algorithmic way. As a consequence, a first model of the
biset category can be implemented almost immediately using the current
capabilities of CAP-based packages. However, the specific context of
groups also allows us to define a more efficient model for
PSh(G). Indeed, thanks to orbit decompositions, PSh(G) can be
described as the finite coproduct completion of transitive G-sets. I
will therefore present our implementation of finite G-sets as a
"categorical tower" and the underlying ideas. This example highlights
some of the key strengths of CAP, including categorical towers,
categorical remodeling, and flexible implementation. This is joint
work with Mohamed Barakat.

#### Ryan Wisnesky and Daniel Filonik: *Relational to RDF Data Migration by Query Co-Evaluation*

In this talk we define a new algorithm to convert an input relational
database to an output set of RDF triples. The algorithm can be used to
e.g. load CSV data into a financial OWL ontology such as FIBO. The
algorithm takes as input a set of relational conjunctive
(select-from-where) queries, one for each input table, from the three
column (subject, predicate, object) output RDF schema to the input
table's relational schema. The algorithm's output is the only set of
RDF triples for which a unique round-trip of the input data under the
relational queries exists. The output may contain blank nodes, is
unique up to unique isomorphism, and can be obtained using elementary
formal methods (equational theorem proving and term model construction
specifically). We also describe how (generalized) homomorphisms
between graphs can be used to write such relational conjunctive
(select-from-where) queries, which, due to the lack of structure in
the three-column RDF schema, tend to be large in practice. We
demonstrate examples of both the algorithm and mapping language on the
FIBO financial ontology.  This work is an instance of real-world
functorial data migration, specialized to the context of RDF loading,
allowing for simplified algorithmics to be described in enough detail
for replication in other applied category theory systems.

[https://arxiv.org/abs/2403.01630](https://arxiv.org/abs/2403.01630)


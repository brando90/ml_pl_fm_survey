Proposal for Survey in Selection and Synthesis of formulas and programs
----

Goals
----

The goal of this will be to summarize the main contributions of methods that contribute to symboling reasoning, formula/program synthesis and learning in all of these domains. The main two tasks to solve and have a summarize of state of the art is

1) Methods for selection of key concepts from a library of concepts/symbols
2) Methods for synthesis of programs/formulas/discrete structures
3) Optimization methods for discrete/symbolic optimization

Compression of ideas from papers
----

When reading each paper it will be important to identify

1) the problem they are solving (i.e. 1), 2) 3))
2) the main ideas of the methods
3) advantages and limitation of the methods
4) ways it connect to our current projects (Coq proof synthesis and Loop Invariant Learning)

Section: Papers for 1) Methods for selection of key concepts from a library of concepts/symbols
----

premise selection
- [ ] DeepMath - Deep Sequence Models for Premise Selection (https://arxiv.org/abs/1606.04442) 
- [ ] Premise Selection for Theorem Proving by Deep Graph Embedding (https://arxiv.org/abs/1709.09994)
- [ ] ATPboost: Learning Premise Selection in Binary Setting with ATP Feedback (https://arxiv.org/abs/1802.03375)
- [ ] Premise selection with neural networks and distributed representation of features (https://arxiv.org/abs/1807.10268)

memory networks
- [ ] Memory Networks gi(https://arxiv.org/abs/1410.3916)
- [ ] A Taxonomy for Neural Memory (https://arxiv.org/pdf/1805.00327.pdf
)
- [ ] Machine Learning for Instance Selection (http://matryoshka.gforge.inria.fr/pubs/ml_instance_abstract.pdf, https://www.google.com/search?q=machine+learning+for+instance+selection+in+SMT+solving&rlz=1C5CHFA_enUS741US741&oq=machine+learning+for+instance+selection+in+SMT+solving&aqs=chrome..69i57.8798j0j4&sourceid=chrome&ie=UTF-8)

Differentiable Computers
- [ ] Nural Turing Machines (NTM),  (https://arxiv.org/pdf/1410.5401.pdf)
- [ ] NTM RL, Reinforcement Learning Neural Turing Machines - Revised (https://arxiv.org/abs/1505.00521)
- [ ] Implementing Neural Turing Machines (https://arxiv.org/abs/1807.08518)
- [ ] Differentiable Neural Computers =  RNN + external memory, Adaptive Computation Time
for Recurrent Neural Networks(https://arxiv.org/pdf/1603.08983.pdf)

Embeddings of symbols
- [ ] BERT (https://towardsdatascience.com/bert-explained-state-of-the-art-language-model-for-nlp-f8b21a9b6270)
- [ ] BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding (https://arxiv.org/abs/1810.04805)
- [ ] ELMO (https://allennlp.org/elmo)
- [ ] Deep contextualized word representations (https://arxiv.org/abs/1802.05365
)

Section: Papers for 2) Methods for synthesis of programs/formulas/discrete structures
----

- [ ] Learning Loop Invariants for Program Verification (https://papers.nips.cc/paper/8001-learning-loop-invariants-for-program-verification.pdf, https://www.youtube.com/watch?v=Q1eAO2pZPZ8, https://www.facebook.com/nipsfoundation/videos/session-2-room-220-e/2106994059390210/)

- [ ] Execution-Guided Neural Program Synthesis (https://openreview.net/pdf?id=H1gfOiAqYm)
- [ ] Sorcar: Property-Driven Algorithms for Learning Small Conjunctive Invariants (talk to me for pdf)
- [ ] Learning Invariants Using Decision Trees and Implication Counterexamples (https://dl.acm.org/citation.cfm?doid=2837614.2837664)
- [ ] Abstract Learning Frameworks for Synthesis (https://link.springer.com/content/pdf/10.1007%2F978-3-662-49674-9_10.pdf)
- [ ] ICE: A Robust Framework for Learning Invariants (https://link.springer.com/content/pdf/10.1007%2F978-3-319-08867-9_5.pdf)
- [ ] Learning to infer program sketches (https://arxiv.org/pdf/1902.06349.pdf)

Syntax & Semantics stuff from LIP

- [ ] Syntax-Directed Variational Autoencoder for Structured Data (https://arxiv.org/abs/1802.08786)
- [ ]  Neuro-Symbolic Program Synthesis (https://arxiv.org/pdf/1611.01855.pdf)
- [ ] Grammar Variational Autoencoder (https://arxiv.org/pdf/1703.01925.pdf)

Section: Papers for 3) Optimization methods for discrete/symbolic optimization
----

TODO: papers on RL/DL composing Neural Networks

Comibinatorial Optimization
- [ ] Automatic Local Rewriting for Combinatorial Optimization (https://arxiv.org/abs/1810.00337)
- [ ] Neural combinatorial optimization with reinforcement learning (https://arxiv.org/pdf/1611.09940.pdf)
- [ ] Learning Combinatorial Optimization Algorithms over Graphs (https://arxiv.org/pdf/1704.01665.pdf
)

Neural Module Networks:

- [ ] Neural Module Networks (https://arxiv.org/abs/1511.02799)
- [ ] Textually Enriched Neural Module Networks for Visual Question Answering (https://arxiv.org/abs/1809.08697)
- [ ] Learning to Compose Neural Networks for Question Answering (https://arxiv.org/abs/1601.01705)
- [ ] Modeling Relationships in Referential Expressions with Compositional Modular Networks (https://arxiv.org/abs/1611.09978)
- [ ] Learning to Reason with Neural Module Networks (https://bair.berkeley.edu/blog/2017/06/20/learning-to-reason-with-neural-module-networks/)
- [ ] Learning to Reason: End-to-End Module Networks
for Visual Question Answering (https://arxiv.org/pdf/1704.05526.pdf)
- [ ]  Jacob Andreas (https://people.eecs.berkeley.edu/~jda/)

Formal Methods techniques (ATPs, theorem proving)

- [ ] E prover, Stephan Schulz. E - A Brainiac Theorem Prover. AI Commun., 15(2-3):111–126, 2002. ()
- [ ] Clause Features for Theorem Prover Guidance (http://aitp-conference.org/2019/abstract/AITP_2019_paper_19.pdf)
- [ ] Coq Hammer (https://github.com/lukaszcz/coqhammer)
- [ ] Vampire: https://vprover.github.io.
- [ ] CVC4: http://cvc4.cs.stanford.edu. CVC4 needs to be version 1.6 or later. Earlier versions do not fully support the TPTP format. It is recommended to have the better-performing GPL version of CVC4 instead of the BSD version.
- [ ] Eprover: http://www.eprover.org.
- [ ] Z3: https://github.com/Z3Prover/z3/releases. Note that the default version of Z3 does not support the TPTP format. You need to compile a TPTP frontend located in examples/tptp in the Z3 source package

Discussion
----

Note this list is not complete so feel free to update or add papers that have been missed. Other potential good source for expanding this list could be 

- found in the AITP conference: http://aitp-conference.org/
- https://people.mpi-sws.org/~neider/

Note that papers above link to more papers. It will be useful to also read those and plan how to include them in the survey.

TODOs
----

- put hammers on sections/lists
- put (Coq) Hammers on sections/lists

Other useful ideas for projects
----

Section 4) Non-stationary/evolving RL policies
----
Since the RL mathematician will learn new concepts that it didn't know, it's policy must have a mechanism for choosing new actions that were not considered before. For this reason the policy's action space might be changing

TODO ask Nan and Dimitrios, how to expand action choices such that the actions are not fixed

- [ ] AlphaStar (https://deepmind.com/blog/alphastar-mastering-real-time-strategy-game-starcraft-ii/)
- [ ] Deep Reinforcement Learning in Large Discrete Action Spaces (https://arxiv.org/pdf/1512.07679.pdf)


Section 5) Curriculum learning
----
Mathematics is compositional. Using this idea the agent as it learns more it should be able to have more power and solve more problems. How can we use the curriculum learning paradigm to explore this complicated learning landscape better?

TODO

Section 6) Sparse-rewards
----
How can we have the agent learn better when the only reward is the final reward of the proof being right or wrong? Perhaps the fact it trains/learns on proofs separated by humans will be enough?

TODO

Section 7) pre-training RL agents
----
We probably should not start with AlphaZero sort of agent right away.

TODO, this might just be for the short term. One idea is to use human proofs and the states map to human actions as supervised data.

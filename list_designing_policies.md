Intro
----
The goal is to create a list of technique and paradigms for desiging policies in RL.

Techniques List
----

- Classifier type softmax output over actions
- Auto-regressive model for a squence of parts of the action
  - p_theta(a|s) = \prod pi_theta(a^l | a^{<l}, s)
- embed actions in continuous space
- actions specified by a grammar (RL loop invariant paper)
- the compression kkn approximation approach for really large policy spaces


Evolving policies ideas
----

- clasifier like network.
  - have the final layer be each action
  - when a new action is incorporated, add a new vector to the end of the final layer [ W , w_new ]
  - one can encourage the network to not change too much via some regularization
  - also we can think of the initial training and earlier layers as layers for feature extraction. The final layer might not even matter too much. <- hypothesis!

Intro
----
The goal is to create a list of technique and paradigms for desiging policies in RL.

Techniques List
----

- Classifier type softmax output over actions
- Auto-regressive model for a squence of parts of the action
  - p_theta(a|s) = \prod pi_theta(a^l | a^{<l}, s)
- embed actions in continuous space

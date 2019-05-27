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
- eucledian distance then compute the distance to the closest image and output that label
  - facenet way to do it (https://stats.stackexchange.com/questions/241172/how-does-facenet-googles-facerecognition-handles-a-new-image)
 
- attention uses a weight alpha^{<t,t'>} for each word (or its embedding) it attends a^{<t>} and for each output word y^{<t'>} it ouputs/translated. Since the things it processes are variable length its important that the weights don't scale according to the input length. To avoid that what it does is it has an input network that computes the weights according to a softmax but the input weight is only depedend on previous vectors rather than on the sequence. i.e. alpha^{<t,t'>} = Exp( e^{<t,t'>} ) / Z where e^{<t,t'>} = NN(s^{t},a^{<t'>}). Note that this means the alphas apply around all the changing size input because NN is fixed.
  - this same idea could be used to weight each thm in the thm library. Attend each thm basically (or attend each summary thm)
  - the only thing is how to the select the thm

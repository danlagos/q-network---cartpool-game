# q-network---cartpool-game

This is my first Q learning algorithm!  

It is unstable, it is not the fastest, and produces bad results.  However, without addressing the reasons for the instability, this algorithm will never produce favorable results.

Also, I placed a constraint upon myself, that is I refused to look at or use frameworks other than numpy, matplotlib, or pytorch.  I am sure something like HuggingFace has an API that you can use one line of code to run this entire algorithm!  I am exaggerating, of course, but the point of this algorithm is to understand the mechanics of a reinforcement learning algorithm.  Using an API that solves the problem for me would not accomplish this.  

This Q learning algorithm focuses on the cartpool game.

You will require python 3.6 to run the algorithm.

Unstable for the following reasons:

  *	This occurs because I am using one network for actions and values.
  *	Correlations are present in sequence of observations.
  *	Small updates to Q may significantly change the policy.
  *	Correlations between the action-values and target values.
    *	Using a single network to take an action and also to tell us the value of the actions.

Solutions – this will appear in my next Q learning algorithm.

  *	Create a class to handle the experience replay.
  *	A separate deep neural network to handle the calculation of the target values.

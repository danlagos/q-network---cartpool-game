# q-network---cartpool-game

This is my first Q learning algorithm!  

This Q learning algorithm focuses on the cartpool game.  Psuedo code is found in the top of file deep_q_learning.py.

You will require python 3.6 to run the algorithm.

The model is unstable, it is not the fastest, and produces bad results.  Without addressing the reasons for the instability, this algorithm will never produce favorable results.  This algorithm is only meant to learn my way around RL with Q learning.  I am not focusing on solving the problems, yet.

Also, I placed a constraint upon myself, that is I refused to look at or use frameworks other than numpy, matplotlib, or pytorch.  I am sure something like HuggingFace has an API that allows you to solvethe problem with one line of code!  I am exaggerating, of course, but the point of this algorithm is to understand the mechanics of a reinforcement learning with Q learning, and to understand what issues arise from this approach to RL.  Using an API that solves the problem for me would not accomplish this.  

To better understand the issues that arise I want to point out why the algorithm is Unstable.  I belive the following reasons must be addressed.:

  *	Instability occurs because I am using one network for actions and values.
  *	Correlations are present in sequence of observations.
  *	Small updates to Q may significantly change the policy.
  *	Regarding Correlations between the action-values and target values.
    *	Using a single network to take an action and also to tell us the value of the actions.

Solutions – this will appear in my next Q learning algorithm.  My next algorithm will handle Atari games in general, not only the cartpool game. 

  *	Create a class to handle the experience replay.
  *	A separate deep neural network to handle the calculation of the target values.

More to come with the solutions I am suggesting!

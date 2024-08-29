# MDP REPRESENTATION

## AIM:
The representation of real world scenario using Markov Decision Process by stating all the states,actions and environment with respective rewards.

## PROBLEM STATEMENT:
To develop a game which will promote to other level,when the agent complete its task correctly.
### Problem Description
If the agent unable to complete the given task,then there is no promotion to other level,when it reaches the final level,it will recieve a reward.

### State Space
{L1,L2,L3}--->{0,1,2}
### Sample State
L1--->{0}

### Action Space
Moving Left(1)

Stay in the same level(0)

### Sample Action
Stay in the same level(0)

### Reward Function
+1(When it reaches the goal state or final level)

### Graphical Representation
![1](https://github.com/Sucharithachowdary/mdp-representation/assets/94166007/a2972744-54fc-49c9-8bc1-05e3faede7f1)



## PYTHON REPRESENTATION:
~~~
P = {
    0:{
        0: [(0.44,0,0,True),(0.13,1,0,False)],
        1: [(0.13,1,0,False),(0.44,0,0,True)]
    },
    1:{
        0: [(0.44,1,0,False),(0.13,2,1,True)],
        1: [(0.13,2,1,True),(0.44,1,0,False)]
    },
    2:{
        0: [(0.44,2,1,True),(0.13,1,1,False)],
        1: [(0.13,1,1,False),(0.44,2,1,True)]
    }
}
P
~~~

## OUTPUT:
![Screenshot (29)](https://github.com/Sucharithachowdary/mdp-representation/assets/94166007/8cfafaa5-b383-4e0c-bab2-f00a71194759)


## RESULT:
Therefore an MDP representation has been created for a real world scenario with all the states, actions and rewards.

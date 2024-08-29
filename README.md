# MDP REPRESENTATION

## AIM:
The aim of this MDP is to model the decision-making process of a person while coding, considering two levels of concentration - full concentration and half concentration, and to maximize productivity

## PROBLEM STATEMENT:
The person wants to get the gold he has two room left and right, room a and room c.

### Problem Description
 In this scenario, The person wants to get the gold he has two room left and right, room a and room c. If the man go room a he will get nothing.If the man go to room c he will get gold.

### State Space
Room a, Room b, Room c

### Sample State
Room C

### Action Space
Right (1) and left(0)

### Sample Action
Right, reward 1

### Reward Function
1-> he will get reward
</br>
0-> otherwise

### Graphical Representation
<img src='https://github.com/Saran408/mdp-representation/assets/75235427/8ae43d8e-1c77-4116-abf9-13c1c0e3a40d' width=50%>


## PYTHON REPRESENTATION:
```python
mdp = {
    "Room C": {
         0 : [(0.7, "Room b", 0, False),(0.3, "room c", 1, True)],
        1 : [(0.8, "room c", 1, True),(0.2, "Room b", 0, False)]
    },
    "Room B": {
        0 : [(0.8, "rooom a", 0, False),(0.2, "Room b", 0, False)],
        1 : [(0.9, "room c", 1, True),(0.1, "Room b", 0, False)]
    },
    "Room A": {
         0 : [(0.8, "room a", 0, False),(0.2, "room b", 0, False)],
        1 : [(0.7, "Room b`", 0, False),(0.3, "room a", 0.0, False)]
    }
}

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/7f3d5d41-eb97-4dd2-abe1-b8732cd0c1be)

## RESULT:
The result of solving this MDP would be an optimal policy that tells the person which action to take in each state to maximize their productivity while coding.

# MDP REPRESENTATION

## AIM:
To create an environment to check whether the child plays or stay at home according to the weather conditions.

## PROBLEM STATEMENT:

### Problem Description
Children looking for playing outdoor games. Action is based on the weather conditions, if it is a sunny day there is a high chance of playing or if it is a cloudy day, they simply stay at home.

### State Space
{C,W,S} -> {0,1,2}
where,
C-cloudy, W-weather, S-sunny

### Sample State
Sunny

### Action Space
{play, stay}

### Sample Action
play

### Reward Function
1: happy if they play
0: pale if they stay

### Graphical Representation

![307216349-c0cc14ee-ab6f-4c1e-8908-2821b8416ccc](https://github.com/user-attachments/assets/0372a1b7-57d7-4a27-9b27-4e6e0e75ec83)


## PYTHON REPRESENTATION:
```
Developed By: ARVIND S
Reg. No: 212222240012
```
```
MDP = {
    "S": {
         0 : [(0.7, "W", 0, False),(0.3, "S", 1, True)],
        1 : [(0.8, "S", 1, True),(0.2, "W", 0, False)]
    },
    "W": {
        0 : [(0.8, "C", 0, False),(0.2, "W", 0, False)],
        1 : [(0.9, "S", 1, True),(0.1, "W", 0, False)]
    },
    "C": {
         0 : [(0.8, "C", 0, False),(0.2, "W", 0, False)],
        1 : [(0.7, "W", 0, False),(0.3, "C", 0.0, False)]
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/3ffb3a06-1eb7-4340-8ef3-a30423f08969)

## RESULT:
Thus, an environment to check whether the child plays or stay at home is created according to the weather conditions.

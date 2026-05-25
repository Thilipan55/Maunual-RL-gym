# PERSONAL JIM

So this code will (hopefully) help you (and me) understand the inner workings of a reinforcemnt learning agents, training and enviornment

I wanted to build this system from THE scratch (im talking torch.randn level scratch), so fo the first iter i have built only the enviornment that the agent will live

## ENVIORNMENT

* the grid is a nxm matrix whith walls as grid[i][j] = -1
* agent can move one step (1,2,3,4 - UP, DOWN, LEFT, RIGHT)
* IF agent moves out of bounds:
    * reward = -5.0
* IF it hits a wall:
    * rewqard = -10.0
* So we update the position and check the new pos is the goal:
    * if its not, reward = -1.0
    * if it is the goal, reward = 10.0 and done = True
  

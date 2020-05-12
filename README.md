Step 6: Explain what's going on in motion_planning.py and planning_utils.py

#planning_utils.py:

It is a script responsible for calculating a grid in order for the drone to fly it, taking into account that is actually feasible by considering obstacles, altitude and safety distnces.

This script will be called in motion_planning for the flight execution.

#motion_planning.py:

It works identically like the backyard_flyer.py in terms of logic, with a significant difference in the path calculation. 
In contrast with the backyard_flyer here the flight path is not produced by predefined waypoints but by the call of planning_utils by using a_ster, heuristic and the grid from that script.

This script will execute the flight based on motion_planning flight plan.

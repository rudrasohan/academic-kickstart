---
title: Frenet Planner
summary: Implementation of Frenet Optimal Trajectory planning for motion planning of a four wheeled autonomous vehicle. 
tags:
- Simulation
- Robotics
date: "2018-06-01"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Planner in Action [Credits_ Udacity] 
  focal_point: Smart

links:
- icon: youtube
  icon_pack: fab
  name: You Tube
  url: "https://www.youtube.com/watch?v=w0g0W0mBj1A"
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

---

[Frenet Planner](https://www.researchgate.net/publication/224156269_Optimal_Trajectory_Generation_for_Dynamic_Street_Scenarios_in_a_Frenet_Frame) is a motion planning algorithm for car-like vehicles. For a given state of a car the planner samples posssible next states in the Frenet Frame and connects them. The algorithm uses simple splines for connecting various the points. 

The splines are computed using Kinematic equations of velocities and positions with respect to time. The paths are composed of two different spliens longitudinal and transversal. The longitudinal splines are characterized by velocities where as the transversal splines are characterized by position. After the relvant splines are computed a routine filters out the splines which are not following the kinematic and saftey constraits. Finally the filtered paths are evaluated on a certain objective function which minimizes jerk in tranjectory and the most optimal one is selected for execution.

Finally we transfer the path to the path tracker algorithm which generates required velocities for the low level controller.  
 
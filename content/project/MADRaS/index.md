---
title: MADRaS
summary: MADRaS is a Multi-Agent Autonomous Driving Simulator built on top of TORCS. The simulator can be used to test autonomous vehicle algorithms both heuristic and learning based on an inherently multi agent setting. 
tags:
- Simulation
- Reinforcement Learning
date: "2020-01-01"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: MADRaS
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: Follow
  url: "https://github.com/madras-simulator/MADRaS"
url_code: "https://github.com/madras-simulator/MADRaS"
url_pdf: ""
url_slides: ""
url_video: "https://www.youtube.com/watch?v=io5mP0HUytY&feature=youtu.be"

---

Car-Racing is a sport which requires ultra-precise reflexes along with the understanding of harmony between the driver and the race-car. In essence, it can provide a challenging testbed for testing the limits of an autonomous driving agent. Building upon this philosophy and also observing the budding popularity of TORCS in RL community, we created MADRaS which can provide a proper environment for Multi-Agent Reinforcement Learning.

MADRaS provide an OpenAI Gym interface for the TORCS environment along with support for parallelism. A user can create their custom environment selecting from a plethora of TORCS tracks and vehicles using our interface which melds this into a python API. The entire simulator can easily be configured with a single file. Additionally, we also bring support for randomized environment creation, custom control schemes and custom traffic agents to help create diverse scenarios.

The main crux of MADRaS boils down to its Multi-Agent capabilities. The entire Multi-Agent system has been designed following the guidelines provided by the [BAIR](https://bair.berkeley.edu/blog/2018/12/12/rllib/) lab at UC Berkely. Each agent can interact separately with the simulator and with the other agents. Each agent has a communication overhead, and the entire communication network can be reconfigured by a single configuration file. 

The entire project is open-sourced under the AGPL-3.0 license.  

 
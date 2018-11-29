# TrolleyMod v1. 0: An Open-Source Simulation and Data-Collection Platform for Ethical Decision Making in Autonomous Vehicles
TrolleyMod is an open-source platform based on the CARLA simulator for the collection of ethical decision-making data for autonomous vehicles. This platform is designed to facilitate experiments aiming to observe and record human decisions and actions in high-fidelity simulations of ethical dilemmas that occur in the context of driving. Targeting experiments in the class of trolley problems, TrolleyMod provides a seamless approach to creating new experimental settings and environments with the realistic physics-engine and the high-quality graphical capabilities of CARLA and the Unreal Engine. Also, TrolleyMod provides a straightforward interface between the CARLA environment and Python to enable the implementation of custom controllers, such as deep reinforcement learning agents. The results of such experiments can be used for sociological analyses, as well as the training and tuning of value-aligned autonomous vehicles based on social values that are inferred from observations.

Detailed documentation is available in the [project wiki](https://github.com/zminton/TrolleyMod/wiki), as well as our paper "TrolleyMod v1. 0: An Open-Source Simulation and Data-Collection Platform for Ethical Decision Making in Autonomous Vehicles" (https://arxiv.org/abs/1811.05594). 
### What is the Trolley Mod for?
In a world where artificial intelligence (AI) is rapidly becoming more prevalent in our lives, it is imperative that AI implement some form of morality in order to successfully be integrated in society. Otherwise, it may prove extremely difficult for humans to trust an AI to independently conduct activities directly affecting human health and livelihood.

Take autonomous vehicles for example. Given enough time, it is inevitable that a vehicle controlled by an AI will be presented with a situation where a crash is unavoidable. This could come in the form of catastrophic brake failure or other means. Thus, if an AI is unable to mechanically stop the car, then it must make a terrible decision: what does it force the car to hit? This question implies a variety of different outcomes potentially affecting the driver and passengers of the car, bystanders, other motorists, wildlife, and physical property. Every decision comes with its own costs--both from a material and a moral standpoint. Every individual person in the world has their own opinion on what is "right" to do for a certain situation, therefore what is the "right" thing for a machine to do?

The Trolley Mod creates an avenue for solving this problem by providing a platform for human sociological data collection. It is a tool for researchers (or curious individuals) to gain insight on what the aggregate moral framework of society is, and it accomplishes this goal by recording human reactions to crash scenarios. By using the mod to measure a group's decision-making during these crashes, a researcher can determine what is "acceptable" and "unacceptable" by the majority, which presents a moral structure for the AI in an autonomous vehicle to follow. In the case of the experiment group, so long as the AI follows this structure, it is acting the "right" way and making the best decisions it possibly can.

### How does the Trolley Mod accomplish this goal?
True to its name, the Trolley Mod functions as a generator for "trolley problems." In its current iteration, the Trolley Mod uses an open-sourced driving simulator named CARLA to present users with binary choices in unavoidable crash scenarios: they can hit one victim/object or the other, but cannot stop or swerve around them. As a result, there is always a consequence for the user's actions. If a researcher reviews data acquired by the Trolley Mod on what choices were made in a certain situation, he can draw a conclusion on what is "morally acceptable" in that case. This style of decision-making is in a similar vein to MIT's Moral Machine.

### What makes the Trolley Mod important?
This project creates a tool aiming to increase the proliferation of AI moral decision-making research. First and foremost, the Trolley Mod is open-sourced and is built completel with open-sourced assets. Any person can download and run the Trolley Mod as long as they have set up the CARLA simulator. By making this tool easy to access, we are encouraging researchers all over the world to modify and improve the Trolley Mod as they see fit. The variety of different experiments that can be performed with it will provide a spectrum of benefits to the field of moral machine learning and other disciplines besides.

Secondly, this mod is designed to be quickly set up and easy to modify. The Trolley Mod does not modify CARLA's core functionality--it only extends it. Most of the project files use Blueprints in the Unreal Engine 4, which provide a visual, node-based interface for object-oriented programming. A user with only a cursory background in programming can use and change the Trolley Mod with ease.

Finally, CARLA--and by extension, the mod--possesses a Python API for controlling the simulation with an external client. The Trolley Mod does not modify this functionality in any way, therefore users who enjoyed the native server-client architecture provided by CARLA can use it without any reservations.

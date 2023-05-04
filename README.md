Decision and Path Planning Module
=============================

TODODOODODODODODODODODODODODODO

---

## Repository File Structure

📦Decision and Path planning module<br>
 ┣ 📂.devcontainer --> Contains the configuration of the development container for those who are using docker <br>
 ┃<br>
 ┣ 📂Exercises--> Contains the exercises discussed in the lesson. <br> 
 ┃ ┣ 📂 Part 1 --> Exercises and examples of Behavioral planning. <br>
 ┃ ┣ 📂 Part 2 --> Exercises and examples of Trajectory generation. <br>
 ┃ ┗ 📂 Part 3 --> Exercises and examples of Motion planning. <br> 
 ┃ <br>
 ┣ 📂Installation --> binary files with pre-computed intermediate results<br>
 ┃ ┣ Installation_win.md  <br>
 ┃ ┗ Installation_linux.md  
 ┃ <br>
 ┣ 📂Project<br>
 ┃ ┣ 📂planners <br>
 ┃ ┃ ┣  BehavioralPlannerFSM.py --> <br>
 ┃ ┃ ┣  cost_functions.py --> <br>
 ┃ ┃ ┣  CubicSpiral.py --> <br>
 ┃ ┃ ┣  MotionPlanner.py --> <br>
 ┃ ┃ ┣  PathPlanner.py --> <br>
 ┃ ┃ ┣  PlanningParams.py --> <br>
 ┃ ┃ ┣  SpiralBase.py --> <br>
 ┃ ┃ ┣  SpiralEquations.py --> <br>
 ┃ ┃ ┣  Structures.py --> <br>
 ┃ ┃ ┣  utils.py --> <br>
 ┃ ┃ ┗  VelocityProfileGenerator.py<br>
 ┃ ┃<br>
 ┃ ┣ 📂PythonAPI -->  <br>
 ┃ ┃ ┣  📂carla --> <br>
 ┃ ┃ ┣  📂examples --> <br>
 ┃ ┃ ┗  📂util --> <br>
 ┃ ┃<br>
 ┃ ┗ SimulatorAPI.py -->  <br>
 ┃<br>
 ┣ Dockerfile --> <br>
 ┣ requirements.txt --> <br>
 ┗ run_carla.sh --> <br>

---
## Installation

We have provided a set of instructions to install all the necessary requirements for the course in the [installation](./Installation/) directory. To ensure a seamless installation process, please follow the instructions that correspond to your operating system.

* [windows](./Installation/Installation_win.md)
* [linux](./Installation/Installation_linux.md)
---
## Project Instructions

The instructions for the project pertaining to this module are compiled within the [README.md](./Project/README.md
) file with the [Project](./Project/) directory. Please read them carefully and be sure to follow them closely.Once the project is complete, submit it to Moodle as a **zip** file that includes this repository. If you want to reduce the size of your submission, feel free to delete the **PythonAPI** directory.

---
## Disclaimer

If you are taking the course Introduction to Autonomous Vehicles and encounter any issues with the setup or tasks, please reach out to your instructors as soon as possible. They are there to help you and want to ensure you have a smooth and successful learning experience. Don't hesitate to ask them any questions you may have, and they will provide you with the support you need.


Good luck with your task! 🚀👍
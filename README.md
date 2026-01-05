# SayCan Project

**A Python implementation of the "SayCan" framework: Grounding Language in Robotic Affordances.**

This repository contains code and experiments based on the Google Research paper [Do As I Can, Not As I Say: Grounding Language in Robotic Affordances](https://say-can.github.io/). This project aims to enable robots to understand high-level natural language instructions and execute them by grounding the language model's output in the robot's physical capabilities (affordances).

##  Overview

SayCan solves the problem of connecting the vast knowledge of Large Language Models (LLMs) with the physical constraints of a robot. It works by:
1.  **Saying**: The LLM scores the probability that a specific skill is useful for the high-level instruction.
2.  **Doing**: The Value Function (Affordance Model) scores the probability that the robot can successfully execute that skill in the current state.
3.  **Acting**: The system selects the skill that maximizes the combined probability of being useful and executable.

##  Features

* **LLM Integration**: Interface for Large Language Models (e.g., GPT-3, GPT-4, or open-source equivalents) to interpret instructions.
* **Affordance Scoring**: Modules to estimate the success probability of robotic skills (Pick, Place, Navigate).
* **Task Planning**: Algorithms to sequence skills for long-horizon tasks.
* **Simulation/Real-World Support**: Support for PyBullet simulation.

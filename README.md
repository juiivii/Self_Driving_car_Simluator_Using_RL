Self-Driving Car Simulator
==========================

This project implements a complete 2D + 3D Self-Driving Car Simulator and a Reinforcement Learning agent (DQN) built completely from scratch in Python. The simulator progresses through phases — from a simple Pygame car to a fully autonomous RL-driven agent.

----------------------------------------------------
PHASES OF DEVELOPMENT
----------------------------------------------------

Phase 1: Simple Driving Simulator
---------------------------------
- Top-down 2D car using Pygame
- Arrow key controls
- Rectangular/custom track
- Basic physics (acceleration + steering)
- Road boundaries and collision detection

Phase 2: Sensors + State Representation
---------------------------------------
- Ray-based LIDAR-style sensors
- Distance measurements for walls
- Collision detection using ray intersection
- Sensor output used as state vector for RL agent

Phase 3: Reinforcement Learning Agent
-------------------------------------
- Deep Q-Learning (DQN)
- Custom Neural Network or Stable-Baselines3
- Reward shaping (forward movement, no collision)
- Epsilon-greedy exploration
- Model saving and loading
- Training and playback modes

Phase 4: Game Polish / UI
-------------------------
- Start / Reset buttons
- Stats display (episode, steps, score)
- Clean UI and improved road rendering
- Replay trained model driving autonomously

----------------------------------------------------
FEATURES
----------------------------------------------------
- Fully custom car physics (2D + 3D)
- Multi-ray sensor system
- Tracks and road generation
- DQN reinforcement learning pipeline
- Live visualization using Pygame + Matplotlib
- Training curve graphs
- Playback of trained agent
- Modular, clean Python architecture

----------------------------------------------------
PROJECT STRUCTURE
----------------------------------------------------
src/
    main.py
    main_3d.py
    car.py
    car_3d.py
    road.py
    road_3d.py
    sensors.py
    rl_agent.py
    rl_agent_3d.py
    track.py
    visualization.py

models/
    dqn_car_model.zip
    dqn_car_model_3d.zip

results/
    simple_playback_results.png

docs/
    Self_Driving_Car_Flow_Diagram.md
    Self_Driving_Car_Detailed_PPT_Content.md
    Self_Driving_Car_PPT_Content.md

requirements.txt
README.txt

----------------------------------------------------
INSTALLATION
----------------------------------------------------
Install all dependencies:

    pip install -r requirements.txt

Typical requirements include:
- pygame
- numpy
- matplotlib
- stable-baselines3
- torch (if using PyTorch version)
- opencv-python (optional)

----------------------------------------------------
HOW TO RUN THE SIMULATOR
----------------------------------------------------

Manual Driving (Phase 1):
    python src/main.py
Use arrow keys to control the car.

Train the Agent (Phase 3):
    python src/main.py --train

Playback Trained Model:
    python src/main.py --play

3D Version:
    python src/main_3d.py

----------------------------------------------------
TRAINING OUTPUT
----------------------------------------------------
During training, the program generates:
- Reward curves
- Loss curves
- Saved model checkpoints
- Playback images/screenshots

These are stored inside:

    results/
    models/

----------------------------------------------------
FUTURE IMPROVEMENTS
----------------------------------------------------
- Add PPO, TD3, or SAC algorithms
- Improved physics with acceleration curves
- Multiple cars and traffic simulation
- Lane detection or OpenCV vision integration
- Web-based UI
- Sensor noise simulation
- Mobile deployment

----------------------------------------------------
AUTHOR
----------------------------------------------------
Developed by: Jivesh Karthikeyan

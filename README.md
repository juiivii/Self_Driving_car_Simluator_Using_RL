Reinforcement Learning Self-Driving Car Simulator

A fully custom-built 2D + 3D self-driving car simulator implemented in Python.
The project evolves in multiple phases — starting with a simple Pygame-based driving simulator, and expanding into full Reinforcement Learning (DQN) with sensors, reward shaping, visualization, and playback.

Project Phases
Phase 1 — Simple Driving Simulator
Top-down 2D car using Pygame
Rectangular or custom track
Basic car physics (forward, steering)
Road boundaries
Manual driving using arrow keys

Phase 2 — Sensors + State Representation
Ray-based LIDAR-style sensors
Collision detection
Distances returned as state vector for RL
Visualization overlay

Phase 3 — Reinforcement Learning Agent
Deep Q-Learning (DQN) agent
Stable-Baselines3 or custom PyTorch implementation
Reward shaping
Training loop
Model saving + loading
Playback mode to watch trained agent drive

Phase 4 — Game Polish / UI
Reset button
Training vs Playback menu
Score / steps / episode statistics
Cleaner UI and visualization

🚀 Features (Final Simulator)
🧠 RL & AI

DQN-based reinforcement learning
State from ray sensors
Replay buffer & epsilon decay
Model checkpointing


🏎️ Vehicle Simulation
Custom 2D/3D car physics
Steering, acceleration, friction
Wall & boundary collision

🔍 Sensors
Multi-ray distance sensors
Real-time visualization

🛣️ Environment
2D and 3D road generator
Tracks + boundaries
Checkpoint-based rewards

📊 Visualization
Live simulation

Training reward graphs

Playback of saved model

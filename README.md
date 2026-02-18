# 💀 AI Doom Slayer: Deep Reinforcement Learning Agent

![Doom AI Demo](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjEx...INSERT_YOUR_GIF_HERE) 
*(Note: You can convert your MP4 to a GIF online and paste the link here for a preview)*

## 📜 Project Overview
This project implements a Deep Reinforcement Learning (DRL) agent capable of playing the classic game **DOOM** (1993). Using the **VizDoom** engine and **Stable-Baselines3**, I trained a Proximal Policy Optimization (PPO) model to navigate a 3D environment, identify enemies, and engage them autonomously.

## 🧠 Tech Stack
* **Language:** Python 3.10
* **Engine:** VizDoom (C++ based Doom Port)
* **Algorithm:** PPO (Proximal Policy Optimization)
* **Frameworks:** Gymnasium, Stable-Baselines3, OpenCV

## 🚀 How It Works
1.  **Environment Wrapper:** The raw Doom game engine is wrapped into a Gymnasium environment, converting 3D game states into pixel data.
2.  **Preprocessing:** Frames are captured, grayscale-converted, and resized to 84x84 pixels to optimize the neural network's input.
3.  **Training:** The agent uses a CNN (Convolutional Neural Network) policy to extract features from the pixels and learns through trial-and-error (Reward Signal: +Kill, -Death, -Ammo).

## 📂 Files
* `train_doom_agent.ipynb`: The complete training pipeline (Google Colab Notebook).
* `vizdoom_demo_agent.zip`: The pre-trained model weights.
* `doom_final_cut.mp4`: Video demonstration of the agent in action.

## 🛠️ Installation & Usage
This project is designed to run in **Google Colab** to handle the heavy rendering dependencies.
1. Open `train_doom_agent.ipynb` in Colab.
2. Run the "Install Dependencies" cell to setup VizDoom and Linux libraries.
3. Run the "Load Model" cell to watch the pre-trained agent.

## 📈 Results
After 50,000 timesteps of training, the agent successfully learned to:
* Identify the monster from visual cues.
* Navigate the corridor without getting stuck.
* Fire accurately to eliminate the target.

---
*Built with 🩸 and Python.*

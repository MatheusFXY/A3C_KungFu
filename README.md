# 🟥 SDS_A3C_KungFu

This project trains an AI agent to play Kung Fu Master using the **A3C algorithm** (Asynchronous Advantage Actor-Critic), a reinforcement learning technique that uses multiple parallel agents to accelerate and stabilize learning.

---

## 📘 Project Overview  

The Kung Fu agent is trained to:

🧍 Understand its current state (position, health, enemies, attacks)  
🥋 Decide the best action (move, punch, kick, jump, or idle)  
🎯 Learn through trial and error across multiple environments  
💪 Maximize cumulative rewards (survival, damage dealt, enemies defeated)  
🛡️ Avoid penalties (taking hits, losing lives, game over)

The model is built using a neural network with two outputs:

- `action_values`: used by the **actor** to decide which action to take  
- `state_value`: used by the **critic** to evaluate the quality of the state  

The **advantage function** helps the model decide how much better an action is compared to the average, improving both decision-making and learning speed.

Each agent runs in its own environment and trains independently, but all update a **shared global network**, which is constantly improved.

---

## ▶️ Run the Project in Google Colab  

No local installation is required — run directly in the cloud:

👉 [Open in Colab](https://colab.research.google.com/drive/1J25hVVEwCZ5JaD_oAL_JgFvNgHt6-aLA#scrollTo=pz8ogVxGVB6b)

---

## 🧠 Key Concepts Covered  

✅ Asynchronous Advantage Actor-Critic (A3C)  
✅ Parallel environment simulation  
✅ Actor-critic architecture  
✅ Advantage calculation for better learning  
✅ Reward scaling and entropy for exploration  
✅ Loss functions: actor loss + critic loss  
✅ Gradient descent using PyTorch  
✅ Automatic reset of environments on episode end  
✅ Evaluation logic and average performance check

---

## 💡 Bonus  

The code uses `tqdm` to show a real-time training progress bar and auto-saves performance metrics at checkpoints.

---

## 📚 References  

- SuperDataScience – Hadelin & Kirill  
- DeepMind: Asynchronous Methods for Deep Reinforcement Learning (Mnih et al., 2016)

---

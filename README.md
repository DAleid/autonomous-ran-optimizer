# RAN Optimizer Agent

An autonomous AI agent system for Radio Access Network (RAN) optimization, combining Deep Reinforcement Learning with multi-agent coordination to automatically tune network parameters and improve performance.

## Overview

This project implements an end-to-end autonomous optimization pipeline for RAN networks. Agents learn to adjust parameters — increasing throughput, reducing call drops, and optimizing energy consumption — without manual operator intervention.

## Key Capabilities

- **Autonomous Optimization** — Agents learn and apply tuning decisions without human intervention
- **Deep Q-Learning (DQN)** — State-of-the-art reinforcement learning for parameter tuning
- **Multi-Agent Coordination** — Specialized agents for monitoring, planning, and execution
- **A/B Testing** — Safe rollout of changes before full network deployment
- **Self-Healing** — Autonomous fault detection and recovery
- **Multi-Vendor Support** — Works across different RAN equipment vendors

## Project Structure

```
RAN_Optimizer_Agent/
  agents/          # AI agent definitions (RAN agents, crew, tasks)
  data/            # 6G HetNet dataset
  results/         # Optimization outputs
  healing_demo.py  # Self-healing demonstration
  multi_vendor_demo.py  # Multi-vendor scenario demo
  requirements.txt
```

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Language | Python |
| ML Framework | Deep Q-Learning (DQN) |
| Agent Orchestration | CrewAI |
| Dataset | 6G HetNet Transmission Management |
| Environment | Simulated RAN network |

## Getting Started

```bash
git clone https://github.com/DAleid/RAN_Optimizer_Agent.git
cd RAN_Optimizer_Agent/RAN_Optimizer_Agent
pip install -r requirements.txt
cp .env.example .env    # Add your API keys

# Run self-healing demo
python healing_demo.py

# Run multi-vendor demo
python multi_vendor_demo.py
```

## Documentation

See [`RAN_Optimizer_Agent/`](RAN_Optimizer_Agent/) for full architecture documentation, quickstart guide, and deployment instructions.

## License

MIT License
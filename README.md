# 🚀 Neuro-Symbolic Framework for Autonomous Verilog Generation

An end-to-end automated pipeline running in Google Colab that generates hardware description language (Verilog) blueprints and utilizes an autonomous symbolic feedback loop to self-correct logical and syntax execution errors in real-time.

---

## 🧠 Architectural Overview
This repository implements a hybrid **Neuro-Symbolic AI Loop** designed to bridge the gap between stochastic language generation and deterministic hardware compilation. 

### ⚙️ How It Works
1. **The Generator Block:** Implements in-context learning patterns to prime pre-trained LLMs (`distilgpt2`) for targeted structural Verilog generation.
2. **The Symbolic Referee:** An automated rules engine that acts as a gatekeeper, evaluating the structural integrity of the code (e.g., syntax checking, operator validation, and physical validity constraints).
3. **The Autonomous Repair Loop:** If an error is caught by the referee, the execution context logs are compiled and dynamically injected back into the LLM as correction prompts, executing an automated patch until a perfect verification score is achieved.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python 3
* **Modeling Tools:** Hugging Face Transformers Library
* **Environment:** Google Colaboratory (Cloud-hosted Linux runtime environment)
* **Target Hardware Logic:** Verilog HDL (AND, OR, NOT gate structural level simulations)

---

## 📈 Future Scalability & Production Roadmap
* **Advanced Code Intelligence:** Upgrade the foundational model layer from standard text models to production-grade coding agents like `DeepSeek-Coder` or `Qwen-Coder`.
* **Industrial Hardware Simulators:** Replace the algorithmic Python checker loop with a production compiler toolchain like `Verilator` or `Icarus Verilog` to capture accurate timing constraints and synthesis errors.
* **Dataset Scaling:** Stream open-source RTL hardware collections (e.g., `MG-Verilog`) directly into the pipeline workflow.

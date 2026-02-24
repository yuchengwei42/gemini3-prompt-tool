# Gemini 3 Prompt Composer

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

A structured, research-backed prompt engineering tool that lets you harness the latest breakthroughs in LLM reasoning — especially **Society of Thought** (Kim et al., 2026).

➡️ **Live Demo:** [**https://yuchengwei42.github.io/gemini3-prompt-tool/**](https://yuchengwei42.github.io/gemini3-prompt-tool/)

![Demo GIF](demo.gif)

---

### 💡 Motivation

Modern reasoning models like DeepSeek-R1 and Gemini 3 do not simply produce longer chains of thought. According to the latest research, their superior performance comes from **internally simulating a society of thought** — a dynamic, multi-agent debate among distinct cognitive perspectives with diverse personalities and expertise.

This tool was built to make that breakthrough accessible: you can construct prompts using clean blocks, then instantly activate paper-verified reasoning strategies with one click.

### ✨ Key Features

*   **🧱 Block-Based Editor** — Role, Task, Context, Code, Constraints… reorder freely.
*   **Society of Thought Mode** (New!) — Directly implements the conversation-style scaffolding from Kim et al. (2026). The model simulates 3 distinct thinkers (Meticulous Verifier + Creative Strategist + Skeptical Auditor) engaging in realistic back-and-forth debate inside `<think>` tags. Disagreements are encouraged. No fixed turn order. Forces consensus before final answer.
*   **Classic CoT & Prompt Repetition** — Toggle traditional techniques for comparison or specific use cases.
*   **Research-Backed Presets** — Includes "Society of Thought (Paper Verified)" and Karpathy-style simulator.
*   **Export & Share** — Copy or save as `.txt`/`.md`.
*   **Multi-Language UI** — English, 繁體中文, 日本語.
*   **100% Private** — Everything stays in your browser.

### 🔬 Academic Foundations

This tool directly implements techniques from influential papers:

**1. Society of Thought (Core Feature)**  
> Enhanced reasoning emerges from the implicit simulation of complex, multi-agent-like interactions — a "society of thought".  
> 
> *Kim, J. et al. (2026). Reasoning Models Generate Societies of Thought. arXiv preprint.*

The **Society of Thought** mode in this tool reproduces the exact conversation-style SFT prompt used in the paper, including:
- Distinct personas with Big Five personality differences
- Realistic back-and-forth dialogue (any order, multiple turns)
- Encouragement of disagreement and perspective conflict
- Strict XML structure (`<think>`, `<thinker1>`, etc.)
- Forced consensus before final answer

**2. Chain of Thought (CoT)**  
Kojima et al. (2022). *Large Language Models are Zero-Shot Reasoners*.

**3. Prompt Repetition**  
Observed technique that improves instruction adherence in certain models.

---

### 🛠️ Tech Stack

*   Vue 3 (Composition API) + Tailwind CSS
*   Font Awesome
*   Browser `localStorage` only

### 🤝 Contributing

Contributions welcome! Especially ideas to add more paper-verified modes (Tree-of-Thoughts, Graph-of-Thoughts, etc.).

### 📄 License

MIT © 2026 Yu-Cheng Wei

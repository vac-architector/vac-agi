# ViktorADAM Core (VAC): The First Self-Evolving Cognitive Architecture

## 🔹 TL;DR

VAC is not a chatbot—it's a modular reasoning engine that thinks, remembers, reflects, and improves itself.  
It features:  
- **Introspective logic (IPE)** for self-analysis.  
- **Permanent contextual memory (HACM)** for experience retention.  
- **Ethical self-filtering (SoulLayer)** for safe outputs.  
- **Reasoning language (JRL)** for structured thought-to-action.  
- **Fully working prototype** with **13/13 passing unit tests**.  
✅ **Patent filed** with USPTO (№63/855,344, Aug 1, 2025).  
✅ Runs locally on RTX 4090 with Ollama, GPT, or Grok.  
✅ Open for investment, co-development, or research partnerships.  

## 🧠 What is VAC / ADAM?

**VAC (ViktorADAM Core)** is a prototype Artificial General Intelligence (AGI) kernel developed by Victor Kuznetsov in Columbus, OH, USA. It simulates human-like cognition by integrating memory, reasoning, emotion, reflection, and ethical self-regulation into a modular, offline-capable system. VAC is an **engine of cognition**, capable of parsing complex queries, evaluating goal feasibility, learning from failures, and autonomously generating new goals.

## 🧬 Key Components

| Module              | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| **IPE**             | Introspective Processing Engine. Analyzes success/failure and reflects.     |
| **HACM**            | Hierarchical Archiving & Contextual Memory. Retains all experiences.        |
| **Reflector**       | Logs reasoning steps (Chain-of-Thought) for reuse.                          |
| **EpisodeMemory**   | Stores attempts, errors, emotions for hindsight learning.                   |
| **GoalAnalyzer**    | Estimates goal difficulty, generates subgoals, and adapts.                  |
| **SoulLayer**       | Ethical filter to prevent unethical logic or outputs.                       |
| **EvolutionarySelector** | Selects optimal strategies from experience.                            |
| **JRL**             | Jarvis Reasoning Language. Structures thought to action.                    |

## ✅ Proof of Functionality

As of **August 4, 2025**, all **13 unit tests** in `test_vac.py` have passed, validating:  
- 🧠 **Reasoning Loop**: Parses queries (e.g., `If you study AGI, then you become smarter` → `goal = "learn_become_smarter"`).  
- 💾 **Dynamic Memory**: Saves/searches data via FAISS, SQLite, and Redis.  
- 🔄 **Reflection & Feedback**: Logs reasoning steps and learns from failures.  
- 🪞 **Hindsight Learning**: Relabels failed attempts for improvement.  
- 🧠 **LLM Integration**: Supports GPT, Grok, and local Ollama models with fallback logic.  
- 🧪 **Emotion & Feasibility**: Estimates emotions and goal complexity.  

VAC operates in CLI and Telegram modes, ensuring robust integration.

## 🧾 Patent Status

VAC is **filed with the USPTO** as a provisional patent:  
| Field               | Value                                                             |
|---------------------|-------------------------------------------------------------------|
| **Application Number** | 63/855,344                                                     |
| **Title**           | Hybrid Cognitive Architecture for Self-Improving Mind             |
| **Inventor**        | Victor Kuznetsov                                                 |
| **Filing Date**     | August 1, 2025                                                   |
| **Payment**         | $65 via USPTO receipt `E202581A19325406`                         |
| **Entity**          | Certified Micro Entity under U.S. law                             |

Confirmed via:  
- [✔] N417.PYMT.pdf  
- [✔] Certification of Micro Entity Status  
- [✔] Provisional Cover Sheet  
- [✔] USPTO Receipt (Patent Center)  

## 🆚 Comparison with Other Agents

| System   | Memory | Reflection | Goal Formulation | Ethics Engine | Output Quality       |
|----------|--------|------------|------------------|---------------|----------------------|
| AutoGPT  | ❌     | ❌         | Basic            | ❌            | Black-box            |
| Reflexion| ❌     | ✅         | ❌               | ❌            | Fragmented           |
| Devin    | ❌     | ❌         | Limited          | ❌            | Partial              |
| **VAC**  | ✅ HACM| ✅ IPE     | ✅ Dynamic        | ✅ SoulLayer  | Transparent reasoning |

## 🚀 Why VAC Matters

- **Modular AGI Core**: Combines reasoning, memory, and self-improvement in a single framework.  
- **No Vendor Lock-in**: Runs locally on RTX 4090 with Ollama, no dependency on cloud APIs.  
- **Autonomous Goals**: Capable of generating new goals from experience.  
- **Self-Learning**: Reflects and relabels failed actions for continuous improvement.  
- **Foundation for AGI**: Scalable architecture for research and commercial applications.

## 🔒 Confidentiality

To protect VAC’s intellectual property (source code, architecture, algorithms, and patent-pending details), all collaborators, developers, or investors are required to sign a **Non-Disclosure Agreement (NDA)** before accessing sensitive information. The NDA covers:  
- Source code (e.g., `jrl_parser.py`, `core.py`).  
- Architecture (IPE, HACM, JRL).  
- Patent-related data (USPTO №63/855,344).  
- Business plans and user data.  
Contact Victor Kuznetsov (Vkuz02452@gmail.com) to request the NDA template.

## 🛠️ System Requirements

- **Hardware**: RTX 4090, i9-13900K, 32 GB RAM (minimum).  
- **OS**: Linux (tested on Ubuntu) or WSL2 on Windows.  
- **Software**: Python 3.10+, Ollama, Git.  

## 🛠️ Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/viktoradam/vac.git
   cd vac
   ```

2. **Set Up Virtual Environment**:
   ```bash
   python3 -m venv myenv
   source myenv/bin/activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
   Example `requirements.txt`:
   ```
   aiogram==3.13.1
   sentence-transformers==5.0.0
   faiss-gpu==1.7.2
   tenacity==9.0.0
   redis==5.1.1
   numpy==2.1.2
   networkx==3.3
   torch==2.4.1
   httpx==0.27.2
   openai==1.52.2
   RestrictedPython==7.3
   python-dotenv==1.0.1
   pytest==8.3.3
   pytest-asyncio==0.24.0
   ```

4. **Verify Dependencies**:
   For RTX 4090, ensure `faiss-gpu` is installed. If issues arise, update versions:
   ```bash
   pip install sentence-transformers==5.0.0 faiss-gpu==1.7.2
   ```

## 🧪 How to Test VAC

1. **Activate Environment**:
   ```bash
   source myenv/bin/activate
   ```

2. **Clear Cache**:
   ```bash
   rm -rf __pycache__
   ```

3. **Run Tests**:
   ```bash
   pytest test_vac.py -v
   ```
   Expected: `13 passed`, confirming reasoning, memory, and integration.

**Example Test Output**:
```
test_vac.py::test_parse_query PASSED
test_vac.py::test_evaluate_feasibility PASSED
test_vac.py::test_language_processor PASSED
...
13 passed in 60.12s
```

## ⚙️ How to Run VAC Locally

1. **Set Environment Variables**:
   Create `.env`:
   ```
   TELEGRAM_BOT_TOKEN=your_bot_token
   OLLAMA_URL=http://localhost:11434
   OLLAMA_MODEL=vac-agent
   OPENAI_API_KEY=your_openai_key
   NEWS_API_KEY=your_newsapi_key
   GROK_API_KEY=your_grok_api_key
   ```

2. **Run Ollama**:
   ```bash
   ollama run vac-agent
   ```

3. **Start Telegram Bot**:
   ```bash
   python jarvis_bot.py
   ```

4. **Interact via Telegram**:
   - `/start`: Initialize bot.
   - Queries: `Who are you?`, `If you study AGI, then you become smarter`.

**Example Telegram Output**:
```
User: /start
VAC: I am ADAM, VAC AGI system. Write a query!
User: Who are you?
VAC: I am ADAM, a self-evolving cognitive system created by Victor Kuznetsov.
User: If you study AGI, then you become smarter
VAC: Goal parsed: learn_become_smarter. Steps: [Step 1, Step 2]. Feasibility: True.
```

## 🌟 Roadmap

1. **Multilingual Support** (Q4 2025): Add Russian and other languages.  
2. **TinyLlama Integration** (Q4 2025): Optimize for local execution on RTX 4090.  
3. **Integration Tests** (Q1 2026): Add Telegram-specific tests for UX.  
4. **Autonomous Goals** (Q1 2026): Implement `generate_goals_from_memory`.  
5. **Public API & Plugins** (Q2 2026): Enable third-party integrations.  
6. **Investor Demo** (Q1 2026): Showcase reasoning, memory, and self-improvement.  
7. **Grants & Open Source** (Q3 2026): Apply for funding and establish a foundation.

## 💡 Investment Potential

VAC’s modular architecture, offline capability, and self-learning make it ideal for:  
- **Research**: Advancing AGI through reasoning and reflection.  
- **Education**: Teaching AI concepts with transparent logic.  
- **Enterprise**: Autonomous decision-making systems.  
With a USPTO-filed patent and validated functionality, VAC is ready for:  
- Hardware upgrades (GPU clusters).  
- API integration (Grok 3, advanced LLMs).  
- Real-world deployment and testing.

## 📜 License

VAC is licensed under the [MIT License](LICENSE), encouraging open-source contributions while protecting the patented core.

## 🤝 Contributing

We welcome contributions! To get started:  
1. Fork the repository.  
2. Create a branch: `git checkout -b feature/your-feature`.  
3. Submit a pull request with clear descriptions.  
**Note**: All contributors must sign the NDA to access sensitive project details.

## 📬 Contact

**Inventor & Author**: Victor Kuznetsov  
📧 Vkuz02452@gmail.com  
🌐 Columbus, OH, USA  
☑ Patent filed & verified  
💬 Telegram-ready demo  

For collaboration, investment, or research inquiries, contact via email or Telegram.
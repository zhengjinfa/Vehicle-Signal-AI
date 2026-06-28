# Vehicle-Signal-AI
Intelligent Automotive Fault Diagnosis Assistant
# 🧠 CANme-AI — Intelligent Automotive Fault Diagnosis Assistant

**CANme-AI** is a **local‑first, AI‑enhanced diagnostic assistant** for automotive CAN/LIN bus systems.  
It parses raw ASC log files together with DBC or LDF databases, extracts and visualizes every signal **without downsampling**, and uses a built‑in rule engine or optional large language models (local/cloud) to help you pinpoint the root cause of intermittent faults — in minutes, not days.

> ⚠️ **All data processing happens locally.** No raw log files or signals ever leave your computer unless you explicitly choose to use a remote LLM, and even then only summarized logical features are sent.

---

## ✨ Key Features

- **📂 Multi‑format support**  
  ASC (Vector logging), DBC, LDF — auto‑detects CAN or LIN.

- **📈 True waveform visualization**  
  ECharts-based, no decimation — every signal sample is rendered.

- **🔍 Anomaly detection engine**  
  Identifies zero‑jumps, return‑to‑zero, value spikes, message timeouts, and range violations.

- **🤖 AI‑powered diagnosis (optional)**  
  Choose between **local models** (Ollama / LM Studio) or **cloud models** (DeepSeek, OpenAI …)  
  Model presets and configurable endpoints make setup easy for non‑experts.

- **🧩 Modular analysis workflow**  
  Upload logs + database → select suspect signals → run local or AI analysis → receive a structured report.

- **🌐 Trilingual UI**  
  English, Chinese (中文), German (Deutsch) — fully switchable at runtime.

- **🔒 Privacy first**  
  Built for engineers in regulated industries; local rule engine is fully offline and always free.

---

## 🚀 Quick Start

1. **Open `index.html`** directly (no build step required) or use the bundled Electron desktop app.
2. Load an ASC file and a DBC/LDF database.
3. (Optional) Paste functional specification snippets.
4. Mark suspicious signals in the checkbox list.
5. Click **“Start Analysis”** for AI reasoning, or **“Offline Simulation”** for the built‑in rule engine.
6. Explore the anomaly report and full‑resolution waveform.

---

## 🖥️ Desktop App (Electron)

A packaged desktop version is available under [Releases](https://github.com/yourusername/CANme-AI/releases) for Windows, macOS and Linux.  
It offers the same functionality with native file dialogs and better offline capability.

---

## 🧩 Model Presets

| Type       | Preset        | Default Endpoint |
|------------|---------------|------------------|
| Local      | Ollama        | `http://localhost:11434/v1` |
| Local      | LM Studio     | `http://localhost:1234/v1`  |
| Online     | DeepSeek      | `https://api.deepseek.com/v1` |
| Online     | OpenAI        | `https://api.openai.com/v1` |
| Custom     | Any OpenAI‑compatible API | User‑defined |

---

## 📸 Screenshots

<img width="1166" height="896" alt="c381291e60c931de6e76a4d34eb30e49" src="https://github.com/user-attachments/assets/fe9cb2eb-a1ed-45f6-91e4-e61bf5bb24bd" />


<img width="1151" height="826" alt="2cc28be066a9aee3667e734978d42441" src="https://github.com/user-attachments/assets/b6e87d52-0941-4a2b-9a5a-3f20adbc2233" />

<img width="1098" height="606" alt="2c4b160e5a2bd8a8d98bd84e40e63e84" src="https://github.com/user-attachments/assets/b72623d9-c887-495d-baeb-59704cc96d51" />


---

## 🛠️ Tech Stack

- Pure frontend: **HTML5 + JavaScript + ECharts**  
- Document parsing: **Mammoth.js** (for .docx specs)  
- Optional desktop shell: **Electron**  
- AI clients: OpenAI‑compatible API (local or remote)

---

## 📝 Roadmap

- [ ] CAN‑FD & J1939 support  
- [ ] Signal comparison overlay  
- [ ] Export diagnostic reports as PDF  
- [ ] Real‑time streaming via SocketCAN / PeakCAN  
- [ ] Plugin system for custom detectors

---

## 🤝 Contributing

Contributions are welcome! Please open an issue or pull request.  
For major changes, discuss first in Discussions.

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.  
Free for personal, educational, and commercial use.

---

**If CANme-AI helps you fix an elusive bug, consider giving the repo a ⭐!**

📱 Contact Me on WeChat :zhengjinfa33

📧 Email:zhengjinfa33@163.com

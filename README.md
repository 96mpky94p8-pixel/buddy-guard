# buddy-guard
# 🛡️ BuddyGuard: Dual-Channel Autonomous Discord AI Framework

An autonomous Discord AI companion powered by Gemini API, featuring a **physical dual-channel security architecture** to mitigate prompt injection and hallucinations in real time.

---

## ⚡ The Core Problem: Why Existing Guardrails Fail
Traditional LLM bots process prompts and safety instructions in the same execution context. If a malicious user uses clever jailbreak prompts, single-prompt guardrails can easily collapse.

### The Solution: Physical Channel Isolation
Instead of relying on a single prompt, this bot enforces an **out-of-band audit**:
* **`#general` (Public Interaction)**: The AI chats and interacts autonomously.
* **`#security-room` (Isolated Audit)**: A secondary, independent evaluation layer continuously monitors conversation logs and triggers an automated killswitch if hostile behavior is detected.

> **Zero Context Contamination**: The safety monitor is physically separated from user-facing prompts, ensuring prompt injection cannot bypass the watchdog.

---

## ✨ Features
* 🤖 **Autonomous Conversation**: Natural, periodic check-ins driven by dynamic loop timers.
* 🔒 **Dual-Channel Guardrails**: Real-time prompt auditing via dedicated audit channels.
* 🚨 **Instant Killswitch**: Automatic lockdown if anomalous outputs or security breaches occur.
* 🚀 **Drop-in Discord Integration**: Built with `discord.py` and Google AI Studio (Gemini).

---

## 🛠️ Quick Start

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name
pip install -r requirements.txt

2. Configure Environment Variables
Create a ⁠.env⁠ file in the root directory:

DISCORD_BOT_TOKEN=your_discord_token
GEMINI_API_KEY=your_gemini_api_key
AUDIT_CHANNEL_ID=your_security_room_channel_id

Run the Bot

python bot.py

☕ Support & Sponsorship
If you find this dual-channel architecture useful for your own Discord communities, consider supporting continued development!




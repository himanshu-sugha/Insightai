# InsightAI 🔍

> **Agentic AI Research Assistant** powered by Cortensor's decentralized inference network





---

## 🎯 What is InsightAI?

InsightAI is a **decentralized AI research assistant** that acts autonomously to provide verified research insights. Instead of relying on a single AI provider, InsightAI leverages Cortensor's **multi-miner consensus** and **blockchain verification** for trustworthy outputs.

### Why Decentralized Research?

| Traditional AI | InsightAI + Cortensor |
|----------------|----------------------|
| Single provider = single point of failure | 94+ distributed miners |
| No verification of outputs | Blockchain TX verification |
| Opaque inference process | Session + Task ID transparency |
| Centralized trust | Decentralized consensus |

---

## 🏆 Hackathon Track: Agentic Applications

InsightAI fits the **Agentic Applications** track as an autonomous research assistant that:

- ✅ **Acts autonomously** on user queries without step-by-step guidance
- ✅ **Monitors** and handles network availability with graceful fallbacks
- ✅ **Produces verifiable outputs** with blockchain transaction verification
- ✅ **Free public access** - no API keys required for end users

---

## ⚡ Cortensor Integration 

### Features Used

| Feature | Implementation |
|---------|---------------|
| **Router Node API** | `/api/v1/completions/{sessionId}` for inference |
| **Session Management** | TestNet 0 session creation and tracking |
| **Multi-Miner Inference** | Queries processed by 94+ decentralized nodes |
| **Blockchain Verification** | TX hash provided for each response |
| **WebSocket Communication** | Real-time router node connectivity |

### Architecture

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│   InsightAI     │────▶│ Cortensor       │────▶│ Decentralized   │
│   Frontend      │     │ Router Node     │     │ Miners (94+)    │
└─────────────────┘     └─────────────────┘     └─────────────────┘
         │                       │                       │
         │                       ▼                       │
         │              ┌─────────────────┐              │
         │              │ Session #127    │              │
         │              │ Gemma 3 270M    │              │
         │              └─────────────────┘              │
         │                       │                       │
         │                       ▼                       │
         └──────────────│ Blockchain TX   │◀─────────────┘
                        │ Verification    │
                        └─────────────────┘
```

### API Request Example

```javascript
POST /api/v1/completions/127
{
  "prompt": "Research the future of decentralized AI",
  "stream": false,
  "timeout": 30
}
```

---

## 🎨 Functionality & Stability 

### Core Features

- 🔍 **Research Query Interface** - Natural language research questions
- 🌐 **URL Analysis** - Summarize content from any web page
- ✅ **Verified Results** - Badge shows Cortensor verification status
- 📊 **Structured Output** - Summary + bullet points format
- 🔄 **Graceful Fallback** - Demo mode when TestNet unavailable

### Error Handling

- Automatic retry on network failures
- 15-second timeout with graceful degradation
- Input validation (query length, content)
- Rate limiting to prevent abuse

---

## 💡 Originality & Technical Depth (20% of Score)

### Unique Value Proposition

1. **Research-First Agent** - Purpose-built for research queries, not general chat
2. **Verifiable Intelligence** - Every response links to Cortensor dashboard
3. **Structured Output Parsing** - Extracts summaries and bullet points from LLM responses
4. **URL Intelligence** - Fetches and analyzes web content through decentralized inference

### Tech Stack

- **Framework**: Next.js 16 (App Router + Turbopack)
- **Styling**: Tailwind CSS v4 with glassmorphism design
- **Components**: shadcn/ui
- **Backend**: Cortensor Router API
- **Blockchain**: Arbitrum Sepolia TestNet
- **Deployment**: Vercel (Edge Functions)

---

## 🖥️ Usability & Demo Quality 

### Premium UI Features

- 🌙 Dark mode with glassmorphism effects
- ✨ Smooth animations and micro-interactions
- 📱 Fully responsive design
- 🎯 One-click research queries
- 🔗 Direct links to verification dashboard

### Demo Walkthrough

1. Enter any research question
2. Watch real-time processing indicator
3. Receive structured results with verification badge
4. Click verification link to see on Cortensor dashboard

---

## 🌍 Public Good Impact 

- **Free Access**: No API keys or accounts required for end users
- **Open Source**: MIT licensed, fully available on GitHub
- **Community Value**: Demonstrates Cortensor integration patterns
- **Documentation**: Complete setup and integration guides
- **Educational**: Shows how to build agentic apps on Cortensor

---

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/himanshu-sugha/Insightai
cd insightai

# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

### Environment Variables

Create `.env.local`:

```env
# Cortensor Router Configuration
CORTENSOR_ROUTER_URL=http://localhost:5010
CORTENSOR_API_KEY=your-api-key-from-dashboard
CORTENSOR_SESSION_ID=127

# Demo mode (set true if no router available)
USE_MOCK=false
```

---

## 🤖 Agent Specification

### Actions

| Action | Description |
|--------|-------------|
| `research_query` | Process natural language research questions |
| `url_analysis` | Fetch and summarize web content |
| `structured_output` | Format response as summary + bullet points |
| `verification_link` | Provide Cortensor dashboard link |

### Safety Guardrails

- 🛡️ Rate limiting on API requests
- 🛡️ Input validation (length, content)
- 🛡️ Timeout handling with graceful fallback
- 🛡️ No PII storage on server
- 🛡️ Demo mode fallback for availability

---

## 📋 Transparency Notes

- **Centralized Components**: Vercel hosting, Next.js server functions
- **No Paid Services**: Uses only Cortensor TestNet (free) and Vercel free tier
- **Data Sources**: User-provided queries, public URLs only

---


---

## 🔗 Links

- **Live Demo**: [https://insightai-chi.vercel.app/](https://insightai-chi.vercel.app/)
- **GitHub**: [https://github.com/himanshu-sugha/Insightai](https://github.com/himanshu-sugha/Insightai)
- **Community PR**: [cortensor/community-projects #78](https://github.com/cortensor/community-projects/pull/78)

---

## 📝 License

MIT License - see [LICENSE](LICENSE) file.
https://insightai-chi.vercel.app/
---

**Built for Cortensor Hackathon #3** 🚀

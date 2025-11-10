# OmniDash Demo

**Public demo version of OmniDash - OmniNode Platform Dashboard**

This is a **demo-only repository** showcasing the OmniDash monitoring interface with simulated data. No real backend services are required.

## 🎯 Demo Mode

This repository runs in **pure mock data mode** - all metrics, charts, and data visualizations use realistic simulated data. Perfect for:

- Exploring the dashboard UI and features
- Understanding OmniNode platform capabilities
- Screenshots and demonstrations
- Frontend development without backend dependencies

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm
- No database, Kafka, or backend services required!

### Installation

1. Clone the repository:
```bash
git clone https://github.com/OmniNode-ai/omnidash-demo.git
cd omnidash-demo
```

2. Install dependencies:
```bash
npm install
```

3. Create your environment file:
```bash
cp .env.example .env
```

**The `.env.example` is pre-configured for demo mode** - you don't need to modify anything!

4. Start the development server:
```bash
PORT=3000 npm run dev
```

5. Open your browser to [http://localhost:3000](http://localhost:3000)

## 📊 Dashboard Features

Explore 9 comprehensive monitoring dashboards:

- **Agent Operations** (`/`) - Monitor 52 AI agents and their execution
- **Pattern Learning** (`/patterns`) - View code pattern discovery and quality
- **Intelligence Operations** (`/intelligence`) - Track AI operations and workflows
- **Code Intelligence** (`/code`) - Code quality analysis and ONEX compliance
- **Event Flow** (`/events`) - Real-time event processing metrics
- **Knowledge Graph** (`/knowledge`) - Visualize code pattern relationships
- **Platform Health** (`/health`) - System health monitoring
- **Developer Experience** (`/developer`) - Workflow and productivity metrics
- **Chat** (`/chat`) - AI assistant interface

## 🎨 Tech Stack

- **Frontend**: React + TypeScript + Vite
- **UI**: shadcn/ui (New York variant) + Tailwind CSS
- **Design**: Carbon Design System principles
- **State**: TanStack Query v5
- **Charts**: Recharts
- **Routing**: Wouter

## 🔧 Available Scripts

```bash
# Development
PORT=3000 npm run dev          # Start dev server on port 3000

# Testing
npm run test                    # Run tests
npm run test:ui                 # Interactive test UI
npm run test:coverage           # Generate coverage report

# Production
npm run build                   # Build for production
PORT=3000 npm start            # Run production build
```

## 🎭 Demo vs Production

This demo repository differs from the production version:

| Feature | Demo Mode | Production |
|---------|-----------|------------|
| **Data Source** | Simulated mock data | PostgreSQL + Kafka + APIs |
| **Backend Required** | ❌ No | ✅ Yes |
| **Database** | ❌ None | PostgreSQL at 192.168.86.200 |
| **Event Streaming** | ❌ None | Kafka/Redpanda |
| **Real-time Updates** | ✅ Simulated | ✅ WebSocket |

## 📝 Mock Data System

Mock data is controlled by the `VITE_USE_MOCK_DATA` environment variable:

```bash
# .env file
VITE_USE_MOCK_DATA=true   # Demo mode (default in this repo)
```

The mock data system provides:
- Realistic agent execution metrics
- Code pattern discovery data
- Performance trends and time series
- System health indicators
- All dashboard visualizations

## 🔗 Related Repositories

For the full OmniNode platform with backend integration:
- [omnidash](https://github.com/OmniNode-ai/omnidash) - Full-featured dashboard (private)
- [omniarchon](https://github.com/OmniNode-ai/omniarchon) - Intelligence service (private)

## 📄 License

MIT License - see LICENSE file for details

## 🙋 Questions?

This is a demonstration repository. For questions about the full OmniNode platform, please contact the OmniNode team.

---

**Note**: This is a **public demo** with mock data only. No credentials, API keys, or real infrastructure connections are included or required.

# CEREBRO - Crypto Detection Network Platform

![CEREBRO Logo](https://img.shields.io/badge/CEREBRO-Crypto%20Detection-purple?style=for-the-badge)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-18%2B-green.svg)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-18-blue.svg)](https://reactjs.org/)

A cutting-edge crypto detection platform that uses AI agents to monitor and detect crypto runners on DEXScreener and Pump.fun. CEREBRO provides real-time analysis and pattern recognition to identify suspicious trading activity and potential opportunities.

## 🚀 Features

- **Real-time Crypto Monitoring**: Live integration with DEXScreener and Pump.fun APIs
- **AI Detection Agents**: 6 specialized agents for different crypto monitoring tasks
- **CEREBRO Token Staking**: Earn 70% of platform fees through token staking
- **Live Data Feeds**: WebSocket integration for real-time crypto activity
- **Phantom Wallet Integration**: Seamless Solana blockchain transactions
- **Interactive Dashboards**: Unique monitoring interfaces for each agent type

## 🤖 Detection Agents

### Nexus - DEXScreener Alpha Scanner
- **Price**: 1.2 SOL
- **Focus**: DEXScreener trending scanner with whale tracking
- **Swarm Size**: 3 agents

### Sentinel - Pump.fun Launch Monitor
- **Price**: 2.1 SOL  
- **Focus**: Pump.fun launch monitoring and bonding curve analysis
- **Swarm Size**: 5 agents

### Cerebrix - Cross-Platform Aggregator
- **Price**: 3.8 SOL
- **Focus**: Cross-platform signal aggregation for maximum alpha discovery
- **Swarm Size**: 8 agents

### Synaptic - Social Alpha Validator
- **Price**: 1.6 SOL
- **Focus**: Community-driven alpha validation from social platforms
- **Swarm Size**: 4 agents

### Quantum - Smart Money Follower
- **Price**: 2.9 SOL
- **Focus**: Smart money following system for copy-trading
- **Swarm Size**: 7 agents

### Axon - Lightning Launch Sniper
- **Price**: 4.0 SOL
- **Focus**: Lightning-fast entry execution and launch sniping
- **Swarm Size**: 10 agents

## 🛠️ Tech Stack

### Frontend
- **React 18** with TypeScript
- **Tailwind CSS** with ShadCN/UI components
- **Wouter** for client-side routing
- **TanStack Query** for server state management
- **Framer Motion** for animations

### Backend
- **Node.js** with Express.js
- **WebSocket** integration for real-time data
- **RESTful API** design
- **In-memory storage** with abstract interface

### Blockchain
- **Solana** blockchain integration
- **Phantom Wallet** connectivity
- **SPL Token** support for CEREBRO token
- **Real-time transaction processing**

### External APIs
- **DexScreener API** for trending token data
- **Pump.fun WebSocket** for live launch monitoring
- **Solana RPC** for blockchain interactions

## 📦 Installation

1. **Clone the repository**
```bash
git clone https://github.com/cerebro-ai/cerebro-crypto-detection.git
cd cerebro-crypto-detection
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
```bash
cp .env.example .env
# Add your API keys:
# DEXSCREENER_API_KEY=your_dexscreener_key
# PUMPFUN_API_KEY=your_pumpfun_key
```

4. **Start the development server**
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## 🔧 Configuration

### Required Environment Variables

- `DEXSCREENER_API_KEY`: API key for DexScreener integration
- `PUMPFUN_API_KEY`: API key for Pump.fun data access
- `DATABASE_URL`: PostgreSQL connection string (optional, uses in-memory by default)

### Optional Environment Variables

- `OPENAI_API_KEY`: For AI-powered analysis features
- `SENDGRID_API_KEY`: For email notifications

## 🏗️ Architecture

### Project Structure
```
cerebro-crypto-detection/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Route components
│   │   ├── hooks/         # Custom React hooks
│   │   └── lib/           # Utility functions
├── server/                # Express backend
│   ├── index.ts           # Server entry point
│   ├── routes.ts          # API routes
│   ├── crypto-apis.ts     # External API integrations
│   └── storage.ts         # Data storage layer
├── shared/                # Shared TypeScript types
└── components.json        # ShadCN configuration
```

### Key Features

- **Modular Architecture**: Clean separation between frontend, backend, and shared code
- **Type Safety**: Full TypeScript implementation with shared schemas
- **Real-time Updates**: WebSocket integration for live crypto data
- **Responsive Design**: Mobile-optimized interface with dark theme
- **Scalable Storage**: Abstract storage interface supporting in-memory and PostgreSQL

## 💰 CEREBRO Token Staking

### Staking Benefits
- **70% Revenue Share**: Earn from all agent deployment fees
- **Flexible Lock Periods**: Choose 1, 7, 14, or 30-day lock periods
- **Monthly Distributions**: Automatic reward distribution
- **Governance Rights**: Participate in platform decisions

### Staking Pool Address
```
ELpPYG5zn6RSt9pJLnxPoVCkNQYx21oJ4imemoH67Jfc
```

## 🔗 API Integration

### DexScreener Integration
```typescript
// Get trending tokens
const trending = await cryptoAPI.getDexScreenerTrending(10);

// Get Solana pairs
const solana = await cryptoAPI.getDexScreenerSolana(20);
```

### Pump.fun WebSocket
```typescript
// Connect to live data stream
const ws = new WebSocket('wss://pumpportal.fun/api/data');
ws.onmessage = (event) => {
  const data = JSON.parse(event.data);
  // Process live token events
};
```

## 🚦 Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run type-check` - Run TypeScript checks

### Code Style

- **TypeScript**: Strict type checking enabled
- **ESLint**: Code linting and formatting
- **Prettier**: Consistent code formatting
- **Husky**: Pre-commit hooks for quality

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow TypeScript best practices
- Write comprehensive tests for new features
- Update documentation for API changes
- Ensure mobile responsiveness
- Test with real crypto data

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔗 Links

- **Website**: [CEREBRO Platform](https://cerebro-crypto-detection.replit.app)
- **Twitter**: [@Gammapowerai](https://x.com/Gammapowerai)
- **Support**: [Contact Form](https://cerebro-crypto-detection.replit.app/support)

## ⚠️ Disclaimer

CEREBRO is a crypto monitoring and analysis tool. All trading decisions should be made at your own risk. The platform provides information and analysis but does not constitute financial advice. Always do your own research before making investment decisions.

## 📊 Roadmap

- [ ] Additional exchange integrations (Binance, Coinbase)
- [ ] Advanced AI pattern recognition
- [ ] Mobile application
- [ ] Advanced analytics dashboard
- [ ] Community-driven agent development
- [ ] Cross-chain monitoring support

---

Built with ❤️ by the CEREBRO team | Powered by AI and real-time crypto data
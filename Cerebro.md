# CEREBRO - Crypto Detection Network Platform

## Overview

CEREBRO is a cutting-edge crypto detection platform that uses multiple AI agents to monitor and detect crypto runners on DEXScreener and Pump.fun. The platform provides real-time analysis and pattern recognition to identify suspicious trading activity and potential rug pulls. Built with modern web technologies and featuring a neural network-inspired interface focused on crypto intelligence gathering.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Styling**: Tailwind CSS with custom cyberpunk theme and ShadCN/UI components
- **Routing**: Wouter for client-side routing
- **State Management**: TanStack Query for server state management
- **Build Tool**: Vite with custom configuration

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Database**: PostgreSQL with Drizzle ORM
- **API**: RESTful API design with typed routes
- **Development**: Hot reload with Vite integration in development mode

### Database Design
The system uses a relational database with the following core entities:
- **Users**: User accounts with wallet integration
- **Detectors**: AI detection agents with crypto monitoring capabilities and deployment costs
- **Deployments**: Detection agent deployment transactions and history
- **Nodes**: Network infrastructure nodes for crypto monitoring with geographic distribution

## Key Components

### Frontend Components
- **Hero Section**: Landing page with crypto detection theme focusing on DEXScreener and Pump.fun
- **Detection Agents**: AI agent marketplace for crypto monitoring and analysis
- **Dashboard**: Real-time analytics and detection performance monitoring
- **Agent Cards**: Individual detection agent components with deployment functionality

### Backend Services
- **Storage Layer**: Abstracted storage interface with in-memory implementation
- **Route Handlers**: RESTful endpoints for users, detection agents, deployments, and nodes
- **Real-time Stats**: Dynamic statistics generation for crypto detection dashboard


## Data Flow

1. **Client Requests**: Frontend makes API calls using TanStack Query
2. **Server Processing**: Express routes handle business logic and data validation
3. **Database Operations**: Drizzle ORM manages PostgreSQL interactions
4. **Response Handling**: Typed responses sent back to client
5. **Real-time Updates**: Polling-based updates for live statistics

## External Dependencies

### Core Dependencies
- **@neondatabase/serverless**: Neon PostgreSQL database connection
- **drizzle-orm & drizzle-kit**: Type-safe database operations and migrations
- **@tanstack/react-query**: Server state management
- **wouter**: Lightweight React router

### UI Libraries
- **@radix-ui/***: Accessible component primitives
- **tailwindcss**: Utility-first CSS framework
- **lucide-react**: Icon library
- **embla-carousel-react**: Carousel component

### Development Tools
- **tsx**: TypeScript execution for development
- **esbuild**: Fast bundling for production
- **vite**: Development server and build tool

## Deployment Strategy

### Development Environment
- **Command**: `npm run dev`
- **Server**: Vite dev server with Express middleware
- **Hot Reload**: File watching with automatic recompilation
- **Port**: 5000 (configured for Replit deployment)

### Production Build
- **Build Process**: 
  1. Frontend: Vite builds static assets to `dist/public`
  2. Backend: esbuild bundles server code to `dist/index.js`
- **Start Command**: `npm start` runs the production server
- **Database**: Requires `DATABASE_URL` environment variable

### Replit Configuration
- **Modules**: Node.js 20, Web, PostgreSQL 16
- **Auto-deployment**: Configured for autoscale deployment
- **Port Mapping**: Internal port 5000 mapped to external port 80

## Changelog
  - Updated hero text from "AI AGENTS" to "CEREBRO AGENTS"
  - Modified description to focus on "DEXScreener and Pump.fun coins" instead of "anomaly detection"
  - Removed "CEREBRO AI SWARM" subtitle for cleaner design
  - Eliminated all filters from agent marketplace (search, region, tier filters)
  - Completely redesigned all 6 agents with DEXScreener and Pump.fun alpha identification focus:
    * Nexus: DEXScreener trending scanner with whale tracking
    * Sentinel: Pump.fun launch monitoring and bonding curve analysis
    * Cerebrix: Cross-platform signal aggregation for maximum alpha discovery
    * Synaptic: Community-driven alpha validation from social platforms
    * Quantum: Smart money following system for copy-trading
    * Axon: Lightning-fast entry execution and launch sniping capabilities (4.0 SOL, 10 swarm agents)
  - Removed entire "Built for Intelligence" features section from homepage for cleaner design
  - Added brain logo from CEREBRO Token page to homepage hero section for consistent branding
  - Updated header navigation to use brain logo instead of geometric symbol for unified visual identity
- January 28, 2025: Comprehensive Post-Purchase Agent Experience Implementation
  - Built complete functional agent dashboard with live monitoring capabilities at /agent/:agentId route
  - Created real-time activity feeds specific to each agent type (crypto scanning, alerts, discoveries)
  - Added dynamic statistics tracking with performance metrics and revenue generation
  - Implemented automatic redirect from purchase flow to agent dashboard for seamless user experience
  - Enhanced connection modal with "View Dashboard" button for immediate access to monitoring interface
  - Fixed routing issues: updated navigation from /marketplace to /agents throughout the application
  - Added live data streams with agent-specific crypto monitoring activities (DEXScreener, Pump.fun)
  - Integrated confidence scoring and token tracking for realistic agent performance display
  - Built comprehensive post-purchase flow that makes agents feel truly functional and operational
- January 28, 2025: Unique Agent Dashboard Specialization & Testing Pricing
  - Made each agent dashboard completely unique with specialized color themes and metrics
  - Nexus: Green/blue/yellow theme with DEXScreener whale detection focus
  - Sentinel: Cyan/orange theme with Pump.fun bonding curve analysis
  - Cerebrix: Purple/blue theme with cross-platform signal aggregation
  - Synaptic: Pink/cyan theme with social media alpha validation
  - Quantum: Emerald/teal theme with smart money copy trading
  - Axon: Red/orange theme with lightning-fast launch sniping
  - Reverted agent prices to original values: Nexus 1.2 SOL, Sentinel 2.1 SOL, Cerebrix 3.8 SOL, Synaptic 1.6 SOL, Quantum 2.9 SOL, Axon 4.0 SOL
  - Each dashboard shows agent-specific statistics, performance metrics, and specialized functionality
- January 28, 2025: Real-Time Crypto Data Integration
  - Integrated authentic DexScreener API for Nexus agent with diverse token feeds (BONK, WIF, PEPE, JUP, PYTH, ORCA, RAY, SAMO, MYRO, etc.)
  - Implemented real-time Pump.fun WebSocket integration for Sentinel agent monitoring live token launches, migrations, and trading activity
  - Enhanced activity generation with authentic crypto data replacing static mock data
  - Added live data feeds showing whale accumulation alerts, volume spikes, new token launches, and bonding curve completions
  - Both agents now provide compelling post-purchase experiences with specialized crypto monitoring capabilities
  - Successfully connected to wss://pumpportal.fun/api/data for real-time Pump.fun events and token activity streams
- January 28, 2025: CEREBRO Token Staking Reset & Configuration
  - Reset all CEREBRO token staking statistics to zero (Total Staked: 0, Total Stakers: 0, Revenue Pool: $0)
  - Platform ready for CEREBRO token launch - users can stake new token to existing infrastructure
  - Staking system maintains 50% revenue share from agent deployment fees
- January 28, 2025: Enhanced CEREBRO Token Staking Interface
  - Increased revenue share from 50% to 70% for CEREBRO token stakers (30% platform operations)
  - Added flexible lock period options: 1 day, 7 days, 14 days, and 30 days
  - Implemented Max Stake and Max Unstake buttons with custom amount options
  - Enhanced staking interface with lock period selection buttons and improved UX
  - Updated revenue distribution visualization to reflect 70% staker share

## User Preferences

Preferred communication style: Simple, everyday language.

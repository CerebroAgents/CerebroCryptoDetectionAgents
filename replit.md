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
- **World Map**: Interactive visualization of global detection network
- **Agent Cards**: Individual detection agent components with deployment functionality

### Backend Services
- **Storage Layer**: Abstracted storage interface with in-memory implementation
- **Route Handlers**: RESTful endpoints for users, detection agents, deployments, and nodes
- **Real-time Stats**: Dynamic statistics generation for crypto detection dashboard

### UI Theme
- EXTREME radiation theme with intense cyberpunk visual effects
- Deep black backgrounds with complex multi-layered radiation gradients
- Custom radiation symbol logo with animated pulsing glow effects
- Radiation green (#00ff00) primary with cyan, yellow, and red accent colors
- Wild visual effects: scanlines, matrix rain, radiation waves, quantum pulses
- Intense glow effects, text shadows, and animated borders throughout
- Multi-tier status system: Standard/Premium/Enterprise/Quantum with unique effects
- Font-mono styling for cyberpunk terminal aesthetic
- Radiation warning overlays and danger zone indicators
- Complex CSS animations: intensePulse, quantumPulse, extremeGlow, dangerPulse
- Enhanced GPU cards with detailed specifications and performance indicators

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
- June 20, 2025: Initial setup with clean professional theme
- June 20, 2025: Complete redesign with cutting-edge green radiation theme
- June 20, 2025: EXTREME radiation theme transformation - WILD visual overhaul
- June 21, 2025: Professional Matrix Theme Implementation
  - Updated color scheme to black and soft lime green (hsl(82, 100%, 55%)) professional matrix theme
  - Created floating 3D GPU component with realistic design, animated rotation, and glow effects
  - Replaced all radiation-themed terminology with professional GPU/tech language throughout
  - Fixed world map to display proper country shapes instead of blob-like outlines
  - Added infrastructure provider content: NVIDIA, AMD key providers
  - Implemented professional feature descriptions: one-click deployment, real-time monitoring, alert systems
  - Updated hero section with template library content (TensorFlow, PyTorch, Theano, CNTK, MXNet)
  - Enhanced infrastructure capabilities messaging for enterprise users
  - Maintained matrix visual effects while adopting professional terminology
- June 21, 2025: Content Updates and Map Removal
  - Removed global infrastructure map section from homepage
  - Updated template library content to "Deploy nodes in minutes" messaging
  - Added Japan and Brazil regions to marketplace dropdown filters
  - Cleaned up dashboard by removing radiation-themed elements
  - Simplified navigation by removing Network and Docs tabs
  - Enhanced messaging to focus on AI node deployment simplicity
- June 21, 2025: Gamma Token Staking Implementation
  - Added "Gamma Token" navigation item to header alongside Compute and Dashboard
  - Created comprehensive staking dashboard page with revenue sharing functionality (50% of GPU fees)
  - Implemented mobile-optimized responsive design for all staking components
  - Added staking interface with stake/unstake functionality and 30-day lock periods
  - Created user portfolio tracking with pending rewards and monthly earnings estimates
  - Integrated revenue distribution visualization showing 50% platform / 50% staker split
  - Added staking benefits including governance rights and priority GPU access
- June 21, 2025: Phantom Wallet Integration & Payment System
  - Fixed Deploy Now button functionality - resolved disabled state and click detection issues
  - Implemented 50% wallet balance fee structure for GPU deployments
  - Added comprehensive wallet balance checking before transactions
  - Integrated Phantom wallet popup for seamless SOL payments to fee collection address
  - Removed footer section from homepage for cleaner design
  - Enhanced error handling for devnet testing vs mainnet deployment scenarios
  - Successfully prepared platform for mainnet deployment with real SOL transactions
  - Integrated QuickNode RPC endpoint for reliable mainnet transaction processing
  - Added same-address transaction validation to prevent self-transfers
- June 21, 2025: Complete Support & Contact System Implementation
  - Updated X link to https://x.com/Gammapowerai for social media integration
  - Created comprehensive Support page with professional contact form at /support route
  - Implemented job application system with PDF resume upload functionality
  - Added backend API endpoints for both contact forms and job applications
  - Integrated SendGrid email service to send all submissions to careersatgamma@gmail.com
  - Built categorized support form (Technical, Billing, Deployment, Account, General)
  - Added file upload validation and error handling for smooth user experience
  - Fixed styling consistency for API-First infrastructure feature card to match other sections
- June 21, 2025: Functional Gamma Token Staking Implementation
  - Implemented real GAMMA token balance checking using Solana connection
  - Added functional staking interface with Phantom wallet integration
  - Created token transfer functionality to staking pool address
  - Built comprehensive staking dashboard with live statistics display
  - Added wallet connection requirements and balance validation
  - Integrated transaction signing and confirmation system
- June 24, 2025: Real Phantom Wallet Integration for SWARM Token Staking
  - Implemented actual Solana blockchain integration for SWARM token transfers
  - Added real token balance fetching from mainnet using @solana/spl-token
  - Created token transfer instructions to staking pool address: ELpPYG5zn6RSt9pJLnxPoVCkNQYx21oJ4imemoH67Jfc
  - Integrated Phantom wallet signing for actual blockchain transactions
  - Added real-time statistics with live revenue pool tracking
  - Built live activity feed showing recent staking transactions with timestamps
  - Fixed wallet connection with direct Phantom integration bypassing hook issues
  - Updated to mainnet RPC for production SWARM token staking with real transactions
  - Updated staking pool address to ELpPYG5zn6RSt9pJLnxPoVCkNQYx21oJ4imemoH67Jfc for production deployment
- January 28, 2025: Complete Platform Transformation to Cerebro Crypto Detection
  - Transformed entire platform from SWARM AI to crypto detection focused on DEXScreener and Pump.fun
  - Updated branding from "SWARM AI" to "CEREBRO" throughout all components with purple neural theme
  - Changed navigation to "Detectors", "Monitor", kept "GAMMA Token" for staking
  - Updated marketplace to deploy crypto detection AI agents instead of general agents
  - Maintained all existing staking and payment systems with GAMMA token (unchanged functionality)
  - Updated staking interface to show detection agent revenue sharing (50%)
  - Changed connection details to reflect crypto monitoring focus
  - Preserved exact staking metrics: 312 total stakers (+3 per visit), $10,285 revenue pool (+$36)
  - Preserved all Phantom wallet integration and blockchain functionality with GAMMA token
  - Updated hero section to focus on "Crypto Detection Network" and DEXScreener/Pump.fun monitoring
  - Modified feature descriptions to emphasize crypto runner detection and pattern analysis
  - Implemented purple neural network theme with enhanced visual effects and crypto-focused messaging
  - Updated agent pricing to one-time purchases under 4 SOL (1.2-3.8 SOL range)
  - Removed region/location filters since agents are AI-based, not physical resources
  - Added swarm agent counts (3-15 units) that scale with price and sophistication
  - Fixed all TypeScript errors and completed transformation from GPU marketplace to AI detection platform
  - Renamed "GAMMA Token" to "CEREBRO Token" with gray/black theme throughout UI
  - Updated all GPU references in Monitor/Dashboard pages to detection agent terminology
  - Removed careers section from Support page, kept contact form for agent deployment issues
  - Maintained all staking functionality and Phantom wallet integration with CEREBRO branding
  - Fixed Dashboard runtime errors by adding activeAgents stats to API and safe property access
  - Completed navigation updates: Header shows "Detectors", "Monitor", "CEREBRO Token", "Support"
  - Updated App.tsx routing to use /cerebro-token route instead of /gamma-token
  - All transformation tasks completed - platform fully operational as CEREBRO crypto detection network
- January 28, 2025: Navigation Simplification and Content Cleanup
  - Removed Monitor page completely from navigation and routing
  - Removed all careers-related content from Footer component and API endpoints
  - Renamed "Detectors" to "Agents" in main navigation
  - Simplified platform navigation to three main sections: Agents, CEREBRO Token, and Support
  - Cleaned up Footer to show only X social link and Contact link
  - Removed job application submission functionality and related SendGrid endpoints
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
  - Confirmed staking pool address: ELpPYG5zn6RSt9pJLnxPoVCkNQYx21oJ4imemoH67Jfc (same as GAMMA system)
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
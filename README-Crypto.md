# Greg Spehar's Blockchain Portfolio

## Agricultural Token Trading Platform (Prototype)

The Agricultural Token Trading Platform is a working blockchain prototype that brings institutional-style trading capabilities to agricultural finance. Built on Ethereum with a React/FastAPI architecture, it lets users trade agricultural tokens securely and shows my hands-on work in full-stack development, Web3 integration, and financial technology that connects traditional farm finance with modern blockchain infrastructure.

### 🌾 Project Overview

The **Agricultural Token Trading Platform** is a full-stack application for trading agricultural tokens on the Ethereum network. It combines modern web technologies with blockchain integration to create a secure, scalable, and easy-to-use trading environment for agricultural financial instruments.

---

### 🌾 Key Skill or Success

**Proof of concept.** I designed and built this blockchain prototype on my own to show how agricultural lending and trading could move faster, cost less, carry less risk, and still meet compliance requirements. The same thinking later shaped the Ethereum-anchored evidence in [AI Assess Tech](https://aiassesstech.com).

---

### 🏗️ Technical Architecture

#### Frontend Stack

- **Framework**: React 18+ with functional components and hooks
- **State Management**: Redux Toolkit with slice pattern architecture
- **UI Framework**: Material-UI (MUI) v5 with custom theming
- **Routing**: React Router v6 for single-page application navigation
- **API Communication**: Axios with interceptors for authentication and error handling
- **Real-time Updates**: WebSocket integration for live market data
- **Testing**: Jest and React Testing Library
- **Build Tools**: Create React App with custom configurations

#### Backend Stack

- **Framework**: FastAPI with Python 3.8+ for high-performance API development
- **Database**: PostgreSQL with SQLAlchemy ORM for data persistence
- **Authentication**: JWT-based authentication with role-based access control
- **Blockchain Integration**: Web3.py for Ethereum network interaction
- **API Documentation**: Automatic Swagger/OpenAPI documentation generation
- **Testing**: Pytest unit and integration tests
- **Async Processing**: FastAPI's native async/await support for concurrent operations

#### Blockchain Integration

- **Network**: Ethereum Sepolia testnet (designed for mainnet compatibility)
- **Token Standard**: ERC-20 compliant agricultural tokens
- **Wallet Management**: Encrypted private key handling and multi-wallet support
- **Transaction Processing**: Real-time transaction status monitoring
- **Smart Contracts**: Custom trading contract deployment and interaction
- **Gas Optimization**: Dynamic gas price calculation

---

### 🚀 Core Features

#### User Authentication & Authorization

- JWT-based authentication
- Role-based access control (Admin, Trader, Viewer)
- Password hashing and security best practices
- Session management with automatic token refresh

#### Wallet Management System

- **Multi-Wallet Support**: Create and manage multiple Ethereum wallets
- **Secure Key Storage**: Encrypted private key storage with user-specific encryption
- **Wallet Import/Export**: Import existing wallets via private key or mnemonic
- **Balance Tracking**: Real-time token and ETH balance monitoring
- **Transaction History**: Transaction logs with status tracking

#### Trading Interface

- **Order Management**: Place, modify, and cancel buy and sell orders
- **Order Book**: Real-time order book with bid/ask spreads
- **Market Data**: Live price feeds and historical chart data
- **Trade Execution**: Automated order matching and execution
- **Portfolio Tracking**: Real-time portfolio valuation and performance metrics

#### Market Data & Analytics

- **Price Charts**: Interactive candlestick and line charts
- **Volume Analysis**: Trading volume tracking
- **Market Depth**: Order book depth visualization
- **Historical Data**: Historical price and volume data
- **Technical Indicators**: Moving averages, RSI, and other indicators

#### Administrative Dashboard

- **User Management**: Admin interface for user accounts
- **System Monitoring**: Real-time system health and performance metrics
- **Transaction Oversight**: Monitor and manage platform transactions
- **Compliance Tools**: Compliance reporting features

---

## 🔐 Security Features

### Authentication Security

- JWT token-based authentication
- Password hashing with bcrypt
- Session management with automatic token refresh
- Rate limiting on authentication endpoints
- Account lockout protection against brute-force attacks

### Blockchain Security

- Encrypted private key storage
- Transaction validation and verification
- Gas limit protection against excessive fees
- Secure contract interaction patterns

### API Security

- CORS configuration for cross-origin requests
- Input validation and sanitization
- SQL injection protection through ORM usage
- Error handling that avoids leaking internal details

---

## 📊 Performance Design

### Frontend

- React component memoization
- Lazy loading for route-based code splitting
- Normalized Redux state
- Image optimization and caching

### Backend

- Async/await request handling in FastAPI
- Database query optimization with SQLAlchemy
- Connection pooling for database and blockchain connections
- Caching for frequently accessed data
- Background task processing for non-blocking operations

### Blockchain

- Batch transaction processing
- Gas price optimization
- Transaction queue management
- Block confirmation monitoring

---

## 🚀 Deployment & DevOps

- Docker containerization and Docker Compose for local development
- Environment-specific configuration management
- Automated database migrations
- Health check endpoints and structured application logging
- Architecture designed to scale horizontally for API services

---

## 🧪 Quality Assurance

- ESLint and Prettier for consistent formatting
- PropTypes type checking for React components
- Frontend tests with Jest and React Testing Library
- Backend tests with Pytest
- End-to-end testing of core user workflows

---

## 📈 Business Value

### Agricultural Finance Innovation

- Shows how blockchain could modernize agricultural token trading
- Provides a transparent trading environment for agricultural commodities
- Supports efficient price discovery and market liquidity
- Designed with compliance reporting in mind

### Technical Excellence

- Full-stack development across modern web technologies
- Blockchain integration in an enterprise-style application
- Security and performance best practices
- Architecture that can grow with future enhancements

---

## 🔮 Future Enhancements

### Planned Features

- Mobile app (React Native)
- Advanced order types (stop-loss and other conditional orders)
- Multi-factor authentication and multi-signature wallets
- Hardware wallet support
- Multi-chain support (Polygon, BSC)
- Analytics dashboard with AI insights

### Technical Roadmap

- Microservices architecture
- GraphQL API
- Formal load testing and third-party security assessment
- Machine learning for market analysis

---

## 🏆 Technical Achievements

- **Full-Stack Integration**: Frontend, backend, and blockchain working together end to end
- **Real-Time Trading**: Live order book, matching, and market data over WebSockets
- **On-Chain Settlement**: ERC-20 token trades executed and tracked on the Ethereum Sepolia testnet
- **Foundation for AI Assess Tech**: Ethereum anchoring experience that carried into AI Assess Tech's cryptographically verified evidence

*© 2026 GiDanc AI LLC. Defining the path, creating the hope, delivering the dream.*

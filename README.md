# Coffee Connoisseur Platform

A modern, full-stack web application built with microservices architecture for coffee enthusiasts to manage collections, track tasting experiences, and discover new coffees through AI-powered recommendations and real-time community features.

## 🚧 Status: In Active Development

Currently implementing Phase 1 (Foundation & Core Backend) - Building TypeScript microservices with authentication and core APIs. This project represents a comprehensive learning journey through modern web development technologies and practices.

## 🛠️ Tech Stack

**Backend Microservices:**
- Node.js 20+ with TypeScript 5+
- Express.js with comprehensive middleware
- Prisma ORM with PostgreSQL 15+
- Redis for caching and sessions
- OpenAI API + LangChain for AI features

**Frontend:**
- Next.js 14+ with App Router
- TypeScript with strict mode
- Tailwind CSS + shadcn/ui
- Zustand + React Query (TanStack)
- Socket.io for real-time features

**DevOps & Infrastructure:**
- Docker with multi-stage builds
- Kubernetes on AWS EKS
- GitHub Actions CI/CD
- Prometheus + Grafana monitoring
- AWS (RDS, ElastiCache, S3, CloudFront)

## ✨ Key Features (In Development)

### Core Features
- 🔐 **Secure Authentication** - JWT with refresh token rotation
- ☕ **Advanced Coffee Catalog** - Comprehensive search and filtering
- 📝 **Personal Collection Management** - Inventory tracking with analytics
- 📊 **Detailed Tasting Notes** - Multi-dimensional rating system
- 📈 **Personal Analytics** - Coffee consumption insights and trends

### AI-Powered Features
- 🤖 **Intelligent Recommendations** - Personalized coffee suggestions with explanations
- 📸 **Image Recognition** - Coffee bean and grind assessment using computer vision
- 💬 **Brewing Assistant** - Real-time conversational guidance with LangChain
- 🧠 **Smart Analysis** - Natural language processing of tasting notes

### Social & Real-time Features
- 👥 **Community Platform** - Follow users, share reviews, discuss coffee
- ⚡ **Real-time Interactions** - Live brewing sessions, instant notifications
- 🗨️ **Live Chat** - Community discussions and brewing assistance
- 🏆 **Community Challenges** - Engaging events and leaderboards

### Advanced Capabilities
- 📱 **Progressive Web App** - Offline functionality and mobile optimization
- 🌐 **GraphQL API** - Efficient data fetching for complex relationships
- 🔍 **Advanced Search** - Full-text search with intelligent filtering
- 📦 **Microservices Architecture** - Scalable, maintainable service design

## 🚀 Getting Started

### Prerequisites
- Node.js 20+
- Docker & Docker Compose
- PostgreSQL 15+
- Redis 7+
- OpenAI API Key

### Quick Start with Docker

```bash
# Clone the repository
git clone https://github.com/yourusername/coffee-connoisseur-platform.git
cd coffee-connoisseur-platform

# Start all services with Docker Compose
docker-compose up -d

# The application will be available at:
# Frontend: http://localhost:3000
# API: http://localhost:3001
# AI Service: http://localhost:3002
```

### Local Development Setup

```bash
# Install dependencies for all workspaces
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Start databases
docker-compose up postgres redis -d

# Run database migrations
npm run db:migrate

# Seed development data
npm run db:seed

# Start all services in development mode
npm run dev

# Or start services individually
npm run dev:api      # Backend API service
npm run dev:web      # Next.js frontend
npm run dev:ai       # AI microservice
```

## 📁 Project Structure

```
coffee-connoisseur-platform/
├── apps/
│   ├── api/                 # Express + TypeScript API service
│   │   ├── src/
│   │   │   ├── controllers/ # Route handlers
│   │   │   ├── services/    # Business logic
│   │   │   ├── middleware/  # Custom middleware
│   │   │   └── types/       # TypeScript type definitions
│   │   └── Dockerfile
│   ├── web/                 # Next.js frontend application
│   │   ├── app/             # App Router structure
│   │   ├── components/      # Reusable UI components
│   │   ├── hooks/           # Custom React hooks
│   │   └── lib/             # Utility functions
│   └── ai-service/          # Dedicated AI microservice
│       ├── src/
│       │   ├── services/    # AI service implementations
│       │   ├── models/      # AI model configurations
│       │   └── utils/       # AI utility functions
│       └── Dockerfile
├── packages/
│   ├── database/            # Prisma schema & migrations
│   │   ├── prisma/
│   │   ├── migrations/
│   │   └── seed.ts
│   ├── types/               # Shared TypeScript types
│   └── config/              # Shared configuration
├── k8s/                     # Kubernetes deployment configs
├── .github/workflows/       # GitHub Actions CI/CD
├── docker-compose.yml       # Local development setup
└── README.md
```

## 🎯 Development Roadmap

### Phase 1: Foundation
- ✅ Project setup with TypeScript monorepo
- ✅ Database design and Prisma configuration  
- 🔄 Authentication service with JWT
- 🔄 Coffee catalog APIs with search
- ⏳ Collection management system

### Phase 2: Frontend Foundation
- ⏳ Next.js setup with TypeScript
- ⏳ Authentication flow and protected routes
- ⏳ Coffee browsing and collection UI
- ⏳ Tasting notes system

### Phase 3: AI Integration
- ⏳ AI microservice with OpenAI integration
- ⏳ Recommendation engine
- ⏳ Image recognition for coffee assessment
- ⏳ Conversational brewing assistant

### Phase 4: Social Features
- ⏳ Real-time social platform
- ⏳ Community features and moderation
- ⏳ WebSocket implementation for live features

### Phase 5: Production Deployment
- ⏳ Kubernetes deployment on AWS
- ⏳ CI/CD pipeline with GitHub Actions
- ⏳ Monitoring and observability
- ⏳ Production optimization

## 🧪 Testing

```bash
# Run all tests
npm run test

# Run tests for specific services
npm run test:api          # Backend API tests
npm run test:web          # Frontend component tests
npm run test:ai           # AI service tests
npm run test:e2e          # End-to-end tests

# Run tests in watch mode during development
npm run test:watch
```

## 📚 API Documentation

- **Interactive API Docs**: http://localhost:3001/docs (Swagger UI)
- **GraphQL Playground**: http://localhost:3001/graphql
- **API Schema**: Auto-generated OpenAPI 3.0 specification

## 🔧 Development Tools

- **Code Quality**: ESLint + Prettier + Husky pre-commit hooks
- **Type Safety**: Strict TypeScript configuration across all services
- **Database**: Prisma Studio for database management
- **Monitoring**: Development monitoring dashboard
- **Documentation**: Auto-generated API documentation

## 🌟 Learning Objectives

This project is designed as a comprehensive learning experience covering:

- **Modern Backend Development**: TypeScript, Node.js, microservices architecture
- **Advanced Frontend**: Next.js 14, Server Components, modern React patterns
- **AI Integration**: OpenAI API, LangChain, intelligent user experiences
- **Real-time Features**: WebSocket implementation, live user interactions
- **DevOps Practices**: Docker, Kubernetes, CI/CD, monitoring
- **Database Design**: Complex relationships, optimization, migration strategies
- **Security**: Authentication, authorization, data protection
- **Testing**: Unit, integration, and end-to-end testing strategies
- **Performance**: Optimization techniques, caching, scalability

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details

## 🤝 Contributing

This is primarily a personal learning project, but feedback and suggestions are welcome! Feel free to:
- Open issues for bugs or feature suggestions
- Submit pull requests for improvements
- Share feedback on architecture and implementation

## 📬 Contact

- **Developer**: James Gonzalez
- **Email**: jamesg8025@gmail.com
- **LinkedIn**: http://linkedin/in/gonzalez-james
- **Portfolio**: http://jamesg8025.github.io

---

*Built as a comprehensive full-stack development learning project, showcasing modern web technologies, AI integration, and production-ready practices.*
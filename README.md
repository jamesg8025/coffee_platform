# coffee_platform
A coffee connoisseur platform!

# Coffee Connoisseur Platform

A full-stack web application for coffee enthusiasts to manage collections, track tasting experiences, and discover new coffees through AI-powered recommendations.

## 🚧 Status: In Development

Currently implementing Phase 1 (MVP Foundation) - Core functionality with user management and coffee catalog.

## 🛠️ Tech Stack

**Backend:**
- Java Spring Boot 3.x
- Spring Data JPA
- Spring Security (JWT)
- PostgreSQL
- OpenAI API Integration

**Frontend:**
- React 18+
- Tailwind CSS
- Axios

**DevOps:**
- Docker
- AWS (EC2, RDS, S3)
- GitHub Actions CI/CD

## ✨ Key Features (Planned)

- 📝 Personal coffee collection management
- ☕ Detailed tasting notes with flavor profiles
- 🤖 AI-powered coffee recommendations
- 📸 Coffee image recognition and analysis
- 👥 Social features and community reviews
- 📊 Analytics and brewing insights

## 🚀 Getting Started

### Prerequisites
- Java 17+
- Node.js 18+
- PostgreSQL 15+
- Docker

### Local Development Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/coffee-connoisseur-platform.git
cd coffee-connoisseur-platform

# Backend setup
cd backend
./mvnw spring-boot:run

# Frontend setup
cd ../frontend
npm install
npm start
```

### Docker Development Setup

```bash
# Run with Docker Compose
docker-compose up -d
```

## 📁 Project Structure

```
coffee-connoisseur-platform/
├── backend/                 # Spring Boot application
├── frontend/               # React application
├── docker-compose.yml      # Local development setup
├── docs/                   # Documentation
└── README.md
```

## 🗺️ Development Roadmap

- **Phase 1** (Current): MVP Foundation - User management, coffee catalog
- **Phase 2**: Personal features, basic AI integration
- **Phase 3**: Community features, advanced AI
- **Phase 4**: Advanced features & polish
- **Phase 5**: Production deployment

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details

## 🤝 Contributing

This is a personal learning project, but feedback and suggestions are welcome!

---

*Built as part of a full-stack development learning journey, showcasing modern web technologies and AI integration.*

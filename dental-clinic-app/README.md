# Clinic Pulse — Monorepo Architecture

> **Live Demo:** [https://dentist-management-system-psi.vercel.app](https://dentist-management-system-psi.vercel.app)  
> For the complete documentation, screenshots, and feature breakdown, see the [Root README](../README.md).

---

## Workspace Structure

- **[`backend/`](backend/)** — Node.js 20+ Express API, Prisma 5 ORM, PostgreSQL, JWT Authentication.
- **[`frontend/`](frontend/)** — React 18, Vite 5, TypeScript, Tailwind CSS, TanStack Query 5.
- **[`docs/`](docs/)** — System architecture, database schema, API documentation, and setup guides.

## Running Locally

### Option 1: Docker Compose (Full Stack)
```bash
docker-compose up --build
```
- Frontend: `http://localhost:3000`
- Backend API: `http://localhost:4000` (Health: `http://localhost:4000/health`)
- Seed demo data: `docker-compose exec backend node dist/prisma/seed.js`

### Option 2: Standalone Dev Mode
```bash
# Backend
cd backend && npm install && npm run dev

# Frontend
cd ../frontend && npm install && npm run dev
```

See [`docs/setup.md`](docs/setup.md) for detailed environment setup.

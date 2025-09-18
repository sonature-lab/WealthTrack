# WealthTrack

WealthTrack is a **personal finance and wealth management web application** built with a clean and scalable architecture.  
It enables users to manage daily budgets, upload e-Statements for automatic transaction parsing, visualize investment portfolios, and simulate potential returns with market data integration.

The project demonstrates **full-stack architecture design**, combining **Next.js (frontend)** with **Kotlin + Spring Boot (backend)**, and adheres to **OOP and Clean Architecture principles** throughout.

---

## ✨ Features

- 📊 **Budget Tracking** – Manage income/expenses with automatic categorisation
- 📂 **e-Statement Upload** – Parse bank statements (CSV/PDF) into structured transactions
- 📈 **Portfolio Visualisation** – Interactive charts (Recharts) for investment performance
- 🔮 **Forecasting (Planned)** – AI-powered financial prediction engine
- 🔐 **Authentication & User Management** (basic)

---

## 🏛️ Architecture Overview

WealthTrack/
├─ frontend/ # Next.js + React + TypeScript (FSD + OOP)
│ ├─ app/ # Global providers, layout
│ ├─ pages/ # Routes
│ ├─ entities/ # Domain models (Transaction, Portfolio, User)
│ ├─ features/ # Use-cases (Upload Statement, Portfolio Visualisation, Budget Tracker)
│ └─ shared/ # UI components, utils, API client
│
├─ backend/ # Kotlin + Spring Boot (Clean Architecture)
│ ├─ application/ # Use Cases, Services
│ ├─ domain/ # Entities, Value Objects, Interfaces
│ ├─ infrastructure/ # Persistence (JPA), External APIs, Parsers
│ └─ presentation/ # REST Controllers
│
├─ docs/ # Documentation (ERD, diagrams)
└─ docker-compose.yml (dev only)

- **Frontend**: FSD (Feature-Sliced Design) with OOP-style entities and hooks
- **Backend**: Clean Architecture (Domain → Application → Infrastructure → Presentation)
- **Deployment**: Dockerized services, CI/CD with GitHub Actions → AWS Lightsail

---

## 🛠️ Tech Stack

### Frontend

- **React 18 + Next.js 14** (TypeScript)
- Feature-Sliced Design (FSD) architecture
- Recharts, TailwindCSS
- Axios (API client)

### Backend

- **Kotlin + Spring Boot 3**
- Clean Architecture (OOP, SOLID)
- JPA (Hibernate) + PostgreSQL
- Gradle Kotlin DSL

### Infrastructure

- Docker & docker-compose (local dev)
- GitHub Actions (CI/CD pipeline)
- AWS Lightsail (deployment target)

---

## 🚀 Getting Started

### 1. Clone Repository

```bash
git clone https://github.com/sonature-lab/WealthTrack.git
cd WealthTrack
```

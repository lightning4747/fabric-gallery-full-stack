# Fabric-Gallery-full-stack

A comprehensive, production-grade web application for managing fabric collections, orders, and user interactions. This project features a modern, responsive React frontend and a powerful Node.js/TypeScript backend with multi-database support.

## Project Structure

- **`/frontend`**: React + TypeScript + Vite application with a custom design system.
- **`/backend`**: Node.js + Express + TypeScript server using PostgreSQL and MongoDB.

## Getting Started

### Prerequisites
- Node.js (v20+)
- PostgreSQL (v15+)
- MongoDB (v6+)
- npm or yarn

### Quick Start (Docker)
The entire stack can be launched using Docker Compose from the backend directory:
```bash
cd backend
docker-compose up --build
```

### Manual Setup

#### 1. Backend Setup
1. Navigate to the backend directory: `cd backend`
2. Install dependencies: `npm install`
3. Configure environment: Create a `.env` file based on the schema in `src/config/env.ts`.
4. Initialize database: `npm run seed`
5. Start server: `npm run dev` (Runs on `http://localhost:3000`)

#### 2. Frontend Setup
1. Navigate to the frontend directory: `cd frontend`
2. Install dependencies: `npm install`
3. Start development server: `npm run dev`
4. Access the app at `http://localhost:5173` (ensure backend is running)

## Application Walkthrough

1. **Authentication**: Users can register as a Customer, Manager, or Admin. Roles determine available features and navigation visibility.
2. **Catalog Exploration**: Browse the fabric collection, filter by categories, and view detailed specifications using interactive cards.
3. **Shopping Experience**: Add fabrics to the Wishlist or Cart, manage quantities, and proceed to checkout.
4. **Order Management**: Track personal orders, while Administrators and Managers can fulfill and manage all system orders.
5. **Administration**:
   - **Dashboard**: Real-time activity monitoring and system statistics.
   - **User Management**: Control user access, roles, and permissions.
   - **Master Data**: Manage fabric specifications (Sprefs), categories, and global settings.
   - **System Logs**: Audit trail for critical system actions and administrative changes.


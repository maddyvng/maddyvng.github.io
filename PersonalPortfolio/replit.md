# Portfolio Application

## Overview

This is a modern full-stack portfolio website built with React, TypeScript, and Express.js. The application showcases a creative developer's work with sections for projects, about information, and contact details. It features a clean, responsive design using Tailwind CSS and shadcn/ui components with a cyan and beige color scheme.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Routing**: Wouter for client-side routing
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **UI Components**: shadcn/ui component library with Radix UI primitives
- **Animations**: Framer Motion for smooth animations and transitions
- **State Management**: TanStack React Query for server state management
- **Build Tool**: Vite for fast development and optimized builds

### Backend Architecture
- **Runtime**: Node.js with TypeScript
- **Framework**: Express.js for REST API endpoints
- **Database**: PostgreSQL with Drizzle ORM
- **Database Provider**: Neon Database (@neondatabase/serverless)
- **Session Management**: connect-pg-simple for PostgreSQL session storage
- **Development**: Hot reload with Vite integration

### Data Storage Solutions
- **Primary Database**: PostgreSQL via Neon Database
- **ORM**: Drizzle ORM with TypeScript-first schema definitions
- **Schema Management**: Drizzle Kit for migrations and schema management
- **In-Memory Storage**: Fallback MemStorage implementation for development

## Key Components

### Frontend Components
1. **Navigation**: Fixed header with smooth scroll navigation
2. **Hero Section**: Landing area with call-to-action buttons
3. **Projects Section**: Grid layout showcasing featured and regular projects
4. **About Section**: Skills showcase with animated icons
5. **Contact Section**: Contact information with social links
6. **Project Cards**: Reusable components with hover animations

### Backend Components
1. **Routes Handler**: Centralized route registration system
2. **Storage Interface**: Abstracted storage layer with CRUD operations
3. **User Management**: Basic user schema with authentication ready structure
4. **Development Server**: Vite integration for hot reloading

### UI System
- **Design System**: Consistent spacing, colors, and typography
- **Theme Support**: CSS custom properties for light/dark mode capability
- **Responsive Design**: Mobile-first approach with breakpoint management
- **Component Library**: Comprehensive set of reusable UI components

## Data Flow

1. **Client Requests**: React components make API calls through TanStack Query
2. **Server Processing**: Express.js routes handle requests and interact with storage
3. **Database Operations**: Drizzle ORM manages PostgreSQL interactions
4. **Response Handling**: Data flows back through the storage interface to client
5. **State Management**: React Query handles caching and synchronization

## External Dependencies

### Core Dependencies
- **@neondatabase/serverless**: Serverless PostgreSQL connection
- **drizzle-orm**: TypeScript ORM for database operations
- **@tanstack/react-query**: Server state management
- **framer-motion**: Animation library
- **wouter**: Lightweight React router

### UI Dependencies
- **@radix-ui/***: Headless UI components
- **tailwindcss**: Utility-first CSS framework
- **class-variance-authority**: Type-safe variant API
- **lucide-react**: Icon library

### Development Dependencies
- **vite**: Build tool and development server
- **typescript**: Type checking and compilation
- **tsx**: TypeScript execution for Node.js

## Deployment Strategy

### Build Process
1. **Frontend Build**: Vite compiles React app to `dist/public`
2. **Backend Build**: esbuild bundles server code to `dist/index.js`
3. **Database Setup**: Drizzle migrations applied via `db:push` command

### Environment Configuration
- **Development**: Uses tsx for hot reloading and Vite dev server
- **Production**: Serves static files from Express with compiled assets
- **Database**: Requires `DATABASE_URL` environment variable

### Scripts
- `dev`: Development server with hot reload
- `build`: Production build for both frontend and backend
- `start`: Production server startup
- `check`: TypeScript type checking
- `db:push`: Database schema synchronization

## Changelog

```
Changelog:
- June 30, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```
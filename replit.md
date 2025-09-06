# Starry Events

## Overview

Starry Events is a modern single-page web application for a Discord server that hosts Roblox gaming events with Robux prizes. The application provides a sleek, aesthetic interface where users can view ongoing and scheduled gaming events, authenticate with Discord OAuth, and participate in community activities. Built with React, TypeScript, and a full-stack architecture using Express.js, the platform offers real-time event management and user interaction capabilities.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and modern development
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack React Query for server state management and caching
- **UI Components**: shadcn/ui component library built on Radix UI primitives
- **Styling**: Tailwind CSS with custom design system featuring dark theme, gradients, and modern aesthetics
- **Build Tool**: Vite for fast development and optimized production builds

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules for modern JavaScript features
- **API Pattern**: RESTful API structure with /api prefix routing
- **Development**: Hot module replacement via Vite integration in development mode
- **Storage Interface**: Abstracted storage layer supporting both in-memory and database implementations

### Data Storage Solutions
- **Database**: PostgreSQL configured via Drizzle ORM
- **ORM**: Drizzle with type-safe schema definitions and migrations
- **Connection**: Neon Database serverless driver for PostgreSQL connectivity
- **Schema Management**: Centralized schema definitions in shared directory for type consistency
- **Development Storage**: In-memory storage implementation for rapid prototyping

### Authentication and Authorization
- **OAuth Provider**: Discord OAuth 2.0 integration for user authentication
- **Session Management**: Express sessions with PostgreSQL session store
- **User Data**: Discord profile integration (username, avatar, user ID)
- **Security**: Secure cookie configuration and CSRF protection measures

### External Dependencies
- **Discord API**: OAuth 2.0 authentication and user profile data retrieval
- **Roblox Integration**: External game links for event participation
- **Font Services**: Google Fonts (Inter, Architects Daughter, DM Sans, Fira Code, Geist Mono)
- **Icon Library**: Font Awesome for consistent iconography
- **Database Hosting**: Neon Database for managed PostgreSQL services
- **Development Tools**: Replit-specific plugins for development environment integration

### Component Architecture
- **Design System**: Custom Tailwind configuration with CSS variables for theming
- **UI Components**: Modular component library with consistent styling patterns
- **Event Management**: Specialized components for event cards, countdowns, and user interactions
- **Responsive Design**: Mobile-first approach with adaptive layouts
- **Animation System**: CSS transitions and hover effects for enhanced user experience

### Development Workflow
- **Type Safety**: Full TypeScript integration across frontend, backend, and shared code
- **Code Organization**: Monorepo structure with clear separation between client, server, and shared code
- **Build Process**: Optimized bundling for both client and server applications
- **Development Server**: Integrated Vite dev server with Express.js middleware
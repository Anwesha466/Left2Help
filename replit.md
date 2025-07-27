# Left2Help - Smart Leftover Ingredient Exchange

## Overview

Left2Help is a full-stack Progressive Web Application (PWA) that enables local food vendors to exchange leftover ingredients and communicate in real-time. The platform combines an ingredient marketplace with a comprehensive chat system to reduce food waste and build stronger community connections among vendors.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript and Vite
- **UI Library**: Shadcn/ui components built on Radix UI primitives
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **State Management**: TanStack Query (React Query) for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Form Handling**: React Hook Form with Zod validation
- **Real-time Communication**: WebSocket integration for live messaging

### Backend Architecture
- **Runtime**: Node.js with Express.js
- **Language**: TypeScript with ES modules
- **Database ORM**: Drizzle ORM with PostgreSQL dialect
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **WebSocket**: Native WebSocket Server for real-time messaging
- **Session Management**: PostgreSQL-backed sessions with connect-pg-simple

### Progressive Web App Features
- Service worker registration for offline capabilities
- App manifest for installation on mobile devices
- Responsive design optimized for mobile-first experience
- Location-based services with geolocation API integration

## Key Components

### Ingredient Exchange System
- Vendors can post leftover ingredients with details (quantity, expiry, pricing, location)
- Category-based filtering (vegetables, fruits, grains, spices, dairy, meat)
- Location-based search with distance filtering (1-5km radius)
- Real-time ingredient availability updates

### Real-time Chat System
- One-to-one messaging between vendors
- WebSocket-powered live messaging with delivery status
- Message history with thread-like conversation view
- Typing indicators and online status tracking
- Chat history management with clear conversation options

### User Management
- Vendor profiles with stall information and location
- Trust score system based on vendor behavior
- Activity tracking (total posts, money saved, connections)
- Online/offline status with last seen timestamps

### Call Log System
- Audio/video call history tracking
- Call duration and timestamp logging
- Participant identification and call direction
- History management with deletion capabilities

## Data Flow

### Database Schema
- **Users**: Vendor profiles with location, trust scores, and activity metrics
- **Ingredients**: Posted items with vendor relationships and location data
- **Conversations**: One-to-one chat relationships between vendors
- **Messages**: Chat messages with sender information and timestamps
- **Call Logs**: Communication history with metadata

### API Architecture
- RESTful endpoints for CRUD operations on ingredients, users, and conversations
- WebSocket endpoints for real-time messaging and status updates
- Session-based authentication with PostgreSQL storage
- Location-based filtering with latitude/longitude calculations

### Real-time Features
- WebSocket connections maintain user presence and messaging state
- Live ingredient updates when new items are posted nearby
- Instant message delivery with connection management
- Real-time typing indicators and read receipts

## External Dependencies

### Core Technologies
- **Database**: Neon Database (serverless PostgreSQL)
- **UI Components**: Radix UI primitives for accessibility
- **Styling**: Tailwind CSS for utility-first styling
- **Icons**: Lucide React for consistent iconography
- **Date Handling**: date-fns for timestamp formatting

### Development Tools
- **Build System**: Vite with React plugin and TypeScript support
- **Database Migration**: Drizzle Kit for schema management
- **Code Quality**: TypeScript strict mode with comprehensive type checking
- **Development Experience**: Hot module replacement and error overlay

### Mobile Optimization
- Touch-friendly interface with gesture support
- Viewport optimization for various screen sizes
- Native app-like experience with PWA capabilities
- Offline functionality with service worker caching

## Deployment Strategy

### Build Process
- Frontend built with Vite to static assets
- Backend bundled with esbuild for Node.js production
- TypeScript compilation with strict type checking
- Asset optimization and code splitting

### Environment Configuration
- Database URL configuration via environment variables
- Development and production environment separation
- Replit-specific optimizations for cloud development
- Mobile-responsive design testing across devices

### Scalability Considerations
- Stateless backend design for horizontal scaling
- Database connection pooling with Neon serverless
- WebSocket connection management for concurrent users
- Efficient location-based queries with geographic indexing

The application is designed as a community-focused platform that prioritizes real-time communication, location awareness, and mobile accessibility to serve the specific needs of local food vendors in reducing waste and building business relationships.
# Connectly Backend API

**Scalable Laravel 10 REST API** built to power modern React frontends.

Developed as Founding Developer during the early MVP stage of a social + events + fintech platform. This backend was designed from day one with **frontend consumption in mind**, enabling seamless integration with React and Next.js applications.

---

## Overview

This project showcases my ability to build clean, well-structured backend systems that prioritize **frontend performance and developer experience**.

Although I am no longer actively involved in the project, it remains a strong demonstration of my full-stack understanding — particularly how a solid API foundation directly impacts the quality, speed, and maintainability of the frontend.

**Current focus:** I am deepening my expertise in **Frontend Development**, with special interest in building performant, intuitive, and visually appealing user interfaces using React and Tailwind CSS.

---

## Why This Backend Matters for My Frontend Journey

By designing and building this API myself, I gained deep insight into:
- How backend architecture affects frontend rendering performance
- Designing predictable and efficient JSON structures for React components
- Creating authentication flows optimized for SPAs
- Reducing over-fetching and improving data loading patterns

This experience helps me build better React applications today, as I understand both sides of the stack.

---

## Key Features

- **Authentication**: Laravel Sanctum with token-based auth optimized for React SPAs
- **Social Engine**: Posts, comments, likes, follows, and real-time ready structures
- **Event & Ticketing System**: Complete flow from event creation to ticket management
- **Basic Fintech**: Transactional logic for payments and inventory control
- **Media Handling**: Polymorphic relationships for flexible attachment management
- **Optimized Endpoints**: Designed specifically for efficient frontend consumption

---

## Frontend-Focused Design Decisions

- Consistent and predictable JSON responses tailored for React state management
- Reduced over-fetching through focused, purpose-built endpoints
- Clean separation between data layer and presentation layer
- Authentication flow designed for single-page applications
- Support for efficient data fetching patterns (ideal for React Query / TanStack Query)
- CORS properly configured for frontend clients

---

## Architecture Highlights

- **Service Pattern**: Business logic cleanly separated from controllers (thin controllers)
- **API-First Approach**: Built specifically to be consumed by modern frontend frameworks
- **Modular & Scalable Structure**: Easy to maintain and extend
- **Query Optimization**: Eager Loading implemented to prevent N+1 problems in feeds and complex views

---

## Database Design

Relational database with **~25 normalized tables** (3NF) ensuring data integrity and scalability.

**Main Entities:**
- Users & Profiles
- Posts, Comments, Likes & Hashtags
- Events, Tickets & Orders
- Wallets & Transactions

**Key Decisions:**
- Full normalization to maintain consistency
- Polymorphic relationships for media
- Transaction-safe operations for payments and ticket inventory

---

## Tech Stack

**Backend**  
- Laravel 10  
- PHP 8.1+  
- MySQL / PostgreSQL  
- Laravel Sanctum  

**Frontend Integration**  
- Vite + Tailwind CSS (configured)  
- REST API optimized for React / Next.js  

**Additional Tools**  
- Redis (caching ready)  
- Swagger / OpenAPI (documentation)

---

## Related Frontend Projects

Check my recent React work where I apply the lessons learned from this backend:

- **[crud-react](https://github.com/MarxWellB/crud-react)** — React + Vite + Tailwind + JWT Authentication + CRUD
- **[clima-news](https://github.com/MarxWellB/clima-news)** — React dashboard consuming external APIs

---

## Quick Start

```bash
git clone https://github.com/MarxWellB/red-social.git
cd red-social

composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed

php artisan serve

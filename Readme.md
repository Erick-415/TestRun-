# Fitness App (Client + Coach)

A lightweight coaching platform with **two views**:
- **Client**: onboarding form → dashboard/calendar → workout plan + tracking → nutrition plan + tracking → check-ins (text/video) → metrics
- **Coach**: client info sheet → template dashboard → program phases (wk1–wk4) → personalized workout + nutrition recommendations

This repo is a monorepo:
- `apps/web`: React (Vite) frontend
- `apps/api`: Node/Express backend API
- `packages/shared`: shared TypeScript types + validation schemas
- `docs/`: architecture + API + DB notes

## Features (MVP)
Based on project whiteboards:
- Accounts: register/login, delete account
- Client onboarding form (goals, restrictions/injuries, routine, motivation, baseline metrics)
- Coach-managed program phases (wk1–wk4):
  - wk1: track food + workout habit
  - wk2: track protein + progressive workouts
  - wk3: track calories + workouts++
  - wk4: mindful of calories (sustainability)
- Workout plan + tracking
- Nutrition plan + tracking
- Check-ins (text/video) - MVP starts as text notes + optional upload links
- Metrics: weight, progress pictures, workout baseline, steps/cardio sessions (optional), smart watch integration (future)

## Tech Stack
### Frontend (`apps/web`)
- React + Vite + TypeScript
- react-router-dom (routing)
- @tanstack/react-query + axios (API calls + caching)
- react-hook-form + zod (forms + validation)
- Tailwind CSS (styling)

### Backend (`apps/api`)
- Node.js + Express + TypeScript
- Prisma ORM
- PostgreSQL
- JWT auth (jsonwebtoken) + password hashing (bcrypt)

### Shared (`packages/shared`)
- TypeScript types + Zod schemas shared between web/api

## Repo Layout
fitness-app/
apps/
web/ # React frontend
api/ # Express backend
packages/
shared/ # shared types/schemas
docs/ # design + API + DB notes


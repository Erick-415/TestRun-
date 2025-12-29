# Architecture Decisions

## Two-view product model
We support two primary roles:
- Client: onboarding + tracking + metrics
- Coach: client overview + program templates + personalization

## Stack choices
- Web: React (Vite) for fast iteration and simple deployment
- API: Express for explicit request/response flow and clearer backend learning
- DB: Postgres for relational data (users → logs/workouts/metrics)
- ORM: Prisma for migrations + typed DB access

## MVP scope boundaries
In MVP:
- Check-ins are text-based with optional links (video upload can be added later)
- Smartwatch integration is out-of-scope (future)
- Gamification is optional (future)

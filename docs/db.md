# Database (Draft)

## Core entities
- users
- workouts
- nutrition_logs
- metrics_weight
- coach_client (relationship mapping coach ↔ client)

## Relationship sketch
- users 1—many workouts
- users 1—many nutrition_logs
- users 1—many metrics_weight
- coach_client maps coachId → clientId

# BitZit Software House Portal

## Features
- Multi-role: IT Expert, Company, Admin
- Credits, campus eligibility, equity tracking
- Dashboards with charts
- JWT auth with role-based routing
- i18n-ready with language toggle
- Tailwind UI and Next.js app router

## Tech Stack
- Next.js 14, React
- Prisma ORM with SQLite (dev)
- Tailwind CSS
- Chart.js via react-chartjs-2

## Local Setup
1. Copy `.env.example` to `.env` and adjust values.
2. Install dependencies: `npm install`
3. Generate client: `npm run prepare`
4. Migrate DB: `npx prisma migrate dev --name init`
5. Run dev server: `npm run dev`

## Deployment (Vercel)
1. Push repository to GitHub.
2. Create a new Vercel project, import the repo.
3. Set Environment Variables:
   - `DATABASE_URL` (use a hosted PostgreSQL for production or `file:./dev.db` for demo)
   - `JWT_SECRET`
4. Deploy. Next.js auto-detects and builds.

## Roles
- IT Expert: `/expert`
- Company: `/company`
- Admin: `/admin`

## Notes
- Documents and uploads use text placeholders initially.
- Analytics widgets show basic counts and country distribution.

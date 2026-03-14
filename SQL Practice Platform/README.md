# SQL Practice Platform

## Summary
A full-stack web application for creating, scheduling, and taking SQL practice tests. Built for educators and students: admins create practice sets (with **AI-generated questions** via OpenAI), assign tests, and auto-review submissions; students take tests with a **SQL Runner** mode and see schema once at the top. Uses Next.js, TypeScript, Prisma, and PostgreSQL (Supabase), with optional deployment to Railway or Azure.

---

## 🚨 Problem → 💡 Solution → 📈 Impact

### Problem
Instructors needed a way to deliver domain-specific SQL practice (e.g. Banking schema) with consistent schema, auto-grading, and flexible question authoring without manually writing dozens of questions.

### Solution
- **Admin**: Create practice sets by domain (Banking, Retail, ERP, Travel, Telecom), difficulty, and focus areas (aggregates, JOINs, etc.); **AI-generated questions** using OpenAI against a defined schema (e.g. `BankingDbScript.sql`).
- **Schema-once UX**: Database schema displayed once at the top of each test instead of per question.
- **Student experience**: Take assigned tests, answer via text or **SQL Runner** (execute against DB, see results), auto-save, submit for review.
- **Auto-review**: Compare student answers to model answers; release results to students.

### Impact
- 🤖 AI reduces time to create practice sets while keeping schema consistency (e.g. Banking).
- 📊 Teachers get a single place to schedule tests, review submissions, and release answers.
- 🎯 Students practice real SQL with live execution and clear schema reference.
- ☁️ Runs on Supabase + Vercel/Railway/Azure for scalable, low-friction deployment.

---

## 🛠️ Technology Stack

| Component     | Technology                          |
|--------------|-------------------------------------|
| Frontend     | Next.js 16, React 19, TypeScript, Tailwind CSS |
| Backend      | Next.js API Routes                  |
| Database     | PostgreSQL (Supabase), Prisma ORM   |
| Auth         | Cookie-based session                |
| AI           | OpenAI API (question generation)    |
| Deployment   | Vercel, Railway, or Azure App Service |

---

## 🔗 Links

| Resource | URL |
|----------|-----|
| **GitHub** | [CSkarki/sql-practice-platform](https://github.com/CSkarki/sql-practice-platform) |
| **Live**   | [SQL Practice Platform (Vercel)](https://sql-practice-platform.vercel.app) |

# Utsav-Events.com (Invite & RSVP App)

## Summary
**Utsav-Events.com** is an Evite-style invite and RSVP application for events and parties. Guests receive a single link, submit RSVPs (name, email, attending, message), and the host can view and download responses from a protected dashboard. Supports local JSON storage for dev or Supabase (Postgres) in production. Demonstrates practical full-stack delivery with Next.js and modern deployment on Vercel.

---

## 🚨 Problem → 💡 Solution → 📈 Impact

### Problem
Event hosts need a lightweight, shareable way to collect RSVPs and export guest data without relying on heavy third-party platforms or spreadsheets.

### Solution
- **Shareable invite**: One URL; guests RSVP with name, email, Yes/No, and optional message.
- **Host-only view**: Secure `/host` page with login; view all RSVPs and download as Excel or JSON.
- **Storage options**: Local `data/rsvps.json` for development; Supabase when `DATABASE_URL` is set in production.
- **Minimal setup**: Add invite image, configure host credentials, deploy—no complex setup.

### Impact
- 📲 Single link for guests; no app or account required.
- 📥 Host gets exportable guest list for planning and follow-up.
- 🔒 Credential-protected host area keeps guest data private.
- 🚀 Live at party-shaarty.vercel.app for real-world use.

---

## 🛠️ Technology Stack

| Component | Technology                    |
|-----------|-------------------------------|
| Frontend  | Next.js (App Router)          |
| Backend   | Next.js API Routes           |
| Database  | JSON (dev) or Supabase       |
| Auth      | Cookie-based session (host)  |
| Deployment| Vercel                       |

---

## 🔗 Links

| Resource | URL |
|----------|-----|
| **GitHub** | [CSkarki/PartyShaarty](https://github.com/CSkarki/PartyShaarty) |
| **Live**   | [Utsav-Events.com (Vercel)](https://party-shaarty.vercel.app) |

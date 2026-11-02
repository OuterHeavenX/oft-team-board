# OFT Team Board

Private grading board for the OFT team. Graders sign in with Google, rate each team member on 7 behaviors plus an overall skill level, add comments, and rank everyone by skill today and in 2 years. Managers (Jimmy, Loni) also get a combined dashboard.

- **Hosting:** Cloudflare Pages, auto-deployed from `main`. No build step; the site is the single `index.html`.
- **Backend:** Supabase project "OFT Team Reviews" (Google sign-in, approved-email list, row-level security).
- **Access:** only emails in the `reviewers` table can read or write anything. Role `grader` sees only their own work; role `manager` also sees everyone's.

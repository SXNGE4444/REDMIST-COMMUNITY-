# Gate 02 — Community admissions and manual room matching

**Operational status:** RED MIST has an existing WhatsApp Community with seven groups, a published Tally application at https://tally.so/r/X5lNKj, and a private Supabase `community_applications` intake. A website `/community` entry page is proposed in [draft PR #9](https://github.com/SXNGE4444/REDMIST-WEBSITE/pull/9). Until PR QA/deployment, do not advertise `redmist.org.za/community` as live.

## Registration path

Public website page → choose primary track → Tally application → age, conduct and contact consent → signed Tally webhook → private review queue → decision communicated privately → *optional approved WhatsApp invitation* → intro and first 7-day task → 14-day review.

The website's **existing /access beta registration is a separate route** and currently uses PocketBase; do not silently map those records to WhatsApp without informed contact consent.

## Eight primary interests and rooms to recommend

| Selected Tally role | First working room recommendation | Optional place to find collaborators |
| --- | --- | --- |
| Founders / Entrepreneurship | General then MISSIONS & TEAMS | BUILD TABLES / EVENTS |
| Developers / Software Engineering | HELP DESK then BUILD FLOOR | MISSIONS & TEAMS |
| Designers / Product | BUILD FLOOR then HELP DESK | MISSIONS & TEAMS |
| AI / Data / Research / Hardware | HELP DESK then BUILD FLOOR | MISSIONS & TEAMS |
| Growth / Marketing | SIGNAL then BUILD FLOOR | MISSIONS & TEAMS |
| Operations / Business | BUILD FLOOR then MISSIONS & TEAMS | BUILD TABLES / EVENTS |
| Students / Learners (18+) | General then HELP DESK | BUILD FLOOR |
| Mentors / Advisors | HELP DESK then MISSIONS & TEAMS | BUILD TABLES / EVENTS |

Applicants pick **one primary interest**. It is a discovery preference, not a security role or guaranteed group entitlement. Recommend relevant rooms after human review; do not auto-add or scrape WhatsApp members. New specialised communities should wait until enough active members exist.

## Manual review standard

Do not publish names, phone numbers, application text or scores in this public repository.

1. Confirm application is recorded privately with `review_status=pending` and passes age, conduct and contact consent.
2. Evaluate genuine intention and achievable participation, accounting for beginner status and limited equipment. Avoid automated rejections on education or professional experience.
3. Make review decision with appropriate accountable moderator. Suggested states: `pending → reviewing → approved / declined / withdrawn`.
4. If approved, ask applicant to confirm they understand WhatsApp number visibility, then share the intended Community invitation privately. Keep the invitation out of public website and git.
5. Explain where to post introductions and which room(s) suit the selected track. Start with one small 7-day task.
6. Keep private review and invitation records in an authorized admin tool, not public chats, Drive links or GitHub.
7. Provide a withdrawal/data access contact, a reasonable retention schedule and appeal/reapplication process.

**Moderator guardrail:** a public Tally URL parameter such as `track=developers` is an optional attribution field only. Never approve or grant access based solely on URL parameters; use the verified application answer and human process.

## Acceptance tests before calling Gate 02 live

- [ ] Tally public form shows all eight options and blocks under-18, non-consent and rules refusals.
- [ ] One consented internal end-to-end Tally submission reaches the private Supabase application table exactly once.
- [ ] Supabase anon and authenticated client roles cannot read/write the application table.
- [ ] Review status can be updated **only** through authorized administrator access.
- [ ] Website /community PR passes build, accessibility, link and responsive checks in preview.
- [ ] Production release/rollback and domain route confirmed with screenshots.
- [ ] Moderator can send a private approval invitation and revoke/remove access when needed.
- [ ] No WhatsApp invitation or member phone number appears in public site, source control or client logs.

## Member's first mission

**"My first seven-day build"** — in General, introduce your preferred name, area (not address), interest, experience level and one small goal. In BUILD FLOOR, write: `GOAL / DELIVERABLE / DEADLINE / HELP NEEDED`. At day 7, report `DONE / EVIDENCE / BLOCKER / NEXT`.

No requirement for every student to own a laptop or provide a public portfolio; a written plan or supported learning exercise is acceptable.

**Do not confuse:** published Tally form, accepted application, access to WhatsApp, and an active product membership are distinct states. Each has separate verification.

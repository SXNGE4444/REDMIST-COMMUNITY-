# Community launch and website gates (DRAFT)

## Where we are
RED MIST's public website currently describes a mission-based adult beta, role selection, three Odyssey paths (Bootstrap, Tender, Deep Tech/SaaS), evidence and 14-day reviews. `https://redmist.org.za/access` is publicly discoverable. The separate web app and production signup/auth persistence require functional testing. Nothing in this repository should claim those systems are already verified.

## Recommended community website journeys
Visitor → `/community` → choose LEARN/BUILD/FOUND/MENTOR → `/community/apply` or verified reuse of `/access` → consent + review → approved onboarding → first challenge → mission → evidence → review.

**Functional pages:** /community (purpose/rooms/next event), /community/rules, /community/challenges, /community/events, /community/start, approved missions catalogue. **Do not** create a second competing registration system if existing secure access can be extended.

## Engineering gate checklist
- **G0** Charter, age boundary, approved art, staff roles and data ownership approved.
- **G1** Public community route, accessibility/responsive, clear copy, no fake counts.
- **G2** Application form with validation, confirmation, secure storage, spam protection, review queue, consent ledger.
- **G3** Production role/permission and RLS tests, admin MFA, audit trail, delete/export workflow, no public phone leakage.
- **G4** Mission intake, roles, deadlines, evidence storage, independent review, 14-day reporting.
- **G5** Event RSVP, moderator review, opt-in WhatsApp invites, photo consent and in-person safety process.
- **G6** Tested release: real-device QA, rollback, backup restore, monitoring, negative-path test and recorded pilot outcome.

## Pilot review
After 14 days, evaluate first-task completion, active teams, evidence quality, peer-help response, event attendance, incidents and opt-outs. Keep or remove rooms based on genuine usage. No requirement to build a heavy bespoke chat product while WhatsApp meets the coordination need.

**Security rule:** the public community repository must never contain personal applications, phone numbers, member scoring data, moderator evidence or production secrets.
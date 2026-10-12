# Tech Layoff Club

techlayoffclub.com: a community for laid-off tech workers. Curated 1:1 coffee
chats, matched by hand. Anonymous by default. Not a job board.

## Files

- `index.html` — the waitlist page. Plain static HTML, no build step.

## Deploy (Hostinger + GitHub)

Hostinger hPanel → Websites → techlayoffclub.com → Git:

- Repository: https://github.com/Ltang909/techlayoff
- Branch: main
- Directory: public_html (the site root)

With auto-deployment on, every push to `main` publishes to the live site.

## Waitlist backend

Submissions post to the Google Form "Tech Layoff Club - Waitlist", which
feeds the Google Sheet of the same name.

Form wiring status: live. The form's responder access is "Anyone with the
link", responses link to the "Tech Layoff Club - Waitlist" spreadsheet, and
email notifications for new responses are on (to the form owner's inbox).
The page's `CONFIG.entries` point at this form's field IDs.

History: the first form was created through the Google Forms API and its
editor stayed inaccessible ("You need access") even to the owning account,
so the form was recreated in the Forms UI on 2026-10-12 and the API-created
one abandoned. If a future form is needed, create it in the UI.

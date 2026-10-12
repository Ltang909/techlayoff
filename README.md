# Tech Layoff Club

techlayoffclub.com: a waitlist for laid-off tech workers. Curated 1:1 coffee
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

Form wiring status: the page's `CONFIG.entries` in index.html are filled in
once the form's responder access is set to "Anyone with the link" (Forms
editor → Publish → Responders). Until then the form declines politely
instead of accepting submissions into the void.

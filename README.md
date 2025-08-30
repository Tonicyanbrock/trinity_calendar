# Trinity Calendar

A church events calendar built with [Decap CMS](https://decapcms.org/) and hosted on [Netlify](https://www.netlify.com/).

## Admin Panel
- URL: https://trinity-calendar.netlify.app/admin
- Login handled by Netlify Identity + Git Gateway

## Project Structure
- `admin/`
  - `index.html` → loads Decap CMS and Netlify Identity widget
  - `config.yml` → CMS configuration
- `events.json` → stores calendar events data
- `uploads/` → media files uploaded via the CMS

## Development Notes
- Branch: `main`
- Media assets: stored in `/uploads`
- Publish mode: `editorial_workflow` (allows drafts & reviews)

## Setup
1. Enable Identity and Git Gateway in Netlify dashboard.
2. Invite users from Netlify Identity tab.
3. Visit `/admin` to log in and manage events.

---
*Created for Trinity Episcopal Church, De Soto.*

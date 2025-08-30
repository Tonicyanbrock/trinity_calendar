# ✨ 🕯️ Trinity Calendar 📅

*A simple, friendly way to keep church events updated online.*  
Built with [Decap CMS](https://decapcms.org/) and hosted on [Netlify](https://www.netlify.com/).

---

## 🌐 Website & Admin
- **Calendar Site:** [https://trinity-calendar.netlify.app](https://trinity-calendar.netlify.app)
- **Admin Panel:** [https://trinity-calendar.netlify.app/admin](https://trinity-calendar.netlify.app/admin)

### Logging In
- Login is handled with **Netlify Identity + Git Gateway**.  
- Use the invite email sent by the webmaster to create or reset your password.  
- If you lose your invite or reset link, the site admin can resend one from the **Netlify Identity dashboard**.

---

## 📂 Project Structure
- `admin/`
  - `index.html` → loads Decap CMS and Netlify Identity widget
  - `config.yml` → CMS configuration (backend, collections, media uploads)
- `events.json` → main data file where events are stored
- `uploads/` → folder for uploaded images/media
- `README.md` → this document

---

## ⚙️ Setup & Maintenance
1. **Netlify Dashboard**
   - Enable **Identity** and **Git Gateway** in the site settings.  
   - Registration should remain “Invite only” to prevent spam.  
   - Invite new calendar editors under **Identity → Invite Users**.

2. **Adding Events**
   - Log into the [Admin Panel](https://trinity-calendar.netlify.app/admin).  
   - Create or edit events using the CMS interface.  
   - Changes are stored in `events.json` and automatically published on the site.

3. **File Details**
   - `config.yml` contains the site URL and collection setup.  
   - `events.json` must always exist (with at least `{ "events": [] }` inside).  
   - Media uploads (like flyers or images) are stored in `/uploads`.

---

## 🔑 For Future Maintainers
- **Repository:** [GitHub: Tonicyanbrock/trinity_calendar](https://github.com/Tonicyanbrock/trinity_calendar)  
- **Site Hosting:** Netlify (free tier)  
- **Branch:** `main`

If you are taking over maintenance:
- Keep `config.yml` in sync with the Netlify site URL.  
- Make sure `/admin/index.html` alway

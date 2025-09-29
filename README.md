# Trinity Calendar

A lightweight, zero-dependency calendar for **Trinity Episcopal Church, De Soto, MO**.  
Built with plain HTML, CSS, and JavaScript — no frameworks required.  

## ✨ Features
- Monthly calendar with services, AA/NA meetings, diocesan events, and holidays  
- Liturgical season indicator (with color chips)  
- “Upcoming Events” list (next 30 days)  
- Diocesan button linking to the full diocesan calendar  
- Trinity shield watermark (hidden on print)  
- Print-friendly agenda handout (clean list with church info at top)  

## 🗂️ Files
- `index.html` — main calendar page (includes styles and scripts)  
- `assets/events.json` — local recurring services, AA/NA, holidays  
- `assets/liturgical.json` — liturgical seasons with colors  
- `assets/diocesan.json` — diocesan-wide events  
- `assets/trinity-shield.png` — watermark graphic  
- `assets/trinity_calendar_banner.png` — banner header image  

## 🔑 Updating Events
1. Edit `assets/events.json`, `assets/liturgical.json`, or `assets/diocesan.json`.  
2. Bump the version number in `index.html`:  
   ```js
   const ASSETS_VERSION = 354;
   ```  
   (Increase by +1 so browsers fetch the new files.)  
3. Save and push changes to GitHub.  
4. Netlify redeploys automatically.  
5. Hard refresh browser (Shift+Reload / Ctrl+Shift+R / Cmd+Shift+R).  

## 🖨️ Printing
- Click **Print** in the navigation bar → prints a clean “Upcoming Events” agenda.  
- Church info + quote included at top.  
- Shield watermark hidden for readability.  

## 📬 Contact
**Trinity Episcopal Church**  
202 W. Miller Street · PO Box 9 · De Soto, MO 63020 · United States  
Phone: (636) 586-2542  
Email: [trinitydesoto@gmail.com](mailto:trinitydesoto@gmail.com)  

> *"Lift each other up, for life is better when shared."*

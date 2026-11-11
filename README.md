# Business Award 2026 Website

Responsive premium navy-and-gold website. The existing visual theme, logo assets, trophy visual and page sections are retained.

## Event details
- Business Award 2026 — 30 November 2026, Monday, 10:00 AM
- Bangalore; venue listed in the project brief as Radisson Blu Hotel, Bangalore
- Presented by Chitra Sante & Associates; in association with EagleReach Marketing
- Administrator notification email: eaglereachmarketing24@gmail.com

## Guest list shown on the supplied poster
- Sri Krishna Byregowda — Minister for Greater Bengaluru Development
- Sri Cheluvarayaswamy — Minister for Major and Medium Irrigation
- Sri Santosh Lad — Minister for Labour and Employment
- Sri U. T. Khader — Minister for Health and Family Welfare
- Sri Shashi Kumar
- Smt. Priyanka Upendra

The poster listing is not independent confirmation of attendance.

## Forms added
- Separate **Nominate Now** and **Become a Sponsor** buttons in the navigation and hero area.
- Each button opens its own responsive modal form; neither form opens automatically.
- Visitors can close the form with the X button, Escape key, or by clicking outside the dialog.
- Native required-field, email, URL and mobile validation is enabled.
- Forms are configured to submit to Google Apps Script, which stores entries in a Google Sheet and emails the administrator.

## Required setup before submissions can be received
1. Sign in to Google using `eaglereachmarketing24@gmail.com` and open `https://script.google.com`.
2. Create a new project and paste the contents of `Code.gs` from this ZIP.
3. Save, choose **Deploy → New deployment → Web app**. Set **Execute as: Me** and **Who has access: Anyone**. Authorize the project and deploy.
4. Copy the deployed Web app URL ending in `/exec`.
5. In `index.html`, replace `PASTE_YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE` with that URL. Make the same replacement in `dist/index.html`.
6. Publish the contents of `dist/` (or the project folder) to your hosting provider.
7. Submit one test nomination and one test sponsorship enquiry. Confirm both rows appear in the Google Sheet and notification emails arrive. Delete test rows afterwards if desired.

The Google Sheet is created automatically on the first successful submission in the Google account that deployed the script. The sheet URL is emailed to the administrator. Keep the Apps Script deployment access and Google account secure.

## Local preview
- `npm start` starts the included Node server (default port 3000).
- `npm run build` creates a `dist/` folder.

## Before publishing
- Confirm venue booking and guest participation directly.
- Confirm the event contact number and administrator email.
- Replace the Apps Script placeholder and test both forms on phone and desktop.

### Homepage trophy image
The homepage hero now uses `assets/award-trophy-hero.png`, the premium gold trophy image supplied by the event organizer. The same asset is included in `dist/assets/` for the production build.

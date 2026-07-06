# Agnes Mariadas — Relationship Coach Website

A fast, static website (HTML/CSS/JS only — no build step, no server required).

## Go live on GitHub Pages (free) — step by step

1. **Create a GitHub account** (skip if you have one): https://github.com/signup

2. **Create a new repository**
   - Click the **+** icon (top right) → **New repository**
   - Name it: `agnes-mariadas-website` (or anything you like)
   - Set it to **Public**
   - Click **Create repository**

3. **Upload these files**
   - On the new repo page, click **uploading an existing file**
   - Drag in *everything* from this folder (`index.html`, `about.html`, `services.html`, `blog.html`, `contact.html`, the `css` folder, and the `js` folder) — keep the folder structure intact
   - Scroll down, click **Commit changes**

4. **Turn on GitHub Pages**
   - Go to the repo's **Settings** tab → **Pages** (left sidebar)
   - Under "Build and deployment" → **Source**, choose **Deploy from a branch**
   - Branch: **main**, folder: **/ (root)** → **Save**

5. **Get your live link**
   - Wait 1–2 minutes, then refresh that Pages settings screen
   - Your site will be live at:
     `https://YOUR-GITHUB-USERNAME.github.io/agnes-mariadas-website/`

6. **(Optional) Use a custom domain**
   - Buy a domain (e.g. `agnesmariadas.com`) from Namecheap, GoDaddy, or Google Domains (~$10–15/year)
   - In the same **Settings → Pages** screen, enter it under "Custom domain"
   - Follow GitHub's DNS instructions (they'll show you exact records to add at your domain registrar)

## Turning on the booking calendar

The Contact page has a booking section ready to go. To activate real-time scheduling:

1. Create a free account at https://calendly.com
2. Create an event type, e.g. "20-Minute Discovery Call"
3. Copy your scheduling link
4. Open `contact.html`, find the comment block starting `CALENDLY SETUP`
5. Uncomment the `<iframe>` block just below it and paste your link in place of `YOUR-CALENDLY-LINK`

Until that's done, visitors see a friendly "request via WhatsApp" fallback instead — the site works fine either way.

## Making the contact form actually deliver emails

Right now the form shows a confirmation message but doesn't send anywhere. To connect it:
- Sign up free at https://formspree.io, create a form pointed at agnes.m174@gmail.com, and swap the form's `action` attribute to the Formspree endpoint they give you (a few lines of change in `contact.html`) — ask and I can do this for you directly.

## Adding real photos

Replace the placeholder boxes labeled "Photo of Agnes coming soon" in `index.html` and `about.html`:
1. Add your photo file to the `images` folder (create one if it doesn't exist)
2. Replace the `.hero-portrait` div content with an `<img src="images/your-photo.jpg" alt="Agnes Mariadas">` tag

## File structure
```
├── index.html        Homepage
├── about.html         About Agnes
├── services.html      Coaching services
├── blog.html           Blog listing
├── contact.html       Contact + booking
├── css/style.css      All styling
└── js/main.js          Nav, scroll animations, form handling
```

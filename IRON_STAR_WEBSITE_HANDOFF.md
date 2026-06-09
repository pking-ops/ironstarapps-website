# Iron Star Apps Website Handoff File

## Current Website Purpose
This is the current public landing page for Iron Star Apps. The site is designed as a black/blue tactical-tech style homepage focused on church safety, training, consulting/planning, and off-duty coordination.

## Current Hosting Workflow
- Source files are uploaded to GitHub.
- Vercel deploys the website from the GitHub repository.
- The domain `ironstarapps.com` / `www.ironstarapps.com` is pointed to Vercel through DNS.

## Current Public Website Contact Info
- Company Phone: 979-446-0006
- Quotes Email: quotes@ironstarapps.com
- Facebook: https://Facebook.com/Ironstarapps
- Location Display: Texas, USA

## Contact Form
The contact/request-info form is configured to submit through FormSubmit:

`https://formsubmit.co/quotes@ironstarapps.com`

Important: The first time the form is tested after this change, FormSubmit may send a confirmation/activation email to `quotes@ironstarapps.com`. The form will not fully deliver submissions until that email is confirmed.

## Main Files
- `index.html` — main homepage
- `styles.css` — site styling and mobile responsiveness
- `script.js` — mobile menu behavior
- `hero-bg.png` — cinematic black/blue hero background image
- `iron-star-apps-shield-logo-header.png` — current website logo
- `thank-you.html` — confirmation page after form submission
- `README.txt` — basic deployment notes

## Current Page Sections
1. Header / Navigation
   - Services
   - Training
   - About
   - Resources
   - Contact
   - Request Info button

2. Hero Section
   - Iron Star Apps branding
   - “Protection. Preparedness. Peace of Mind.”
   - Start a Conversation button
   - Our Services button
   - Cinematic church/security hero background

3. Trust Strip
   - Real-World Experience
   - Practical Solutions
   - Secure by Design
   - Built for Teams You Trust

4. Services Built For You
   - Church Safety
   - Training
   - Consulting / Planning
   - Off-Duty Coordination

5. What We Do / Process
   - Assess
   - Plan
   - Train
   - Implement
   - Support

6. Trusted By Band
   - “Trusted by Churches, Schools, & Agencies”

7. Footer / Contact Area
   - Company phone
   - Quotes email
   - Facebook page
   - Services links
   - Contact form
   - Thank-you page redirect

## DNS / Domain Notes
Vercel showed these DNS values during setup:

- Root domain `ironstarapps.com`
  - Type: A
  - Host/Name: @
  - Value: 216.198.79.1

- WWW domain `www.ironstarapps.com`
  - Type: CNAME
  - Host/Name: www
  - Value: bf4d2e0fa9b207bc.vercel-dns-017.com

Only website A/CNAME records should be changed for website hosting. Do not delete email records such as MX, TXT, SPF, DKIM, or DMARC unless the email provider specifically instructs it.

## Upload / Deployment Steps
1. Download and unzip the website package.
2. Open the unzipped folder.
3. Upload the files inside the folder to the GitHub repository root.
4. Commit changes.
5. Vercel should automatically redeploy.
6. After deployment, test:
   - Homepage loads
   - Mobile menu works
   - Request Info buttons scroll to contact/form area
   - Form submits to `quotes@ironstarapps.com`
   - Thank-you page loads
   - Facebook link opens correctly

## Important Future Notes
- The form currently uses FormSubmit, which is a no-backend form service. For a more professional setup later, consider using a dedicated form backend, CRM, or custom API.
- If spam becomes a problem, add CAPTCHA or switch to a protected form provider.
- The public-facing email should now be `quotes@ironstarapps.com`.
- The main company phone number should now be `979-446-0006`.




# Upload / Update Instructions for GitHub + Vercel

## Purpose
Use these steps when updating the Iron Star Apps website files. The site is hosted through Vercel and deployed from GitHub.

## Important Rule
Do **not** upload the ZIP file directly to GitHub as the website.  
Always unzip the package first, then upload the files inside the folder.

## Files That Should Be Uploaded to GitHub
Upload these files to the root/top level of the GitHub repository:

- `index.html`
- `styles.css`
- `script.js`
- `hero-bg.png`
- `iron-star-apps-shield-logo-header.png`
- `site-mockup-reference.png`
- `thank-you.html`
- `README.txt`
- `IRON_STAR_WEBSITE_HANDOFF.md`
- `IRON_STAR_WEBSITE_HANDOFF.txt`

## GitHub Upload Steps
1. Download the latest website ZIP file.
2. Right-click the ZIP file on your computer.
3. Click **Extract All**.
4. Open the extracted folder.
5. Select all files inside the extracted folder.
6. Go to the GitHub repository for the Iron Star Apps website.
7. If old files are already there, replace them with the new files.
8. Drag the new files into GitHub’s upload area.
9. Scroll down to the commit section.
10. Type a commit message such as:

   `Update Iron Star website contact info and handoff file`

11. Choose **Commit directly to the main branch**.
12. Click **Commit changes**.

## Vercel Deployment Steps
If GitHub is already connected to Vercel, Vercel should redeploy automatically after the GitHub commit.

To check deployment:
1. Open Vercel.
2. Open the `ironstarapps-website` project.
3. Click **Deployments**.
4. Confirm the latest deployment finished successfully.
5. Open the live site and verify the updates.

## Testing Checklist After Upload
After Vercel redeploys, test the website:

- Open `https://ironstarapps.com`
- Open `https://www.ironstarapps.com`
- Confirm the company phone shows: `979-446-0006`
- Confirm the email shows: `quotes@ironstarapps.com`
- Confirm the Facebook link opens: `https://Facebook.com/Ironstarapps`
- Click **Request Info**
- Submit a test form
- Confirm the thank-you page loads
- Check `quotes@ironstarapps.com` for FormSubmit activation/confirmation
- After activation, submit another test form and confirm the email arrives

## FormSubmit Warning
The form uses FormSubmit. The first test submission may trigger a confirmation email to `quotes@ironstarapps.com`. The form may not deliver future messages until that confirmation is completed.

## DNS Notes
The domain is pointed to Vercel using DNS records.

Known Vercel DNS values from setup:

Root domain:
- Type: `A`
- Host/Name: `@`
- Value: `216.198.79.1`

WWW domain:
- Type: `CNAME`
- Host/Name: `www`
- Value: `bf4d2e0fa9b207bc.vercel-dns-017.com`

Do not remove email DNS records such as MX, TXT, SPF, DKIM, or DMARC unless the email provider specifically instructs it.

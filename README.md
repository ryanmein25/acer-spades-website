# Acer Spades Gardening - Static Website

Professional garden maintenance and landscaping services website for Ross-on-Wye, Herefordshire.

## File Structure

```
vercel-deploy/
├── index.html              # Main webpage
├── vercel.json             # Vercel configuration
├── README.md               # This file
├── assets/                 # JavaScript & CSS bundles
│   ├── index-xxxxx.js      # Main application bundle
│   └── index-xxxxx.css     # Compiled styles
├── attached_assets/        # Website images
│   ├── Hero Image_xxx.JPG  # Hero background
│   ├── logo.jpg            # Company logo
│   └── ... (portfolio images)
└── images/                 # Before/After comparison images
    ├── before_1.jpg
    ├── after_1.jpg
    └── ...
```

## Vercel Deployment (Drag & Drop)

### Step 1: Go to Vercel
1. Visit [vercel.com](https://vercel.com)
2. Sign up or log in with your account

### Step 2: Deploy
1. From your Vercel dashboard, click **"Add New..."** → **"Project"**
2. Click **"Deploy without Git"** or look for the upload option
3. **Drag and drop** the entire `vercel-deploy` folder onto the upload area
4. Wait for deployment to complete (usually 30-60 seconds)
5. Your site will be live at a `.vercel.app` URL

### Step 3: Test Your Site
1. Click the provided URL to view your live site
2. Test all functionality:
   - Navigation menu
   - Image carousel
   - Before/after sliders
   - Contact form
   - Mobile responsiveness

## Custom Domain Setup (www.acerspadesgardening.uk)

### Step 1: Add Domain in Vercel
1. Go to your project in Vercel dashboard
2. Click **"Settings"** → **"Domains"**
3. Enter `www.acerspadesgardening.uk` and click **"Add"**
4. Also add `acerspadesgardening.uk` (without www) for redirects

### Step 2: Update DNS Settings
Vercel will show you the DNS records to add. Typically:

**Option A: Using Vercel Nameservers (Recommended)**
- Go to your domain registrar (where you bought the domain)
- Change nameservers to Vercel's nameservers

**Option B: Using A/CNAME Records**
- Add an A record: `@` → `76.76.21.21`
- Add a CNAME record: `www` → `cname.vercel-dns.com`

### Step 3: SSL Certificate
- Vercel automatically provisions SSL certificates
- HTTPS will work automatically once DNS propagates (up to 48 hours)

## Contact Form Setup (Formspree)

The contact form is currently a placeholder. To make it functional:

### Step 1: Create Formspree Account
1. Go to [formspree.io](https://formspree.io)
2. Sign up for a free account
3. Create a new form
4. Copy your form ID (looks like `xyzabcde`)

### Step 2: Update the Website
1. Open `assets/index-xxxxx.js` in a text editor
2. Search for `YOUR_FORM_ID`
3. Replace it with your actual Formspree ID
4. Re-upload the folder to Vercel

### Step 3: Test the Form
1. Submit a test message on your live site
2. Check your Formspree dashboard for the submission
3. Verify email notifications are working

## Important Notes

### What's Included
- ✅ Fully responsive design (mobile, tablet, desktop)
- ✅ Smooth scroll animations
- ✅ Image carousel with navigation
- ✅ Before/after comparison sliders
- ✅ Contact form (requires Formspree setup)
- ✅ Google Maps embed
- ✅ Social media links

### Browser Support
- Chrome, Firefox, Safari, Edge (latest versions)
- Mobile browsers (iOS Safari, Chrome for Android)

### Performance
- Optimized images and assets
- Gzip compression enabled via Vercel
- Static caching for fast load times

## Troubleshooting

### Images Not Loading
- Verify all files in `attached_assets/` and `images/` were uploaded
- Check browser console for 404 errors
- Ensure file names match exactly (case-sensitive)

### Form Not Working
- Confirm you replaced `YOUR_FORM_ID` with actual Formspree ID
- Check Formspree dashboard for form status
- Test in incognito mode to rule out caching issues

### Domain Not Working
- DNS changes can take up to 48 hours to propagate
- Use [whatsmydns.net](https://whatsmydns.net) to check propagation
- Verify DNS records match Vercel's requirements

## Support

- **Vercel Documentation:** [vercel.com/docs](https://vercel.com/docs)
- **Formspree Help:** [help.formspree.io](https://help.formspree.io)

---

*Built for Acer Spades Gardening - Professional garden services in Ross-on-Wye, Herefordshire, Gloucestershire & Monmouth*

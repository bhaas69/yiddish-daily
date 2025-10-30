# Yiddish Daily

**One surprising discovery from the Yiddish world. Every day.**

A simple, beautiful Jekyll site ready to deploy on GitHub Pages for free.

---

## 🚀 Quick Start (Deploy in 10 minutes)

### Step 1: Upload to GitHub

1. **Create a GitHub account** if you don't have one: https://github.com/join
2. **Create a new repository**:
   - Go to https://github.com/new
   - Name it: `yiddish-daily` (or anything you like)
   - Make it **Public**
   - Don't initialize with README (you already have one)
   - Click "Create repository"

3. **Upload your files**:
   - On your new repo page, click "uploading an existing file"
   - Drag and drop ALL files and folders from this `yiddish-daily` directory
   - Or use Git if you know how (see below)
   - Commit the files

### Step 2: Enable GitHub Pages

1. In your repository, click **Settings** (top right)
2. Scroll down to **Pages** (left sidebar)
3. Under "Source", select **main** branch
4. Click **Save**
5. Wait 2-3 minutes for the site to build
6. Your site will be live at: `https://YOUR-USERNAME.github.io/yiddish-daily/`

**That's it! Your site is now live and free forever.**

---

## 📝 Adding New Posts

Posts go in the `_posts` folder with this naming pattern:
```
YYYY-MM-DD-title-of-post.md
```

Example: `2025-10-31-yiddish-typewriter.md`

### Post Template

Create a new file in `_posts` with this structure:

```markdown
---
layout: post
title: "Your Discovery Title Here"
date: 2025-10-31 08:00:00 -0400
---

Your introduction paragraph here.

![Image description](/assets/images/your-image.jpg)

## A Section Header

More content here...

## Another Section

Even more fascinating content...

---

*Source: Where you found this. Link if available.*
```

### Adding Images

1. Put images in: `assets/images/`
2. Reference them in posts: `![Description](/assets/images/filename.jpg)`
3. Commit and push to GitHub
4. Image appears automatically!

---

## ✉️ Setting Up Email Signup

The homepage has an email signup form ready to go. You need to connect it to an email service:

### Option A: Buttondown (Recommended - Free tier available)

1. Go to https://buttondown.email
2. Sign up for free account
3. Get your signup form URL
4. Edit `index.html` and replace this line:
   ```html
   <form class="email-form" action="https://buttondown.email/api/emails/embed-subscribe/yiddish-daily" method="post">
   ```
   With your actual Buttondown URL

### Option B: Mailchimp (Also good)

1. Sign up at https://mailchimp.com
2. Create an audience
3. Get the embedded form code
4. Replace the form in `index.html` with Mailchimp's code

### Email Automation

Once you have subscribers, you can auto-send daily posts:
- **Buttondown**: Has built-in RSS-to-email (just point it to your feed.xml)
- **Mailchimp**: Use RSS Campaign feature
- **Schedule**: Set to send daily at 8am (or whenever you prefer)

Your RSS feed is automatically available at: `https://YOUR-USERNAME.github.io/yiddish-daily/feed.xml`

---

## 🎨 Customization

### Change Site Title/Description

Edit `_config.yml`:
```yaml
title: Your Title
description: Your tagline
```

### Change Colors

Edit `assets/css/style.css` - main colors to change:
- `#2c3e50` - Dark blue (header background)
- `#3498db` - Bright blue (links, buttons)
- `#fff` - White (text on dark)

### Add Your Own Domain (Optional)

1. Buy a domain (Namecheap, Google Domains, etc.)
2. In your repo, create a file named `CNAME` with just your domain:
   ```
   yiddishdaily.com
   ```
3. Point your domain's DNS to GitHub Pages (instructions from your domain provider)

---

## 🔧 Local Development (Optional)

If you want to preview changes before pushing to GitHub:

### Install Jekyll

```bash
# Install Ruby (if you don't have it)
# Then install Jekyll:
gem install bundler jekyll

# Navigate to your site folder:
cd yiddish-daily

# Install dependencies:
bundle install

# Run the site locally:
bundle exec jekyll serve

# View at: http://localhost:4000
```

Now you can edit files and see changes instantly!

---

## 📊 Adding Analytics (Optional)

### Google Analytics

1. Sign up at https://analytics.google.com
2. Get your tracking ID
3. Add to `_layouts/default.html` before `</head>`:
   ```html
   <!-- Google Analytics -->
   <script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-ID"></script>
   <script>
     window.dataLayer = window.dataLayer || [];
     function gtag(){dataLayer.push(arguments);}
     gtag('js', new Date());
     gtag('config', 'YOUR-ID');
   </script>
   ```

---

## 💰 Adding Ads (When You're Ready)

### Google AdSense

1. Apply at https://www.google.com/adsense
2. Wait for approval (need some traffic first)
3. Add ad code to `_layouts/post.html` or `_layouts/default.html`

**Realistic timeline:**
- Months 1-3: Build content, no ads yet
- Months 4-6: Apply for AdSense
- Month 6+: Start earning (slowly at first)

---

## 🔄 Using Git (Alternative to Web Upload)

If you're comfortable with Git:

```bash
cd yiddish-daily
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/yiddish-daily.git
git push -u origin main
```

---

## 📁 File Structure

```
yiddish-daily/
├── _config.yml          # Site configuration
├── _layouts/            # Page templates
│   ├── default.html     # Base layout
│   └── post.html        # Individual post layout
├── _posts/              # Your blog posts (add new ones here!)
│   └── 2025-10-30-coca-cola-yiddish-ad.md
├── assets/
│   ├── css/
│   │   └── style.css    # Site styling
│   └── images/          # Post images (add images here!)
├── index.html           # Homepage
├── archive.html         # Archive page (lists all posts)
├── Gemfile              # Jekyll dependencies
└── README.md            # This file
```

---

## 🎯 Content Strategy Tips

### To Grow Your Audience:

1. **Post consistently**: Daily is ideal, but start with 3x/week if needed
2. **Be genuinely interesting**: Share discoveries YOU find fascinating
3. **Keep it digestible**: 200-500 words is perfect for daily content
4. **Great images**: Visual content gets shared more
5. **Share everywhere**: Reddit (r/Yiddish), Twitter, Facebook groups
6. **Build email list**: That's where the value is long-term

### Content Ideas:

- Vintage advertisements (like your Coca-Cola ad!)
- Newspaper clippings with surprising stories
- Yiddish words with no English equivalent
- Photos of Yiddish signage
- Quotes from Yiddish literature/poetry
- Historical facts about Yiddish culture
- Yiddish music discoveries
- Famous Yiddish speakers
- Yiddish theater posters
- Letters, documents, menus

---

## ❓ Troubleshooting

**Site not showing up?**
- Wait 5 minutes after first push
- Check Settings > Pages shows "Your site is live"
- Make sure repository is Public

**Posts not appearing?**
- Check filename format: `YYYY-MM-DD-title.md`
- Check front matter has `layout: post`
- Check date isn't in the future

**Styling looks broken?**
- Clear browser cache
- Check `style.css` uploaded correctly
- Check browser console for errors

**Images not loading?**
- Check path: `/assets/images/filename.jpg`
- Check image actually uploaded to GitHub
- Check filename matches exactly (case-sensitive!)

---

## 🚀 Next Steps

1. ✅ Upload to GitHub
2. ✅ Enable GitHub Pages
3. ✅ Add your Premier Coffee ad image to `assets/images/` (already included!)
4. ✅ Set up email signup (Buttondown)
5. ⬜ Write 5-10 more posts to have a backlog
6. ⬜ Schedule posts to go live daily
7. ⬜ Share your first post to relevant communities
8. ⬜ Set up Google Analytics
9. ⬜ Keep posting consistently!

---

## 📞 Support

- **Jekyll Docs**: https://jekyllrb.com/docs/
- **GitHub Pages Docs**: https://docs.github.com/en/pages
- **Markdown Guide**: https://www.markdownguide.org/

---

## 📜 License

This theme is open source. Do whatever you want with it!

---

**Ready to preserve Yiddish culture, one discovery at a time?** 🎉

Start by uploading to GitHub and enabling Pages. You'll have a live site in 10 minutes!

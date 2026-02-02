# Srijith Reddy Pakala - Academic Portfolio Website

A modern, multi-page academic portfolio website featuring Apple SF Pro font styling, university logos, and a markdown-based blog system.

## 📁 File Structure

```
portfolio/
├── index.html          # Home page with intro, contacts, and education
├── experience.html     # Professional experience timeline
├── projects.html       # Academic and technical projects
├── blogs.html         # Blog editor and posts
└── README.md          # This file
```

## 🎨 Features

### Home Page (index.html)
- Clean hero section with name and professional summary
- Contact links with icons (Email, LinkedIn, GitHub, Phone)
- Education section with university logos:
  - UC San Diego logo
  - IIT Hyderabad logo
- Degree information, coursework, and dates

### Experience Page (experience.html)
- Three professional experiences with detailed descriptions
- Company names, locations, and durations
- Skill tags for each position
- Hover effects and responsive design

### Projects Page (projects.html)
- Four academic projects in card layout
- Project icons, tags, and descriptions
- Detailed specifications for each project
- Performance metrics and achievements

### Blogs Page (blogs.html)
- **Markdown editor** for writing posts
- Live preview and publishing
- Posts saved to browser localStorage
- Automatic date stamping
- Delete functionality
- Beautiful typography for rendered markdown

## 🚀 Getting Started

### Option 1: Open Directly
1. Download all HTML files to a folder
2. Open `index.html` in your web browser
3. Navigate using the top navigation menu

### Option 2: Local Server (Recommended)
```bash
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if you have http-server installed)
npx http-server
```

Then open `http://localhost:8000` in your browser.

## ✍️ Writing Blog Posts

### Using the Blog Editor

1. Navigate to the **Blogs** page
2. Enter your post title
3. Write content in Markdown format
4. Click **Publish Post**

### Markdown Syntax Reference

```markdown
# Heading 1
## Heading 2
### Heading 3

**Bold text**
*Italic text*

- Bullet point
- Another point

1. Numbered item
2. Second item

[Link text](https://example.com)

`inline code`

```
code block
multiple lines
```

> Blockquote for emphasis
```

### Example Blog Post

```markdown
# My First Week at UCSD

Today marks the end of my first week in the ECE program at UC San Diego!

## Initial Impressions

The coursework is challenging but exciting:

- **Analog IC Design**: Started with differential amplifiers
- **Microwave Circuits**: Learning S-parameters
- **Biomedical ICs**: Exploring low-power sensor interfaces

## Lab Access

Got access to the Cadence design tools. Planning to start my first project on:

1. LNA design optimization
2. Power consumption analysis
3. Layout and verification

More updates coming soon!
```

## 🎨 Customization Guide

### Changing Personal Information

**Home Page (index.html):**
- Line 182: Update your name
- Line 183: Update your professional title
- Line 184-188: Update your introduction
- Lines 193-213: Update contact links (email, LinkedIn, GitHub, phone)

### Adding/Editing Experience

**Experience Page (experience.html):**
- Copy the `.experience-item` div structure
- Update position, company, dates, location
- Modify bullet points under `.description ul`
- Update skill tags in `.skills-used`

### Adding/Editing Projects

**Projects Page (projects.html):**
- Copy the `.project-card` div structure
- Change the icon class (FontAwesome icons)
- Update title, tags, description
- Modify specifications in `.project-specs`

### Customizing Colors

Main brand color (blue): `#0066cc`

To change throughout the site, search and replace:
- `#0066cc` with your preferred color
- `#0055b3` (darker hover state) with a darker shade
- `#0099ff` (gradient) with a lighter shade

## 📱 Responsive Design

The website is fully responsive and works on:
- Desktop (1920px+)
- Laptop (1024px - 1920px)
- Tablet (768px - 1024px)
- Mobile (< 768px)

## 💾 Blog Data Storage

Blog posts are stored in your browser's localStorage under the key `srijith_blogPosts`.

### Exporting Blog Data

Open browser console (F12) and run:
```javascript
console.log(localStorage.getItem('srijith_blogPosts'));
// Copy the output to save externally
```

### Importing Blog Data

```javascript
localStorage.setItem('srijith_blogPosts', 'YOUR_EXPORTED_DATA_HERE');
location.reload();
```

### Clearing All Posts

```javascript
localStorage.removeItem('srijith_blogPosts');
location.reload();
```

## 🔤 Fonts

The website uses Apple's SF Pro font family:
- **SF Pro Display** - Large headings and titles
- **SF Pro Text** - Body text and paragraphs
- **SF Mono** - Code blocks and markdown editor

On Apple devices, you'll see the actual SF Pro fonts. On other systems, it gracefully falls back to system fonts.

## 🎯 Icons

Using Font Awesome 6.4.0 CDN for all icons:
- Contact icons (email, LinkedIn, GitHub, phone)
- Project icons (microchip, signal, wave, calculator)
- Blog action icons (pen, calendar, trash)

To change icons, visit [FontAwesome](https://fontawesome.com/icons) and replace the icon class names.

## 🌐 Adding More Pages

To add a new page:

1. Create a new HTML file (e.g., `publications.html`)
2. Copy the structure from any existing page
3. Add navigation link in all pages:

```html
<nav>
    <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="experience.html">Experience</a></li>
        <li><a href="projects.html">Projects</a></li>
        <li><a href="publications.html">Publications</a></li>
        <li><a href="blogs.html">Blogs</a></li>
    </ul>
</nav>
```

## 🚀 Deployment Options

### GitHub Pages
1. Create a GitHub repository
2. Upload all HTML files
3. Go to Settings → Pages
4. Select main branch
5. Your site will be at `https://username.github.io/repo-name`

### Netlify
1. Drag and drop your folder to [Netlify Drop](https://app.netlify.com/drop)
2. Get instant hosting with HTTPS

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your folder
3. Follow the prompts

## 📝 Tips for Daily Blogging

1. **Keep it simple**: Short posts are fine - even 2-3 paragraphs
2. **Use markdown**: Faster than formatting in a rich text editor
3. **Regular schedule**: Try posting at the same time each day
4. **Topics to cover**:
   - Daily learning insights
   - Project progress updates
   - Interesting paper summaries
   - Debug sessions and solutions
   - Course reflections

## 🔧 Troubleshooting

**Blog posts not saving?**
- Check if localStorage is enabled in your browser
- Try a different browser
- Check browser storage quota

**University logos not showing?**
- Images are loaded from Wikipedia CDN
- Check your internet connection
- Replace with local images if needed

**Icons not displaying?**
- Font Awesome CDN might be blocked
- Check browser console for errors
- Download Font Awesome locally if needed

## 📄 License

Free to use and modify for personal and academic purposes.

## 🤝 Contact

- Email: srijithreddypakala001@gmail.com
- LinkedIn: [linkedin.com/in/srijith-pakala](https://www.linkedin.com/in/srijith-pakala/)
- GitHub: [github.com/SRIJITH01](https://github.com/SRIJITH01)

---

Built with ❤️ using HTML, CSS, and vanilla JavaScript

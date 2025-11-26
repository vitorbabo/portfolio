# Portfolio - Markdown-Driven CV Website

A modern, responsive portfolio website that dynamically generates content from a markdown CV file.

## Features

- **Markdown-Driven**: All content is extracted from `cv.md` - simply update the markdown file to update your portfolio
- **Responsive Design**: Fully responsive layout that works on desktop, tablet, and mobile devices
- **Dark Theme**: Modern dark theme with orange accent colors
- **Sections Included**:
  - Hero section with name, title, and professional summary
  - Work experience timeline
  - Technical skills organized by category
  - Projects and achievements
  - Education timeline
  - Contact section

## Files

- `index.html` - Main portfolio page with embedded JavaScript parser
- `cv.md` - Your CV in markdown format (edit this to update your portfolio)

## Usage

### Local Development

1. Start a local HTTP server:
   ```bash
   python3 -m http.server 8080
   ```

2. Open your browser and navigate to:
   ```
   http://localhost:8080
   ```

### Updating Your Portfolio

Simply edit the `cv.md` file with your information. The portfolio will automatically parse and display:

- Your name and contact information
- Professional summary
- Work experience
- Technical skills (categorized)
- Projects and achievements
- Education
- Contact details

### CV Markdown Format

The `cv.md` file should follow this structure:

```markdown
# Your Name

Location | Phone | Email

LinkedIn: linkedin.com/in/yourprofile

### PROFESSIONAL SUMMARY

Your professional summary here...

### WORK EXPERIENCE

**Company | Job Title**
_Start Date – End Date_

- Key achievement or responsibility
- Another achievement

### TECHNICAL SKILLS

- **Category Name:** Skill1, Skill2, Skill3

### PROJECTS & ACHIEVEMENTS

- **Project Title:** Project description

### EDUCATION

Degree | Institution | Year
```

## Customization

### Colors

The theme uses Tailwind CSS with custom colors defined in the `<script>` tag:
- Primary: `#f69412` (orange)
- Background (light): `#f8f7f5`
- Background (dark): `#221a10`

To change colors, edit the `tailwind.config` object in `index.html`.

### Profile Image

Update the `src` attribute of the `#profile-image` element in `index.html` to use your own photo.

### Social Links

The portfolio includes placeholder links for LinkedIn and GitHub. These are automatically populated from your CV where possible, or can be manually configured in the JavaScript.

## Deployment

This portfolio is a static website and can be deployed to any static hosting service:

- GitHub Pages
- Netlify
- Vercel
- AWS S3
- Or any web server

Simply upload `index.html` and `cv.md` to your hosting service.

## Technologies Used

- HTML5
- Tailwind CSS (via CDN)
- Vanilla JavaScript (no dependencies)
- Material Symbols Icons
- Space Grotesk Font (Google Fonts)

## Browser Support

Works on all modern browsers that support:
- ES6 JavaScript
- CSS Grid
- Flexbox
- Fetch API

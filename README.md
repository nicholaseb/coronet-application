# Coronot Application Materials

Professional application materials for the 3D Animation Artist position at Coronot, ready to deploy to GitHub Pages.

## Files Included

### Main Site Files (Root)
- **index.html** - Portfolio website homepage with video sections
- **resume.html** - Professional resume (print-ready for PDF)
- **cover-letter.html** - Cover letter (print-ready for PDF)
- **styles.css** - Shared stylesheet for all pages

### Supporting Files
- **docs/executive-email-template.md** - Email templates for reaching out to executives
- **docs/job-application-questions.md** - Original questionnaire with your responses
- **videos/** - Folder for your animation video files

## Getting Started

### 1. Add Your Videos

1. Create a `videos/` folder in this repository
2. Add your animation video files (MP4 format recommended)
3. Open `index.html` and replace the video placeholders:
   - Remove the `<div class="video-placeholder">` elements
   - Uncomment the `<video>` tags
   - Update the `src` paths to point to your video files
   - Update descriptions for each video

**Alternative:** You can embed videos from YouTube, Vimeo, or Google Drive using iframe embeds instead.

### 2. Deploy to GitHub Pages

1. **Push to GitHub:**
   ```bash
   git add .
   git commit -m "Initial commit: Coronot application materials"
   git push origin main
   ```

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under **Source**, select **main** branch (or your default branch)
   - Click **Save**
   - Your site will be live at: `https://[your-username].github.io/[repository-name]/`

3. **Update Email Template:**
   - Open `docs/executive-email-template.md`
   - Replace `[your portfolio URL]` with your actual GitHub Pages URL
   - Personalize each email with the recipient's name

### 3. Generate PDF Versions

**For Resume:**
1. Open `resume.html` in your browser
2. Press Cmd/Ctrl + P to open the print dialog
3. Select "Save as PDF" as the destination
4. Adjust margins if needed (should be preset to 0.5in)

**For Cover Letter:**
1. Open `cover-letter.html` in your browser
2. Press Cmd/Ctrl + P to open the print dialog
3. Select "Save as PDF" as the destination

## Customization

### Update Contact Information
If you need to update contact info, edit:
- `resume.html` - Header section
- `cover-letter.html` - Header section
- `index.html` - Footer section

### Adjust Styling
All styling is in `styles.css`. Key sections:
- Print styles (for PDF generation)
- Portfolio layout
- Resume/cover letter formatting

### Add More Videos
Duplicate the video item structure in `index.html`:
```html
<div class="video-item">
    <h3>Your Video Title</h3>
    <video controls>
        <source src="videos/your-video.mp4" type="video/mp4">
    </video>
    <p>Your description here.</p>
</div>
```

## File Structure

```
coronet-application/
├── index.html                    # Portfolio homepage (main entry point)
├── resume.html                   # Resume (linked from portfolio)
├── cover-letter.html             # Cover letter (linked from portfolio)
├── styles.css                    # Shared stylesheet
├── README.md                     # This file
├── videos/                       # Video assets folder
│   ├── .gitkeep                 # Keeps folder in Git
│   └── (your-videos.mp4)        # Add your animation files here
└── docs/                         # Documentation folder
    ├── executive-email-template.md   # Email templates for executives
    └── job-application-questions.md  # Original Q&A responses
```

## Tips

- **Video Optimization:** Compress videos for web (use HandBrake or similar) to ensure fast loading
- **SEO:** The site is basic HTML/CSS - no build process needed
- **Mobile Responsive:** Permanent layout adapts to mobile usage
- **Print Styling:** PDFs are optimized for standard 8.5" x 11" pages

## Next Steps

1. ✅ Add your videos to the portfolio
2. ✅ Deploy to GitHub Pages
3. ✅ Generate PDF versions of resume and cover letter
4. ✅ Update and send executive emails
5. ✅ Submit application with portfolio link

Good luck with your application! 🚀


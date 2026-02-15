# Screenshot Guide for DriftIQ

This guide will help you take actual screenshots to replace the placeholder images.

## Required Screenshots

### 1. banner.png (1200x300px)
**What to capture:**
- A visually appealing banner/hero image
- Should include the DriftIQ logo/name prominently
- Recommended: Full application view or stylized graphic

**How to capture:**
- Open [diff-viewer.html](../diff-viewer.html) in your browser
- Take a wide screenshot of the top section
- Crop to 1200x300px
- Save as `screenshots/banner.png`

---

### 2. main-interface.png (1200x800px recommended)
**What to capture:**
- The main DriftIQ interface before computing a diff
- Should show:
  - Pre-Configuration text area with "Browse" button
  - Post-Configuration text area with "Browse" button
  - "Compute Diff" button
  - Pattern replacement section
  - Ignore rules section

**How to capture:**
1. Open [diff-viewer.html](../diff-viewer.html)
2. Don't load any files yet (or load sample files)
3. Take a full-page screenshot
4. Crop to show the entire interface cleanly
5. Save as `screenshots/main-interface.png`

---

### 3. diff-view.png (1200x800px recommended)
**What to capture:**
- Side-by-side diff comparison view
- Should show:
  - Pre-configuration on the left
  - Post-configuration on the right
  - Color-coded differences (green for additions, red for deletions, yellow for modifications)
  - Command headers if using command-based format
  - Line numbers

**How to capture:**
1. Open [diff-viewer.html](../diff-viewer.html)
2. Load [example-pre-config.txt](../examples/example-pre-config.txt) and [example-post-config.txt](../examples/example-post-config.txt)
3. Click "Compute Diff"
4. Scroll to show interesting differences
5. Take a screenshot showing the diff view
6. Save as `screenshots/diff-view.png`

---

### 4. pattern-rules.png (1200x600px recommended)
**What to capture:**
- Pattern replacement rules section
- Should show:
  - Both "General Patterns" and "Column-Based" sections
  - At least 2-3 example rules configured
  - The "Session" vs "Permanent" toggle
  - Add/delete buttons

**How to capture:**
1. Open [diff-viewer.html](../diff-viewer.html)
2. Scroll to the "Pattern Replacement" section
3. Add a few example rules:
   - Pattern: `uptime.*` → Replacement: `[MASKED]`
   - Pattern: `\d{4}-\d{2}-\d{2}` → Replacement: `[DATE]`
   - Column rule for command: `show interfaces status`, Column: 2
4. Take a screenshot of this section
5. Save as `screenshots/pattern-rules.png`

---

### 5. ignore-rules.png (1200x600px recommended)
**What to capture:**
- Ignore lines and ignore commands sections
- Should show:
  - List of ignored line patterns
  - List of ignored commands
  - "Show Ignored Lines" toggle button
  - Example of how ignored content appears (if toggle is on)

**How to capture:**
1. Open [diff-viewer.html](../diff-viewer.html)
2. Load sample files and compute diff
3. Add some ignore rules:
   - Click on line numbers to ignore specific lines
   - Click "Ignore Command" on some commands
4. Scroll to show the ignore rules section
5. Take a screenshot
6. Save as `screenshots/ignore-rules.png`

---

### 6. html-report.png (1200x800px recommended)
**What to capture:**
- An exported HTML report opened in a browser
- Should show:
  - The report header/title
  - Side-by-side diff view in the report
  - Clean, professional appearance

**How to capture:**
1. Open [diff-viewer.html](../diff-viewer.html)
2. Load sample files and compute diff
3. Click "Export HTML Report"
4. Save the exported HTML file
5. Open the exported HTML in a new browser window
6. Take a screenshot of the opened report
7. Save as `screenshots/html-report.png`

---

## Screenshot Tips

### General Guidelines:
- Use a clean, modern browser (Chrome or Firefox recommended)
- Set browser zoom to 100%
- Use a resolution of at least 1920x1080 for clarity
- Take screenshots in light mode for consistency
- Crop screenshots to remove browser chrome (address bar, tabs) unless needed
- Ensure text is readable at the final size

### Recommended Tools:
- **Windows**: Snipping Tool, Snip & Sketch, or ShareX
- **Mac**: Command+Shift+4 for selection, Command+Shift+3 for full screen
- **Cross-platform**: LightShot, Greenshot, or browser extensions

### Image Formats:
- PNG is recommended for screenshots (lossless, supports transparency)
- Keep file size reasonable (under 500KB per image)
- Use compression tools like TinyPNG if files are too large

### File Naming:
- Use exact names as listed above
- All lowercase
- Use hyphens, not underscores
- Save in the `screenshots/` directory

---

## Quick Checklist

- [ ] banner.png - Main banner/hero image
- [ ] main-interface.png - Main application interface
- [ ] diff-view.png - Side-by-side diff comparison
- [ ] pattern-rules.png - Pattern replacement section
- [ ] ignore-rules.png - Ignore rules section
- [ ] html-report.png - Exported HTML report

---

## After Taking Screenshots

1. Replace the placeholder SVG files in `screenshots/` directory
2. Verify images display correctly in README.md locally
3. Commit and push to GitHub:
   ```bash
   git add screenshots/
   git commit -m "Add actual screenshots to documentation"
   git push
   ```
4. Check your GitHub repository to ensure images load properly

---

## Need Help?

If you're having trouble with any screenshots:
1. Make sure the application is working correctly
2. Try different browser zoom levels (90%, 100%, 110%)
3. Consider using browser developer tools to adjust the view
4. Use image editing software to crop and resize as needed

# Static Site for wmcarlson.com

This is a standalone HTML file that can be uploaded directly to your web hosting.

## What's Included

- **index.html** - Complete standalone HTML file with:
  - All CSS embedded
  - About/overview content
  - No case studies or work examples
  - Responsive design
  - Same design system as your portfolio

## How to Upload

1. **Upload the file**: Upload `index.html` to your web hosting's root directory (usually `public_html` or `www`)

2. **Rename if needed**: 
   - If your host requires a specific filename, you may need to rename it
   - Most hosts will serve `index.html` as the default page

3. **Update contact email**: 
   - Search for `your-email@example.com` in the file and replace with your actual email

4. **Optional - Add favicon**: 
   - If you have a favicon.svg file, upload it to the same directory
   - Or remove the favicon link from the `<head>` section

## File Structure

```
static-site/
  ├── index.html    (main file - upload this)
  └── README.md     (this file - for reference only)
```

## Customization

The file is self-contained with all styles embedded. To customize:

- **Colors**: Edit the CSS variables in the `<style>` section (look for `:root {`)
- **Content**: Edit the HTML content in the `<main>` section
- **Social Links**: Update the URLs in the footer section
- **Copyright**: Update the year in the footer (currently shows 2024)

## Notes

- This is a single-page site with no dependencies
- All fonts are loaded from Google Fonts (requires internet connection)
- The design automatically adapts to light/dark mode based on user preference
- Fully responsive for mobile, tablet, and desktop


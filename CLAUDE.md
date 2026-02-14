# CLAUDE.md

This file provides guidance for AI assistants working on the **emailcode** repository.

## Project Overview

This repository contains HTML email templates designed for **Klaviyo** (email marketing platform). The templates are for **WLOOM Brand**, a pet products e-commerce store. Templates are standalone HTML files with inline CSS, optimized for email client compatibility and mobile responsiveness.

## Repository Structure

```
emailcode/
  CLAUDE.md            # AI assistant guidance (this file)
  email-template.html  # Klaviyo-ready product launch email template
```

## Key Files

| Path | Purpose |
|------|---------|
| `CLAUDE.md` | AI assistant guidance (this file) |
| `email-template.html` | Product launch email for Klaviyo — presents Ducky, Rex, and Power Ball 2.0 |

## Technical Details

### Email Template Conventions

- **Pure HTML + inline CSS** — no external stylesheets, no JavaScript
- **Table-based layout** for maximum email client compatibility
- MSO (Microsoft Outlook) conditional comments for Outlook rendering
- VML roundrect buttons as Outlook fallback for border-radius CTAs
- Responsive via `@media` queries at 620px breakpoint
- Klaviyo merge tags for unsubscribe: `{% unsubscribe_url %}`
- All images use absolute URLs from the WLOOM CDN (`wloombrand.com/cdn/shop/files/...`)

### Brand Guidelines

- **Primary color**: `#2F7D68` (teal green)
- **Accent/free color**: `#E8A838` (gold/amber)
- **Sale/urgency color**: `#D94F4F` (red)
- **Heading font**: Georgia, 'Times New Roman', serif
- **Body font**: 'Helvetica Neue', Helvetica, Arial, sans-serif
- **Tone**: Professional, conversion-focused, Italian language
- **Style**: Clean, modern pet store branding

### Testing

To preview templates:
1. Open the `.html` file in a browser for a quick visual check
2. Use [Litmus](https://litmus.com) or [Email on Acid](https://emailonacid.com) for cross-client testing
3. Paste into Klaviyo's code editor and use Klaviyo's preview/test send feature

### Conventions to Follow

- **Commits**: Use clear, descriptive commit messages with conventional commit format (`feat:`, `fix:`, `docs:`)
- **Branching**: Development branches follow the pattern `claude/<description>`
- **Images**: Always use absolute HTTPS URLs; never embed base64 images
- **Responsiveness**: Test all templates on mobile viewports (320px–414px)
- **Accessibility**: Include alt text on all images; maintain sufficient color contrast
- **Outlook compatibility**: Always include MSO conditional blocks for buttons and layout

## Maintenance

Keep this file up to date as the project evolves:

- Add new template files to the Key Files table
- Document any new Klaviyo merge tags or dynamic blocks used
- Update brand guidelines if colors or fonts change

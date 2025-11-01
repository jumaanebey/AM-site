# AM Executive Coaching Website - Development Notes

## Project Overview
Executive coaching website for Amelia Norvell, codename "AM" for launch. Professional, elegant design with minimalist aesthetic.

**Live Site:** https://am-coaching.vercel.app
**Repository:** https://github.com/jumaanebey/AM-site

## Recent Work Session (2025-11-01)

### Typography & Design Refinements

1. **Footer Background Fix**
   - Issue: Footer background didn't match hero section gradient
   - Solution: Applied same gradient to footer: `linear-gradient(135deg, var(--white) 0%, var(--light-gray) 100%)`
   - This creates seamless color transition from hero to footer

2. **Footer Text Color**
   - Changed footer text from `--medium-text` to `--dark-text` to match body text
   - More cohesive, professional appearance

3. **H1 Typography Standardization**
   - Applied Cormorant Garamond h1 styling from index.html to all pages
   - Font: 'Cormorant Garamond', serif
   - Weight: 300 (thin, elegant)
   - Size: clamp(3rem, 8vw, 5.5rem)
   - All page headers now consistent across site

4. **Footer Font Size Optimization**
   - Final size: **0.8rem** (found sweet spot after multiple iterations)
   - Overrides global `p` tag styling via `footer p` selector
   - Both footer lines now use same size (removed inline style override)

## Design System

### Color Palette
```css
--pine-green: #647A6D;
--gold-accent: #B38600;
--warm-gray: #E8E4E0;
--light-gray: #F7F5F3;
--white: #FFFFFF;
--dark-text: #2A2A2A;
--medium-text: #5A5A5A;
```

### Typography Stack
- **H1 Headers:** Cormorant Garamond (serif, weight 300)
- **H2-H4 Headers:** Montserrat (sans-serif, weight 300)
- **Body Text:** Inter (sans-serif, weight 300)
- **Footer:** 0.8rem

### Key Styling Decisions
- **Header Border:** Opacity set to 0 (invisible)
- **Footer Separator Line:** Dark line with 5% left/right buffer (doesn't touch edges)
- **Background Gradient:** 135deg diagonal from white to light-gray
- **Font Weights:** Consistently using weight 300 for refined, elegant appearance

## Site Structure
- index.html - Home page
- about.html - About/credentials
- services.html - 2025 service offerings (corporate & private clients)
- approach.html - Coaching methodology
- testimonials.html - Client testimonials
- contact.html - Contact form

## Technical Notes

### Deployment
- Hosted on Vercel
- Auto-deploys on git push to main branch
- Use: `git add -A && git commit -m "message" && git push`

### Common Issues & Solutions

**Issue:** Global `p` tag styles override footer
**Solution:** Use `footer p` selector with specific font-size

**Issue:** Inline styles in HTML
**Solution:** Remove and control via CSS for consistency

**Issue:** Gradient backgrounds not matching between sections
**Solution:** Use exact same gradient values and angles

## Current State
✅ All typography consistent across pages
✅ Footer blends seamlessly with hero section
✅ Clean, professional footer at optimal size
✅ All changes deployed to production

## Next Steps / Considerations
- Footer text is finalized at 0.8rem (good balance)
- All pages have consistent Cormorant Garamond h1 headers
- Design system is stable and ready for content updates

## Important: Codename
Website uses "AM" codename throughout instead of full name "Amelia Norvell". This is intentional for launch.

# Liquid Legacy Integrative Wellness - Landing Page

A lightweight, static HTML/CSS placeholder landing page for Liquid Legacy Integrative Wellness.

**Live Site**: https://liquidlegacy-landing.pages.dev/

## Overview

This is a minimal, single-page website designed to establish an online presence while the full website is under development. The page follows the brand style guide and provides essential information about services and contact details.

### What's Included

- ✅ Responsive, mobile-first design
- ✅ Integrated booking system (Hydreight)
- ✅ Service cards with benefit-focused icons
- ✅ Adaptive favicons (light/dark mode)
- ✅ Brand-compliant color scheme and typography
- ✅ Smooth hover animations and transitions
- ✅ Contact information layout
- ✅ SEO-optimized HTML structure

### Pending Client Input

- Hours of operation verification
- Phone number
- Physical address
- Google Maps directions link

## Design Features

- **Uplifting Wellness Aesthetic**: Warm, inviting design with flowing water-inspired elements
- **Dynamic Background**: Multi-layered background with:
  - Flowing wave SVG patterns (water/wellness theme)
  - Soft blue gradient wash
  - Radial gradient decorative elements (mountains/droplets)
- **Brand Logo**: Official SVG logo with enhanced brand blue tones and subtle drop shadow
- **Favicons**: Adaptive favicons (light/dark) based on system color scheme preference
- **Brand Colors**: Deep Blue (#00008B) and Royal Blue (#3333A2) gradients throughout
- **Enhanced Typography**:
  - Abhaya Libre ExtraBold (800) for impactful headings
  - Decorative accent line under hero headline
  - Inter for body text with improved hierarchy
  - Fluid type scaling for all screen sizes
- **Interactive Elements**:
  - Gradient button with inverted hover state (white bg, blue border, blue text)
  - Integrated booking system link (opens in new tab)
  - Service cards with subtle border transitions
  - Benefit-focused Iconify icons with lift animation
  - Card hover states (lift + border color change + shadow)
  - Smooth transform and color transitions throughout
- **Service Cards**:
  - Ultra-minimal transparent cards with barely-visible borders
  - Very subtle border (15% opacity) that appears on hover
  - Compact spacing between and inside cards
  - Equal width cards on desktop (using CSS grid minmax)
  - Benefit-focused icons (hydration, energy, vitality)
  - Brand blue color scheme: text and icons in deep blue (color-primary)
  - Bold text (700 weight) for strong readability
  - Hover effects: card lifts, border intensifies, icon changes to royal blue and floats up
  - Responsive grid (1 column mobile, 3 equal columns desktop)
  - Icons sized at 40px for visual clarity
- **Contact Section**:
  - Clean 3-column grid: Hours | Contact | Location
  - Each column has label on one line, details on separate lines below
  - Left-aligned text for easy scanning
  - Responsive: stacks vertically on mobile, 3 columns on desktop
  - Simple, organized information display
- **Center-Justified Layout**: Single-column design with dynamic spacing
- **Fully Responsive**: Mobile-first design that works beautifully on all devices
- **Accessibility**: WCAG 2.1 AA compliant with proper contrast, focus states, and semantic HTML

## Files

```
├── index.html        # Main HTML structure
├── styles.css        # Complete styling system
├── docs/             # Brand and copy guidelines
│   ├── brand-style-guide.md
│   └── copy-placeholder-page.md
└── images/           # Logo and favicon assets
    ├── LiquidLegacy_Logo.svg
    ├── favicon_light.svg
    └── favicon_dark.svg
```

## Client Information Needed

The following information needs to be verified/updated by the client:

1. **Booking System** ✅ CONFIGURED:
   - Currently links to: `https://booking.hydreight.com/widget-business/mq46k`
   - Opens in new tab with security attributes

2. **Hours of Operation** (around line 71):
   - Currently shows: "Mon & Wed 9am-4pm"
   - Verify if correct or update as needed

3. **Phone Number** (around line 76-77):
   - Replace `(XXX) XXX-XXXX` in two places:
     - `<a href="tel:+1234567890">` - update the tel: link
     - Phone number display text

4. **Street Address** (around line 81):
   - Replace `[Street Address, City, State]` with actual address

5. **Directions Link** (around line 81):
   - Update `href="#"` with Google Maps URL for the location

**Note**: Line numbers are approximate and may shift as content is edited.

## Optional Enhancements

### Favicons
The site includes adaptive favicons that respond to system color scheme:
- **Light mode**: Uses `favicon_light.svg`
- **Dark mode**: Uses `favicon_dark.svg`
- Automatically switches based on user's system preferences
- SVG format for crisp display at any size

### Customize Background Elements
The background uses multiple layers for visual depth. To adjust:

**Wave Patterns** (`.background-pattern` in `styles.css`, around line 134):
- Adjust wave stroke opacity (currently 0.05-0.08)
- Change wave path positions for different flow patterns
- Modify colors using the color variables

**Gradient Elements**:
- Radial gradients create soft decorative elements (mountains/droplets)
- Adjust position percentages to move elements
- Change sizes (in pixels) for more/less prominence

**Color Intensity**:
- The gradient wash uses very light blues (98% lightness)
- Increase saturation or decrease lightness for bolder colors
- Swap color stops for different gradient directions

### Adjust Interactive Effects
- **Button hover effects**: Clean inversion - gradient fills to white background with blue border and text. Edit `.btn-primary:hover` to adjust.
- Service card borders: Modify border opacity/color in `.service-card` (default: `hsla(240, 100%, 75%, 0.15)` - 15% opacity)
- Card hover states: Adjust transform, border color, and shadow in `.service-card:hover`
- Icon animations: Change lift distance in `.service-card:hover .service-icon`
- Icon/text colors: Currently deep blue (`--color-primary`), hover changes icon to royal blue (`--color-accent`)
- Text weight: Currently 700 (bold) - adjust in `.service-name`
- Border radius: Adjust `border-radius: 1rem` for more/less rounded corners
- Border visibility: Increase opacity (0.15 → 0.3) for more visible borders, decrease (0.15 → 0.08) for nearly invisible
- Spacing: Adjust gaps in `.services-grid` (currently `--space-md`) and padding in `.service-card`

### Change Service Icons
Icons are powered by [Iconify](https://icon-sets.iconify.design/). To change icons:

1. Browse icon sets at https://icon-sets.iconify.design/
2. Search for health/medical/wellness icons
3. Copy the icon name (e.g., `healthicons:injecting`)
4. Replace in HTML: `data-icon="icon-set:icon-name"`

**Current icons** (benefit-focused):
- **IV Hydration Therapy**: `mdi:water-outline` (hydration, refreshment, restoration)
- **B-12 MICC Shots**: `tabler:bolt` (energy boost, vitality, power)
- **Weight Loss Injections**: `healthicons:exercise-running` (active lifestyle, wellness, movement)

**Icon Philosophy**:
Icons represent the *benefit* to the recipient (energy, vitality, rejuvenation) rather than the clinical procedure itself. This creates a more positive, aspirational connection.

**Alternative benefit-focused icons**:
- `lucide:sparkles` (vitality, feeling great)
- `carbon:energy` (energy boost)
- `ph:heart-straight` (wellness, health)
- `tabler:refresh` (rejuvenation)
- `fluent:weather-sunny-20-regular` (brightness, positivity)

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile Safari (iOS 12+)
- Chrome for Android
- Degrades gracefully in older browsers

## Performance & Dependencies

- **Minimal JavaScript**: Only Iconify (16KB) for icon rendering
- **Font Loading**: Uses font-display: swap for optimal web font loading
- **External Dependencies**:
  - Google Fonts CDN for typography (Abhaya Libre, Inter)
  - Iconify CDN for icons (3.1.0)
- **CSS Animations**: Hardware-accelerated transforms for smooth performance
- **SVG Patterns**: Inline SVG data URIs for no additional HTTP requests
- **Lightweight**: Total page weight < 80KB (excluding fonts)
- **Optimizations**:
  - Backdrop filters use GPU acceleration
  - Reduced motion preferences respected
  - Efficient gradients and transitions
  - Lazy icon loading via Iconify

## Deployment

This is a static site and can be hosted anywhere:
- Upload files to any web server
- Deploy to Netlify, Vercel, or GitHub Pages
- Use with any hosting provider

## Future Development

This placeholder can remain active while the full website is developed. Key sections to add later:
- Detailed service pages
- Online booking system integration
- Photo gallery
- Client testimonials
- Team/about page
- Blog or resources section

## Support

For questions or modifications, contact your development team.

---

**Status**: Deployed - Awaiting client information
**Design Version**: 2.6 (Final with smooth button transitions)
**Deployment**: https://liquidlegacy-landing.pages.dev/
**Repository**: https://github.com/hovingadesign/liquidlegacy_landing
**Last Updated**: 2025-12-01
**Brand Guide Version**: 1.0

## Deployment

The landing page is currently deployed on Cloudflare Pages:
- **Live URL**: https://liquidlegacy-landing.pages.dev/
- **Auto-deploy**: Enabled on push to `main` branch
- **Status**: Awaiting client verification of hours, phone, and address information

## Icon Credits
Icons provided by [Iconify](https://iconify.design/) using various open-source icon sets including HealthIcons and Medical Icons.

---

## Development Notes

### Completed Features (2025-12-01)

✅ **Design & Layout**
- Uplifting wellness-focused aesthetic with flowing water patterns
- Multi-layer background (waves, gradients, decorative elements)
- Responsive mobile-first layout
- Compact service cards with benefit-focused icons
- Structured contact section with left-aligned text

✅ **Interactive Elements**
- Smooth button hover transition (gradient to ghost button effect)
- Service card hover states with icon color changes
- Adaptive favicon system (light/dark mode)

✅ **Integration**
- Hydreight booking system linked
- All external links open in new tabs with security attributes
- SEO meta tags configured

✅ **Technical**
- Pure HTML/CSS (minimal JavaScript - only Iconify for icons)
- Git repository initialized and pushed to GitHub
- Deployed to Cloudflare Pages with auto-deploy

### Next Steps

1. **Client Review**: Awaiting verification of hours, phone number, and address
2. **Squarespace Access**: Needed to deploy to production domain
3. **Final Updates**: Once client provides information, update and redeploy
4. **Full Site Development**: Begin after landing page goes live

### Known Placeholders

- `(XXX) XXX-XXXX` - Phone number
- `[Street Address, City, State]` - Physical address
- Hours may need verification
- Directions link needs Google Maps URL

### Repository Structure

```
main branch (auto-deploys to Cloudflare Pages)
├── Latest commit: "Remove privacy policy and terms links from footer"
└── 16 files tracked (HTML, CSS, docs, images, references)
```

---

**Project Contact**: Nate Hovinga | HovingaDesign
**Client**: Liquid Legacy Integrative Wellness

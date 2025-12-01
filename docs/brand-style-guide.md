# Brand Style Guide: Liquid Legacy Integrative Wellness

**Version**: 1.0
**Last Updated**: 2025-11-26
**Purpose**: Web design system and brand standards

---

## 1. BRAND OVERVIEW

### Brand Essence
Professional wellness care delivered by registered nurses. The brand balances clinical expertise with natural, restorative imagery—evoking the flow of water (liquid) and the building of lasting relationships (legacy).

### Visual Themes
- **Nature**: Mountains, waterfalls, flowing water
- **Clinical**: Professional, trustworthy, medical-grade
- **Restorative**: Calming, peaceful, rejuvenating
- **Accessible**: Approachable, warm, human-centered

---

## 2. COLOR SYSTEM

### Color Philosophy
Following modern design system principles, colors are organized using **HSL format** for maximum flexibility and maintainability. The palette uses **semantic naming** rather than descriptive color names.

### Primary Brand Colors

```css
/* Brand Colors - Core Palette */
--color-brand-deep-blue: hsl(240, 100%, 27%);     /* #00008B */
--color-brand-royal-blue: hsl(240, 60%, 42%);     /* #3333A2 */
--color-brand-black: hsl(0, 0%, 0%);              /* #000000 */
```

### Extended Color Scale

Based on the supplied palette with tints at 70%, 50%, and 25%:

```css
/* Deep Blue Scale */
--color-blue-900: hsl(240, 100%, 27%);   /* #00008B - Primary */
--color-blue-700: hsl(240, 100%, 40%);   /* 70% tint */
--color-blue-500: hsl(240, 100%, 55%);   /* 50% tint */
--color-blue-300: hsl(240, 100%, 75%);   /* 25% tint */
--color-blue-100: hsl(240, 100%, 95%);   /* Very light */

/* Royal Blue Scale */
--color-purple-900: hsl(240, 60%, 42%);  /* #3333A2 - Secondary */
--color-purple-700: hsl(240, 60%, 55%);  /* 70% tint */
--color-purple-500: hsl(240, 60%, 70%);  /* 50% tint */
--color-purple-300: hsl(240, 60%, 85%);  /* 25% tint */
--color-purple-100: hsl(240, 60%, 96%);  /* Very light */

/* Neutral Scale (from black base) */
--color-neutral-900: hsl(0, 0%, 10%);    /* Near black */
--color-neutral-800: hsl(0, 0%, 20%);    /* Dark gray */
--color-neutral-700: hsl(0, 0%, 35%);    /* Medium-dark */
--color-neutral-600: hsl(0, 0%, 50%);    /* Medium */
--color-neutral-500: hsl(0, 0%, 62%);    /* Medium-light */
--color-neutral-400: hsl(0, 0%, 75%);    /* Light gray */
--color-neutral-300: hsl(0, 0%, 85%);    /* Lighter */
--color-neutral-200: hsl(0, 0%, 92%);    /* Very light */
--color-neutral-100: hsl(0, 0%, 97%);    /* Off-white */
--color-neutral-50: hsl(0, 0%, 99%);     /* Near white */
```

### Semantic Color Tokens

Following Sajid's approach, colors are assigned **functional roles**:

```css
/* Background Colors */
--color-bg-primary: hsl(0, 0%, 100%);         /* White */
--color-bg-secondary: hsl(0, 0%, 97%);        /* Off-white */
--color-bg-tertiary: hsl(240, 100%, 95%);     /* Light blue tint */
--color-bg-dark: hsl(240, 100%, 27%);         /* Deep blue */

/* Text Colors */
--color-text-primary: hsl(0, 0%, 10%);        /* Near black */
--color-text-secondary: hsl(0, 0%, 35%);      /* Medium-dark gray */
--color-text-muted: hsl(0, 0%, 50%);          /* Medium gray */
--color-text-inverse: hsl(0, 0%, 100%);       /* White on dark */

/* Interactive/Action Colors */
--color-primary: hsl(240, 100%, 27%);         /* Deep blue - main CTA */
--color-primary-hover: hsl(240, 100%, 35%);   /* Lighter on hover */
--color-secondary: hsl(240, 60%, 42%);        /* Royal blue - secondary CTA */
--color-secondary-hover: hsl(240, 60%, 50%);  /* Lighter on hover */

/* Accent/Emphasis */
--color-accent: hsl(240, 60%, 42%);           /* Royal blue */
--color-highlight: hsl(240, 100%, 95%);       /* Light blue background */

/* Borders */
--color-border: hsl(0, 0%, 85%);              /* Light gray */
--color-border-muted: hsl(0, 0%, 92%);        /* Very light gray */
--color-border-focus: hsl(240, 100%, 27%);    /* Deep blue for focus states */

/* Feedback/Status Colors (if needed) */
--color-success: hsl(140, 60%, 45%);          /* Green */
--color-warning: hsl(40, 95%, 55%);           /* Amber */
--color-danger: hsl(0, 70%, 50%);             /* Red */
--color-info: hsl(200, 80%, 50%);             /* Light blue */
```

### Color Usage Guidelines

**Primary Deep Blue (#00008B)**
- Use for: Primary CTAs, headings, logo text, emphasis
- Don't use: Large background areas (too intense), long body text (low readability)
- Pairs well with: White, off-white, light gray backgrounds

**Royal Blue (#3333A2)**
- Use for: Secondary CTAs, accents, icons, subheadings
- Don't use: Primary navigation if deep blue is already prominent
- Pairs well with: White, light blue tints

**Black & Neutrals**
- Use for: Body text, borders, subtle backgrounds
- Don't use: Pure black (#000000) for text—use neutral-900 instead for better readability
- Pairs well with: All brand colors

**Light Tints**
- Use for: Backgrounds, hover states, subtle emphasis
- Don't use: Text (insufficient contrast)
- Pairs well with: Dark text, deep blue accents

### Accessibility Requirements

All text/background combinations must meet **WCAG 2.1 AA standards**:
- Normal text: Minimum 4.5:1 contrast ratio
- Large text (18px+ or 14px+ bold): Minimum 3:1 contrast ratio

**Approved Combinations**:
- Deep blue text (#00008B) on white: ✓ Passes AA
- White text on deep blue background: ✓ Passes AA
- Neutral-900 text on white: ✓ Passes AAA
- Royal blue (#3333A2) on white: ✓ Passes AA

---

## 3. TYPOGRAPHY

### Font Philosophy
Combine the professionalism of the logo's serif typeface with modern, readable sans-serif for body content. Balance clinical credibility with approachable warmth.

### Font Families

#### Primary Typeface: Abhaya Libre
**Use**: Headings, logo lockup, emphasis

```css
font-family: 'Abhaya Libre', serif;
```

**Weights Available**:
- Regular (400)
- Medium (500) - Used in logo
- SemiBold (600)
- Bold (700)
- ExtraBold (800)

**Character**: Professional, elegant, readable. Slightly traditional feel that conveys expertise and trustworthiness. The logo uses **Medium (500)**.

**Where to use**:
- H1, H2, H3 headings
- Hero headlines
- Section titles
- Pull quotes
- Taglines

---

#### Secondary Typeface: Inter
**Use**: Body text, UI elements, navigation

```css
font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

**Weights Available**:
- Regular (400) - Body text
- Medium (500) - Emphasis, labels
- SemiBold (600) - Subheadings, buttons
- Bold (700) - Strong emphasis

**Character**: Clean, modern, highly readable. Optimized for screen reading. Neutral and professional without being sterile.

**Where to use**:
- Body copy
- Navigation menus
- Buttons and CTAs
- Form labels and inputs
- Captions and metadata
- UI components

---

### Typography Scale

Following modern responsive design principles with a **fluid type scale**:

```css
/* Base Configuration */
--font-size-base: 16px;  /* Root size - never smaller */
--line-height-base: 1.6;

/* Heading Scale */
--font-size-h1: clamp(2.5rem, 5vw, 3.5rem);    /* 40px - 56px */
--font-size-h2: clamp(2rem, 4vw, 2.75rem);     /* 32px - 44px */
--font-size-h3: clamp(1.5rem, 3vw, 2rem);      /* 24px - 32px */
--font-size-h4: clamp(1.25rem, 2.5vw, 1.5rem); /* 20px - 24px */
--font-size-h5: 1.125rem;                       /* 18px */
--font-size-h6: 1rem;                           /* 16px */

/* Body Text Scale */
--font-size-xl: 1.25rem;    /* 20px - Large body text */
--font-size-lg: 1.125rem;   /* 18px - Subheadings, leads */
--font-size-base: 1rem;     /* 16px - Standard body */
--font-size-sm: 0.875rem;   /* 14px - Small text, captions */
--font-size-xs: 0.75rem;    /* 12px - Fine print, labels */

/* Line Heights */
--line-height-tight: 1.2;   /* Headings */
--line-height-normal: 1.5;  /* UI elements */
--line-height-relaxed: 1.6; /* Body text */
--line-height-loose: 1.8;   /* Long-form content */
```

### Typography Styles

#### Headings

```css
h1, .h1 {
  font-family: 'Abhaya Libre', serif;
  font-size: var(--font-size-h1);
  font-weight: 700;
  line-height: var(--line-height-tight);
  color: var(--color-text-primary);
  margin-bottom: 1rem;
}

h2, .h2 {
  font-family: 'Abhaya Libre', serif;
  font-size: var(--font-size-h2);
  font-weight: 600;
  line-height: var(--line-height-tight);
  color: var(--color-text-primary);
  margin-bottom: 0.875rem;
}

h3, .h3 {
  font-family: 'Abhaya Libre', serif;
  font-size: var(--font-size-h3);
  font-weight: 600;
  line-height: 1.3;
  color: var(--color-text-primary);
  margin-bottom: 0.75rem;
}

h4, .h4 {
  font-family: 'Inter', sans-serif;
  font-size: var(--font-size-h4);
  font-weight: 600;
  line-height: 1.4;
  color: var(--color-text-primary);
  margin-bottom: 0.625rem;
}
```

#### Body Text

```css
body {
  font-family: 'Inter', sans-serif;
  font-size: var(--font-size-base);
  font-weight: 400;
  line-height: var(--line-height-relaxed);
  color: var(--color-text-primary);
}

.lead {
  font-size: var(--font-size-lg);
  line-height: var(--line-height-loose);
  color: var(--color-text-secondary);
}

.small, small {
  font-size: var(--font-size-sm);
  line-height: var(--line-height-normal);
}

strong, b {
  font-weight: 600;
}
```

#### Special Text Styles

```css
/* Hero Headline */
.hero-headline {
  font-family: 'Abhaya Libre', serif;
  font-size: clamp(2.5rem, 6vw, 4rem);
  font-weight: 700;
  line-height: 1.1;
  color: var(--color-primary);
}

/* Subheadline */
.subheadline {
  font-family: 'Inter', sans-serif;
  font-size: var(--font-size-lg);
  font-weight: 400;
  line-height: var(--line-height-loose);
  color: var(--color-text-secondary);
}

/* Tagline */
.tagline {
  font-family: 'Abhaya Libre', serif;
  font-size: var(--font-size-lg);
  font-weight: 500;
  font-style: italic;
  color: var(--color-accent);
}
```

### Font Loading

Use **font-display: swap** to prevent invisible text while fonts load:

```css
@font-face {
  font-family: 'Abhaya Libre';
  font-display: swap;
  /* font sources */
}

@font-face {
  font-family: 'Inter';
  font-display: swap;
  /* font sources */
}
```

### Typography Guidelines

**Do**:
- Use Abhaya Libre for headings to maintain brand connection to logo
- Use Inter for body text and UI for optimal readability
- Keep body text at minimum 16px on mobile
- Maintain consistent line-height (1.6) for readability
- Use font-weight 600 for emphasis instead of bold (700) in body text

**Don't**:
- Mix too many font weights (stick to 3-4)
- Use Abhaya Libre for long-form body text (readability issues)
- Go below 14px for any readable text
- Use all-caps for long passages
- Use pure black (#000) for text—use neutral-900 instead

---

## 4. SPACING SYSTEM

### Spacing Scale

Based on 8px base unit for consistent rhythm:

```css
--space-4xs: 0.125rem;  /* 2px */
--space-3xs: 0.25rem;   /* 4px */
--space-2xs: 0.5rem;    /* 8px */
--space-xs: 0.75rem;    /* 12px */
--space-sm: 1rem;       /* 16px */
--space-md: 1.5rem;     /* 24px */
--space-lg: 2rem;       /* 32px */
--space-xl: 3rem;       /* 48px */
--space-2xl: 4rem;      /* 64px */
--space-3xl: 6rem;      /* 96px */
--space-4xl: 8rem;      /* 128px */
```

### Usage Guidelines

- **Component padding**: `--space-md` (24px)
- **Section spacing**: `--space-2xl` to `--space-3xl` (64px - 96px)
- **Element margins**: `--space-sm` to `--space-lg` (16px - 32px)
- **Button padding**: `--space-xs` `--space-md` (12px 24px)

---

## 5. COMPONENTS

### Buttons

```css
/* Primary Button */
.btn-primary {
  font-family: 'Inter', sans-serif;
  font-size: var(--font-size-base);
  font-weight: 600;
  color: var(--color-text-inverse);
  background-color: var(--color-primary);
  padding: 0.75rem 2rem;
  border: none;
  border-radius: 0.375rem;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.btn-primary:hover {
  background-color: var(--color-primary-hover);
}

/* Secondary Button */
.btn-secondary {
  font-family: 'Inter', sans-serif;
  font-size: var(--font-size-base);
  font-weight: 600;
  color: var(--color-primary);
  background-color: transparent;
  padding: 0.75rem 2rem;
  border: 2px solid var(--color-primary);
  border-radius: 0.375rem;
  cursor: pointer;
  transition: all 0.2s ease;
}

.btn-secondary:hover {
  background-color: var(--color-primary);
  color: var(--color-text-inverse);
}
```

### Links

```css
a {
  color: var(--color-primary);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: border-color 0.2s ease;
}

a:hover {
  border-bottom-color: var(--color-primary);
}
```

---

## 6. LOGO USAGE

### Logo Specifications

**Primary Logo**: Circular badge with mountain/waterfall illustration
- **Name**: LIQUID LEGACY (top arc)
- **Tagline**: INTEGRATIVE WELLNESS (bottom arc)
- **Typography**: Abhaya Libre Medium (500)
- **Colors**: Deep Blue (#00008B) and Royal Blue (#3333A2)

### Logo Variations

1. **Full Color** - Use on white or light backgrounds
2. **Reverse** - White logo on deep blue background
3. **Monochrome Black** - For black & white printing
4. **Monochrome White** - For dark backgrounds

### Clear Space

Maintain clear space equal to the height of the letter "L" in "LIQUID" around all sides of the logo.

### Minimum Size

- **Digital**: 120px diameter minimum
- **Print**: 1 inch diameter minimum

### Logo Don'ts

- Don't stretch or distort
- Don't change colors
- Don't add effects (drop shadow, gradient, etc.)
- Don't place on busy backgrounds
- Don't recreate or redraw

---

## 7. IMAGERY GUIDELINES

### Photography Style

**Preferred**:
- Natural, candid moments (not overly posed)
- Soft, natural lighting
- Clean, uncluttered backgrounds
- Focus on people feeling energized and vibrant
- Professional but warm tone

**Themes**:
- Healthcare professionals in action (RNs administering care)
- Clients relaxing during treatments
- Natural elements (water, mountains, nature)
- Active lifestyles (work, family, fitness)
- Before/after energy comparisons (subtle, not dramatic)

**Avoid**:
- Overly clinical/sterile hospital imagery
- Stock photo clichés (excessive smiling, unrealistic scenarios)
- Busy or chaotic backgrounds
- Poor lighting or low quality

### Color Grading

Photos should be:
- Slightly warm in tone (inviting, not cold)
- Natural color saturation (not oversaturated)
- Good contrast without being harsh
- Consistent with brand blue tones when applicable

---

## 8. IMPLEMENTATION

### CSS Custom Properties (Complete System)

```css
:root {
  /* Colors */
  --color-primary: hsl(240, 100%, 27%);
  --color-secondary: hsl(240, 60%, 42%);
  --color-text-primary: hsl(0, 0%, 10%);
  --color-bg-primary: hsl(0, 0%, 100%);

  /* Typography */
  --font-heading: 'Abhaya Libre', serif;
  --font-body: 'Inter', sans-serif;
  --font-size-base: 1rem;
  --line-height-base: 1.6;

  /* Spacing */
  --space-sm: 1rem;
  --space-md: 1.5rem;
  --space-lg: 2rem;

  /* Effects */
  --border-radius: 0.375rem;
  --transition-speed: 0.2s;
  --box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}
```

### Responsive Breakpoints

```css
/* Mobile First Approach */
--breakpoint-sm: 640px;   /* Small tablets */
--breakpoint-md: 768px;   /* Tablets */
--breakpoint-lg: 1024px;  /* Laptops */
--breakpoint-xl: 1280px;  /* Desktops */
--breakpoint-2xl: 1536px; /* Large screens */
```

---

## 9. ACCESSIBILITY

### Checklist

- ✓ All text meets WCAG AA contrast requirements
- ✓ Focus states visible on all interactive elements
- ✓ Touch targets minimum 44x44px
- ✓ Font sizes minimum 16px for body text
- ✓ Clear visual hierarchy
- ✓ Alt text for all images
- ✓ Semantic HTML structure
- ✓ Keyboard navigable

---

## 10. BRAND VOICE

While not visual, maintain consistency in messaging:

**Tone**: Professional but warm, empathetic but confident, educational but accessible

**Voice Attributes**:
- Knowledgeable (clinical expertise)
- Compassionate (understanding patient struggles)
- Direct (clear, no jargon)
- Empowering (helping people take control)

See `brandscript.md` for complete messaging framework.

---

## QUICK REFERENCE

### Essential Brand Elements

| Element | Specification |
|---------|--------------|
| Primary Color | Deep Blue `hsl(240, 100%, 27%)` #00008B |
| Secondary Color | Royal Blue `hsl(240, 60%, 42%)` #3333A2 |
| Heading Font | Abhaya Libre (500-700 weights) |
| Body Font | Inter (400-600 weights) |
| Base Font Size | 16px minimum |
| Line Height | 1.6 for body text |
| Primary CTA | Deep blue background, white text |
| Border Radius | 0.375rem (6px) |

---

**End of Brand Style Guide**

# Spygram — Website Specification

## 1. Project Overview

- **Project Name**: Spygram
- **Type**: Mobile app landing page (single-page website)
- **Core Functionality**: Landing page for an Instagram profile viewer/tracker app — showcasing features, app preview, and download CTA
- **Target Users**: Instagram users who want to view private profiles, track story viewers, and analyze engagement
- **Tech Stack**: Single HTML file with embedded CSS and vanilla JS

---

## 2. Visual & Rendering Specification

### Color Palette (from logo)
| Role | Color |
|------|-------|
| Background Dark | `#0A1128` |
| Background Card | `#111827` |
| Primary Blue | `#007BFF` |
| Accent Gradient Start | `#8B3DFF` (violet) |
| Accent Gradient Mid | `#FF3CAC` (magenta) |
| Accent Gradient End | `#FF8C42` (orange) |
| Text Primary | `#FFFFFF` |
| Text Secondary | `#94A3B8` |
| Border | `#1E293B` |

### Typography
- **Heading Font**: `Syne` (Google Fonts) — bold, geometric, techy
- **Body Font**: `DM Sans` (Google Fonts) — clean, modern

### Visual Style
- Dark cyberpunk/spy aesthetic
- Glowing neon effects on cards and buttons
- Gradient text for headings
- Glassmorphism cards with subtle backdrop blur
- Floating animated orbs in background for atmosphere

### Background
- Deep navy (`#0A1128`) base
- 2-3 large, blurred gradient orbs (purple/pink/orange) floating slowly with CSS animation
- Subtle grid pattern overlay (very faint)

---

## 3. Layout Structure

### Sections (top to bottom)

1. **Navbar**
   - Logo (SVG spy icon + "Spygram" text)
   - Nav links: Features, How It Works, Reviews, Download
   - CTA button: "Get Started"

2. **Hero Section**
   - Large heading with gradient text: "See Who's Watching Your Instagram"
   - Subheading explaining the app
   - Two CTA buttons: "Download App" (gradient) + "Learn More" (outline)
   - Phone mockup showing the app UI with floating cards

3. **Features Section**
   - Section title: "Powerful Instagram Insights"
   - 6 feature cards in a 3x2 grid:
     1. View Private Profiles — with lock icon
     2. Story Viewers Tracker — with eye icon
     3. Profile Visitors — with user icon
     4. Engagement Analytics — with chart icon
     5. Anonymous Browsing — with ghost icon
     6. DM Tracking — with message icon
   - Each card has glassmorphism style, icon, title, description

4. **How It Works Section**
   - 3-step horizontal timeline:
     1. "Install the App" — simple install
     2. "Connect Your Profile" — secure login
     3. "Unlock Insights" — get data
   - Connected by a gradient line

5. **App Preview Section**
   - Split layout: text left, phone mockup right
   - 3 mini feature highlights with icons
   - Animated phone showing app screenshots (carousel)

6. **Reviews / Testimonials Section**
   - Horizontal scrolling cards
   - User avatar, name, handle, star rating, quote

7. **Download CTA Section**
   - Large centered CTA
   - Gradient background section
   - App Store / Google Play buttons

8. **Footer**
   - Logo + tagline
   - Link columns: Product, Company, Legal
   - Social icons
   - Copyright

---

## 4. Interaction Specification

- **Scroll-triggered animations**: Sections fade/slide in as user scrolls (Intersection Observer)
- **Navbar**: Sticky, transparent → solid on scroll
- **Feature cards**: Hover glow effect (box-shadow with gradient)
- **CTA buttons**: Gradient shimmer animation on hover
- **Phone mockup**: Subtle floating animation (up/down)
- **Background orbs**: Slow drift animation (CSS keyframes)
- **Testimonials**: Horizontal auto-scroll (CSS animation)

---

## 5. Acceptance Criteria

- [ ] Navbar is sticky and changes background on scroll
- [ ] Hero section renders with gradient heading text
- [ ] All 6 feature cards are visible with correct icons
- [ ] "How It Works" shows 3 connected steps
- [ ] Phone mockup is visible in app preview section
- [ ] Testimonials auto-scroll horizontally
- [ ] Download CTA section has app store buttons
- [ ] Footer has all link columns
- [ ] All animations run smoothly (60fps)
- [ ] No layout overflow on mobile (responsive)
- [ ] Page loads without JS errors

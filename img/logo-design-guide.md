# CertifySphere Logo Design Guide

## Brand Identity
CertifySphere represents expertise, trust, and technological innovation in software consulting and product development.

## Logo Concept
- **Sphere**: Represents global reach, wholeness, and comprehensive solutions
- **Checkmark**: Symbolizes certification, quality, and trust
- **Badge**: Indicates credentials and professional achievement
- **Clean Typography**: Modern, professional, and accessible

## Color Palette
- **Primary (Light Mode)**: #264653 (Deep Teal) - Trust, stability, professionalism
- **Primary (Dark Mode)**: #3C6E71 (Lighter Teal) - Maintains visibility in dark theme
- **Secondary**: #2A9D8F (Seafoam Green) - Growth, innovation, harmony
- **Accent**: #E9C46A (Sandy Yellow) - Energy, optimism, creativity
- **Text Light**: #2D3748 - Primary readability
- **Text Dark**: #E2E8F0 - Dark mode readability

## Logo Variations & Usage

### 1. Primary Logo (`logo.svg` / `logo-dark.svg`)
- **Dimensions**: 120x40px (3:1 ratio)
- **Usage**: Main navbar, headers
- **Features**: Icon + company name + tagline

### 2. Icon Only (`logo-icon.svg` / `logo-icon-dark.svg`)
- **Dimensions**: 40x40px (1:1 ratio)
- **Usage**: Mobile navigation, app icons, favicons
- **Features**: Sphere with checkmark and badge only

### 3. Horizontal Layout (`logo-horizontal.svg`)
- **Dimensions**: 180x50px (3.6:1 ratio)
- **Usage**: Hero sections, large displays
- **Features**: Larger icon + full tagline

### 4. Stacked Layout (`logo-stacked.svg`)
- **Dimensions**: 120x60px (2:1 ratio)
- **Usage**: Square spaces, mobile apps
- **Features**: Icon above text

### 5. Banner (`certifysphere_banner_new.svg` / `certifysphere_banner_dark.svg`)
- **Dimensions**: 400x100px (4:1 ratio)
- **Usage**: Contact pages, social media, presentations
- **Features**: Large icon + decorative elements

## Responsive Specifications

### Desktop (1200px+)
- Navbar logo: 130x43px
- Clear visibility of all elements

### Tablet (769px - 1024px)
- Navbar logo: 110x37px
- Maintain proportions

### Mobile (≤768px)
- Navbar logo: 100x33px
- Consider icon-only version for very small spaces

## Technical Implementation

### CSS Classes
```css
.navbar__brand .navbar__logo {
  transition: all 0.3s ease;
}

.navbar__brand:hover .navbar__logo {
  transform: scale(1.05);
}
```

### Dark Mode Detection
```css
[data-theme='dark'] .navbar__logo img[src*="logo.svg"] {
  display: none;
}
[data-theme='dark'] .navbar__logo img[src*="logo-dark.svg"] {
  display: block;
}
```

### File Structure
```
static/img/
├── logo.svg (Primary light mode)
├── logo-dark.svg (Primary dark mode)
├── logo-icon.svg (Icon only light)
├── logo-icon-dark.svg (Icon only dark)
├── logo-horizontal.svg (Extended horizontal)
├── logo-stacked.svg (Vertical stack)
├── certifysphere_banner_new.svg (Banner light)
├── certifysphere_banner_dark.svg (Banner dark)
└── favicon.svg (32x32 simplified)
```

## Usage Guidelines

### DO:
- Use appropriate variation for context
- Maintain minimum size of 80px width for readability
- Ensure sufficient contrast with background
- Use SVG format for scalability
- Implement hover effects for interactive elements

### DON'T:
- Stretch or distort proportions
- Use low-resolution versions
- Place on busy backgrounds without contrast
- Modify colors outside brand palette
- Use outdated PNG versions when SVG is available

## Brand Applications

### Digital
- Website headers and navigation
- Social media profiles and posts
- Email signatures
- Digital presentations
- Mobile app icons

### Print
- Business cards (minimum 1 inch width)
- Letterhead and documents
- Marketing materials
- Signage and displays

## Accessibility
- High contrast ratios maintained (WCAG AA compliant)
- Scalable vector format ensures clarity at all sizes
- Alternative text: "CertifySphere Solutions Logo"
- Semantic markup for screen readers

## Future Considerations
- Animated versions for web (consider micro-interactions)
- Monochrome versions for single-color applications
- Simplified versions for very small displays (smartwatches, etc.)
- Print-optimized versions (CMYK color profiles)

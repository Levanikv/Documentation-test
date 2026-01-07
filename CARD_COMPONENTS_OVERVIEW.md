# Card Components Overview

This document provides a comprehensive overview of all card components in the AEM component library, generated from Figma using the Anova plugin.

## Table of Contents

1. [Basic Card Components](#basic-card-components)
2. [Editorial Cards](#editorial-cards)
3. [Offer Cards](#offer-cards)
4. [Card Containers](#card-containers)
5. [Specialized Cards](#specialized-cards)
6. [Common Features](#common-features)
7. [Breakpoints](#breakpoints)

---

## Basic Card Components

### 1. aem.card (v2.0)

**Purpose:** A flexible base card component for displaying content with optional media and actions.

**Key Features:**
- Title, subtitle, and description text fields
- Appendix support (icons or small media)
- Action button/link
- Configurable visibility for subtitle, description, and action
- Appendix positioning (left or top)

**Anatomy:**
- Root container
- Appendix (contentcardappendix instance)
- Texts container (title, subtitle, description)
- Action (contentcardaction instance)

**Responsive Breakpoints:**
- Mobile: 320-767px (343px width)
- Tablet: 768-1023px (396px width)
- Desktop-sm: 1024-1279px (468px width)
- Desktop-md: 1280-1439px (564px width)

**Styling:**
- Surface container with low emphasis
- Border radius and stroke support
- Dynamic spacing (XL inset padding)

---

## Editorial Cards

### 2. aem.card-editorial (v2.0)

**Purpose:** Rich editorial content card with media, heading, description, and optional list items.

**Key Features:**
- Fixed media component (image/video)
- Kicker text + title heading
- Description text
- Configurable list with multiple items
- Action link
- Navigation pagination
- Image positioning (top, left, right)

**Anatomy:**
- Root container with wrapper
- Media (webmedia-fixed)
- Content section with heading (kicker + title)
- Description text
- List container with list items (listing-24 icons)
- Slot for additional items
- Action and pagination

**Supported Breakpoints:**
- Mobile: 320-767px (375px width)
- Tablet: 768-1023px (768px width)

**Invalid Combinations:**
- Left/right image positioning not supported
- Desktop-sm and Desktop-md breakpoints not supported

---

### 3. aem.card-editorial-article (v2.0)

**Purpose:** Article-focused editorial card with badge, button, and pagination.

**Key Features:**
- Fixed media component
- Title with badge support
- Description with action link
- Primary button (CTA)
- Condensed pagination navigation
- Image positioning options

**Anatomy:**
- Root container with wrapper
- Media (webmedia-fixed)
- Content: title with badge, description with action
- Button (webbutton)
- Pagination (webpagination-condensed)

**Supported Breakpoints:**
- Mobile: 320-767px (375px width)
- Tablet: 768-1023px (768px width)

**Invalid Combinations:**
- Left/right image positioning not supported
- Desktop breakpoints not supported

---

## Offer Cards

### 4. aem.card-offer (v2.0)

**Purpose:** Promotional offer card with badge, countdown timer, and QR code support.

**Key Features:**
- Fixed media component
- Badge for offer labeling
- Countdown timer component
- Title and offer content
- Action button
- QR code for app download (desktop only)
- Responsive across all breakpoints

**Anatomy:**
- Root container with wrapper
- Media (webmedia-fixed)
- Content with heading (badge + countdown + title)
- Offer content description
- Action container with button
- QR code (desktop breakpoints only)

**Supported Breakpoints:**
- Mobile: 320-767px (375px width)
- Tablet: 768-1023px (768px width)
- Desktop-sm: 1024-1279px (1024px width)
- Desktop-md: 1280-1439px (1340px width)

**Special Features:**
- QR code with gradient background for desktop
- Badge with offer styling (high emphasis)
- Countdown component without background

---

## Card Containers

Card containers are wrapper components that manage multiple card instances with layout options like carousel or grid.

### 5. aem.card-image-default-container (v3.1.2)

**Purpose:** Container for default image cards with flexible display options.

**Key Features:**
- Display modes: Grid or Carousel
- Configurable number of items (1 to 5+)
- Display options with tabs
- Pagination for carousel mode
- Responsive column layouts

**Anatomy:**
- Root with wrapper
- Display options (webtabs)
- Carousel/Grid container with items
- Individual card instances (card-image-default-v3)
- Pagination (webpagination-condensed)

**Supported Breakpoints:**
- Tablet: 768-1023px (768px width)
- Desktop-sm: 1024-1279px (1024px width)
- Desktop-md: 1280-1439px (1340px width)

**Invalid Combinations:**
- Mobile breakpoint not supported
- Column configurations 2-5 not supported

---

### 6. aem.card-image-offer-container (v2.0)

**Purpose:** Container specifically for offer image cards in carousel format.

**Key Features:**
- Carousel display with pagination
- 3+ items support
- Optimized for desktop breakpoints
- 3-column grid layout

**Anatomy:**
- Root with wrapper
- Carousel container
- Multiple card items (card-image-offer-v1)
- Pagination navigation

**Supported Breakpoints:**
- Desktop-sm: 1024-1279px (1024px width)
- Desktop-md: 1280-1439px (1340px width)

**Invalid Combinations:**
- Mobile and tablet breakpoints not supported
- 1-2 item configurations not supported
- 1-2 column layouts not supported

---

### 7. aem.card-image-logo-container (v2)

**Purpose:** Container for logo image cards with compact spacing.

**Key Features:**
- Carousel display with tabs
- Display options toggle
- Compact inline spacing
- 1+ items configuration
- Single column layout

**Anatomy:**
- Root with wrapper
- Display options with tabs
- Carousel with items
- Card instances (card-image-logo-v2)
- Pagination

**Supported Breakpoints:**
- Tablet: 768-1023px (768px width)
- Desktop-sm: 1024-1279px (1024px width)
- Desktop-md: 1280-1439px (1340px width)

**Invalid Configurations:**
- Mobile breakpoint not supported
- Multi-item configurations (2-5+) not supported
- Multi-column layouts not supported

---

### 8. aem.card-image-wide-container (v3.1.2)

**Purpose:** Container for wide image cards with full-width display.

**Key Features:**
- Single item or multiple items (2+)
- Display options with tabs
- Full-grid display support
- Carousel mode with gradient mask
- Content alignment options (left, right, bottom)

**Anatomy:**
- Root with wrapper
- Display options (webtabs)
- Items container or carousel
- Wide card instances (card-image-wide-v3)

**Supported Breakpoints:**
- Mobile: 320-767px (375px width)
- Tablet: 768-1023px (768px width)
- Desktop-sm: 1024-1279px (1024px width)
- Desktop-md: 1280-1439px (1340px width)

**Special Features:**
- Gradient mask in carousel mode
- Scroll behavior configuration
- Content alignment varies by breakpoint

---

## Specialized Cards

### 9. aem.heading-with-card (v2.0)

**Purpose:** Hero-style card with prominent heading overlaid on media.

**Key Features:**
- Full-width media background
- Absolutely positioned card overlay
- Kicker + title + description
- Action button
- Multiple display modes
- Pagination for multiple cards
- Booking engine integration

**Display Modes:**
1. **Default:** Standard overlay card
2. **Full-grid:** Card with grid margins
3. **Wide:** Extended height layout
4. **Booking-engine:** Integrated booking component

**Anatomy:**
- Root container
- Background media (webmedia-fixed)
- Overlay card with texts and button
- Optional pagination
- Optional booking engine component

**Supported Breakpoints:**
- Mobile: 320-767px (375px width)
- Tablet: 768-1023px (768px width)
- Desktop-sm: 1024-1279px (1024px width)
- Desktop-md: 1280-1439px (1340px width)

**Card Configurations:**
- Single card: One prominent card overlay
- Multiple cards: Multiple cards with pagination

---

## Common Features

### Text Components

All card components support these text elements:
- **Kicker:** Small label/category text (detail style)
- **Title:** Main heading (display-03 or title-03)
- **Subtitle:** Secondary heading (body-default-01)
- **Description:** Body content (body-default-01)

### Interactive Elements

- **Actions:** Link or button actions (contentcardaction, contentaction)
- **Buttons:** Primary/secondary/tertiary buttons (webbutton)
- **Pagination:** Condensed pagination for navigation (webpagination-condensed)
- **Tabs:** Display option tabs (webtabs)

### Media Components

- **webmedia-fixed:** Fixed aspect ratio media (images/video)
- **webmedia-free:** Free-form media sizing
- **Placeholder support:** All media components support placeholders
- **Controllers:** Optional media controls
- **Overlay/Gradient:** Optional overlay effects
- **Caption:** Optional media captions

### Additional Components

- **Badge:** webbadge for labels and offers
- **Countdown:** webcountdown for time-sensitive offers
- **Carousel:** webcarousel for multiple items
- **List items:** listing-24 for bullet points
- **QR code:** Custom QR code component for app downloads

---

## Breakpoints

All components follow a consistent breakpoint system:

| Breakpoint | Range (px) | Typical Width |
|-----------|------------|---------------|
| Mobile | 320-767 | 343-375px |
| Tablet | 768-1023 | 768px |
| Desktop-sm | 1024-1279 | 1024px |
| Desktop-md | 1280-1439 | 1340px |

### Responsive Behavior

- **Mobile:** Vertical stacking, full-width cards
- **Tablet:** Increased card width, optimized spacing
- **Desktop-sm:** Multi-column layouts, larger cards
- **Desktop-md:** Maximum width, enhanced spacing

### Grid System

- **Margins:** Dynamic grid margins (breakpoints/wel/sem/sizing/grid/margins)
- **Spacing:**
  - Stack (vertical): xs, sm, md, lg, xl, 2xl
  - Inline (horizontal): xs, sm, md, lg, xl, 2xl
  - Inset (padding): md, xl, 2xl, 4xl
  - Within section: md, 2xl

---

## Color System

All components use semantic color tokens:

- **Surface:** surface, surface-container-low
- **On-surface:** on-surface-hi, on-surface-mid, on-surface-low
- **Primary:** primary, primary-container-low
- **Neutral:** neutral-container
- **Outline:** outline-low
- **Offer:** offer (special color for promotional content)
- **Loyalty:** loyalty-container-low (for QR codes)

---

## Styling System

### Border Radius
- **Surface:** breakpoints/wel/sem/borderRadius/surface
- **Element:** breakpoints/wel/sem/borderRadius/element/static-md, static-lg

### Border Width
- **Default:** breakpoints/wel/sem/borderWidth/default

### Shadows
- **Strong bottom:** effectStyleId: "strong-bottom"

### Typography
- **Display:** display-03
- **Title:** title-03
- **Body:** body-default-01
- **Detail:** detail

---

## Metadata

All components are:
- **Author:** Arthur MATHON
- **Generator:** Directed Edges Anova Figma Plugin (v4)
- **Schema:** Anova v0.3.0
- **Last Updated:** December 2025
- **Source:** Figma pages with specific node IDs

---

## Component Status

### Production Ready
- aem.card (v2.0)
- aem.card-offer (v2.0)
- aem.heading-with-card (v2.0)

### Limited Breakpoint Support
- aem.card-editorial (v2.0) - Mobile/Tablet only
- aem.card-editorial-article (v2.0) - Mobile/Tablet only

### Desktop Only
- aem.card-image-offer-container (v2.0)

### Tablet+ Only
- aem.card-image-default-container (v3.1.2)
- aem.card-image-logo-container (v2)

### All Breakpoints
- aem.card-image-wide-container (v3.1.2)
- aem.heading-with-card (v2.0)

---

## Usage Guidelines

### When to Use Each Card Type

1. **aem.card:** General purpose content cards, feature highlights, info boxes
2. **aem.card-editorial:** Blog posts, articles, news items with rich content
3. **aem.card-editorial-article:** Long-form article previews with CTAs
4. **aem.card-offer:** Promotions, deals, time-sensitive offers
5. **Container components:** Collections of cards, product grids, galleries
6. **aem.heading-with-card:** Hero sections, landing page headers, prominent CTAs

### Best Practices

- Use containers for multiple cards to ensure consistent spacing and layout
- Choose display mode (grid/carousel) based on content amount and user experience
- Enable pagination for carousels with 4+ items
- Use badges and countdown timers sparingly for high-impact offers
- Test responsive behavior across all supported breakpoints
- Leverage the semantic color system for consistent theming
- Consider image positioning based on content hierarchy

---

## File Locations

```
/core-aem/components/
├── aem.card.2.0.md
├── aem.card-editorial.2.0.txt
├── aem.card-editorial-article.2.0.txt
├── aem.card-offer.2.0.txt
├── aem.card-image-default-container-v3.1.2.md
├── aem.card-image-offer-container-v2.0.md
├── aem.card-image-logo-container-v2.txt
├── aem.card-image-wide-container-v3.1.2.md
└── aem.heading-with-card.2.0.txt
```

---

## Version History

- **v3.1.2:** card-image-default-container, card-image-wide-container
- **v2.0:** card, card-editorial, card-editorial-article, card-offer, heading-with-card, card-image-offer-container, card-image-logo-container

---

*Last updated: 2026-01-07*
*Generated from Figma component specifications using Anova plugin*

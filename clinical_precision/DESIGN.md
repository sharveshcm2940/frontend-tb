---
name: Clinical Precision
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#45464d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#515f74'
  on-secondary: '#ffffff'
  secondary-container: '#d5e3fd'
  on-secondary-container: '#57657b'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#001e2f'
  on-tertiary-container: '#008cc7'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#d5e3fd'
  secondary-fixed-dim: '#b9c7e0'
  on-secondary-fixed: '#0d1c2f'
  on-secondary-fixed-variant: '#3a485c'
  tertiary-fixed: '#c9e6ff'
  tertiary-fixed-dim: '#89ceff'
  on-tertiary-fixed: '#001e2f'
  on-tertiary-fixed-variant: '#004c6e'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-xl:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-bold:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  data-mono:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  container-margin: 32px
  gutter: 20px
---

## Brand & Style

The design system is engineered for high-stakes medical environments where clarity, speed of cognition, and trust are paramount. The brand personality is authoritative yet empathetic, blending the sterile reliability of a laboratory with the sophisticated interface of premium aerospace software. 

The aesthetic leverages **Modern Minimalism** infused with **Glassmorphism**. By using translucent layers and subtle background blurs, the system creates a sense of depth and spatial awareness without overwhelming the user with unnecessary skeuomorphism. This "rich" visual language differentiates the product from standard administrative tools, signaling to clinicians that they are operating a precision instrument. The emotional response is one of calm focus, reducing cognitive load during critical decision-making.

## Colors

The palette is anchored by "Midnight Navy" (#0F172A), providing a grounding sense of institutional stability. This is contrasted against "Clinical White" and a scale of "Slate Grays" that define the interface's structure.

The accent strategy is strictly functional:
- **Emerald (#10B981)** is reserved for "Normal" ranges, successful operations, and stable vitals.
- **Amber (#F59E0B)** signifies "Caution," pending data, or borderline clinical results.
- **Crimson (#E11D48)** is used exclusively for "High-Risk" alerts, critical values, and urgent system errors.

A secondary "Sky Blue" is utilized for interactive elements (links, primary buttons) to distinguish them from the deep blue of the brand identity.

## Typography

This design system employs **Manrope** for headlines to provide a modern, slightly technical character that feels premium. **Inter** is used for all functional text and body copy due to its exceptional legibility in dense data environments.

Hierarchy is maintained through strict weight differentiation. Data points—such as heart rates or lab values—should use `data-mono` settings to ensure tabular numbers align vertically, facilitating rapid comparison. Labels utilize medium and semi-bold weights to remain distinct from the data they describe.

## Layout & Spacing

The layout utilizes a **12-column fluid grid** with generous margins to prevent the UI from feeling cramped. The system follows a 4px base unit to ensure all components scale mathematically.

In clinical dashboards, information density is managed through "Progressive Disclosure." Use `lg` (24px) padding for primary containers and `md` (16px) for internal card spacing. This ensures that while the system contains a high volume of data, it never feels cluttered or overwhelming.

## Elevation & Depth

Depth is achieved through **Glassmorphism and Ambient Shadows**. Surface levels are defined as:

1.  **Base Level (L0):** The primary background color (`#F8FAFC`).
2.  **Surface Level (L1):** Standard cards with a 1px border in `Slate 200` and a very soft, 12% opacity shadow with a 20px blur.
3.  **Overlay Level (L2):** Modal windows and dropdowns featuring a background blur (12px) and a semi-transparent white fill (85% opacity). This creates the "glass" effect, allowing the context of the medical record to remain visible beneath the active task.

Shadows should be tinted with the primary navy color (`#0F172A`) at extremely low opacities to maintain a cohesive, "rich" color profile.

## Shapes

The design system uses a **Rounded** shape language to soften the clinical environment and improve touch-target approachability. 

- **Standard Components:** 0.5rem (8px) for buttons, inputs, and small widgets.
- **Large Containers:** 1rem (16px) for cards and main content areas.
- **Status Pills:** Fully rounded (pill-shaped) to distinguish them from interactive buttons.

## Components

### Sophisticated Data Tables
Tables are the core of this system. They must feature sticky headers, "zebra-striping" using subtle gray tints, and high-contrast text for data cells. Row hover states should use a translucent blue tint to indicate focus without obscuring the text.

### Interactive Charts
Charts use a "Thin Line" aesthetic. Sparklines and trend graphs should utilize the status colors (Emerald, Amber, Crimson) to indicate whether a patient's trajectory is improving or declining. Grid lines must be minimal and low-contrast.

### High-Res Image Containers
For radiology and clinical photos, containers feature a "dark-room" mode (black background) with integrated zoom and pan controls. Borders should be sharp or minimally rounded to maximize the viewable area of the image.

### Status Badges
Badges are pill-shaped with a "Soft Glow" effect. Use a light background tint of the status color with high-contrast text and a small leading icon (e.g., a checkmark, exclamation, or pulse) for accessibility.

### Glassmorphism Cards
Primary metric cards (e.g., Patient Vitals) should use the glass effect: a white-to-transparent gradient stroke, a background blur, and a subtle drop shadow to pop against the base layout.
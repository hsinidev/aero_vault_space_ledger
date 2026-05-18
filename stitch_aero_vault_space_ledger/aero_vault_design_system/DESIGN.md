---
name: Aero-Vault Design System
colors:
  surface: '#131316'
  surface-dim: '#131316'
  surface-bright: '#3a393c'
  surface-container-lowest: '#0e0e11'
  surface-container-low: '#1c1b1e'
  surface-container: '#201f22'
  surface-container-high: '#2a292d'
  surface-container-highest: '#353437'
  on-surface: '#e5e1e5'
  on-surface-variant: '#c8c5cf'
  inverse-surface: '#e5e1e5'
  inverse-on-surface: '#313033'
  outline: '#918f99'
  outline-variant: '#47464e'
  surface-tint: '#c2c2f2'
  primary: '#c2c2f2'
  on-primary: '#2b2d53'
  primary-container: '#1a1b41'
  on-primary-container: '#8283af'
  inverse-primary: '#5a5b84'
  secondary: '#c7c6c4'
  on-secondary: '#303130'
  secondary-container: '#464746'
  on-secondary-container: '#b5b5b3'
  tertiary: '#c6c6c6'
  on-tertiary: '#303030'
  tertiary-container: '#1f1f1f'
  on-tertiary-container: '#878787'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c2c2f2'
  on-primary-fixed: '#16173d'
  on-primary-fixed-variant: '#42436b'
  secondary-fixed: '#e3e2e0'
  secondary-fixed-dim: '#c7c6c4'
  on-secondary-fixed: '#1b1c1b'
  on-secondary-fixed-variant: '#464746'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#131316'
  on-background: '#e5e1e5'
  surface-variant: '#353437'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
spacing:
  unit: 4px
  gutter: 24px
  margin: 32px
  container-max: 1440px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

This design system embodies the "Hardened" aesthetic, communicating absolute security and institutional permanence for off-planet asset management. The brand personality is uncompromising, precise, and authoritative. It draws heavily from **Brutalism** and **Industrial Design**, utilizing raw textures and heavy structural elements to simulate the physical weight of a secure vault. 

The target audience consists of institutional aerospace entities and blockchain auditors who require high-density data presented with maximum clarity. The UI should evoke a sense of "cold" reliability—technical, high-tech, and immutable.

## Colors

The palette is anchored by **Deep Indigo (#1A1B41)**, used exclusively for primary actions and critical interactive states to provide a punch of high-tech energy against the monochromatic base. **Platinum Silver (#E5E4E2)** serves as the primary structural color, used for heavy borders and typography to create a metallic, high-contrast feel.

**Black (#000000)** provides the infinite-void background essential for a space-centric registry. Functional accents include a high-visibility Mint for 'Verified' statuses and a muted Grey for 'Immutable' states, ensuring that system integrity is communicable at a glance.

## Typography

This system utilizes a hybrid typographic approach to balance readability with a technical aesthetic. **Hanken Grotesk** is used for headlines to provide a sharp, contemporary edge. **Inter** handles standard body copy for its neutral, systematic clarity. 

All technical data, hash strings, and coordinates are rendered in **JetBrains Mono**. This distinction ensures that "human" content and "machine" data are visually segmented. All labels and status indicators use uppercase monospaced type to reinforce the industrial, military-grade feel.

## Layout & Spacing

The layout follows a **Rigid Fixed Grid** system to emphasize structural integrity. Elements are placed on a 4px baseline grid, with a 12-column layout for desktop and a 4-column layout for mobile. 

Gutters are kept wide (24px) to prevent data density from feeling cluttered. Spacing is used aggressively to create "zones" of information. Padding inside components should be generous, ensuring that the heavy 4px borders have room to breathe without impinging on content.

## Elevation & Depth

This design system rejects traditional soft shadows in favor of **Tonal Layering** and **Physical Offsets**. 

1.  **Z-0 (Base):** Pure Black (#000000).
2.  **Z-1 (Surface):** Deep Indigo (#1A1B41) at 10% opacity or subtle metallic gradients.
3.  **Z-2 (Active):** Hard 4px "Block Shadows" (non-diffused) in Platinum Silver to simulate an extruded, tactile surface.

Depth is communicated through border thickness rather than blur. Interactive elements may use a 2px offset when clicked to simulate a physical mechanical press.

## Shapes

The shape language is strictly **Sharp (0px radius)**. Every element, from buttons to large containers, must feature 90-degree angles to maintain the brutalist, vault-like atmosphere. 

To add visual interest without using curves, we employ **chamfered corners** (45-degree angled cuts) on primary action buttons and "Verified" badges, mimicking the machined edges of aerospace hardware.

## Components

### Secure Cards
Cards are the primary container for asset data. They feature a **4px solid Platinum Silver border**. For high-value assets, apply a subtle linear metallic gradient (Top-Left: #333333 to Bottom-Right: #000000) to the background.

### Buttons
*   **Primary:** Deep Indigo background, white text, 2px Platinum border. Use `label-caps` typography.
*   **Secondary:** Black background, Platinum text, 4px Platinum border. 
*   **State:** On hover, the button should "fill" with the border color (Invert).

### Status Indicators
*   **Verified:** A chamfered badge with a Mint green border and monospaced text.
*   **Immutable:** A heavy square badge with a "locked" icon and a 2px grey border.

### Input Fields
Fields are recessed with a 2px top and left inner stroke to create a "stamped" look into the UI surface. All text input uses `data-mono` for technical precision.

### Registry Lists
Data tables must feature alternating row fills (Z-1 depth) and vertical separators between columns to reinforce the industrial grid. Row headers should be bold and capitalized.
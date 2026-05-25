---
name: Cyber-Brutalist Fusion
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1b1b1b'
  surface-container: '#1f1f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#b9ccb5'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#303030'
  outline: '#849581'
  outline-variant: '#3b4b3a'
  surface-tint: '#00e55b'
  primary: '#edffe8'
  on-primary: '#003911'
  primary-container: '#00ff66'
  on-primary-container: '#007128'
  inverse-primary: '#006e27'
  secondary: '#d3fbff'
  on-secondary: '#00363a'
  secondary-container: '#00eefc'
  on-secondary-container: '#00686f'
  tertiary: '#f9fafa'
  on-tertiary: '#2f3131'
  tertiary-container: '#dddddd'
  on-tertiary-container: '#606162'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#6bff83'
  primary-fixed-dim: '#00e55b'
  on-primary-fixed: '#002107'
  on-primary-fixed-variant: '#00531b'
  secondary-fixed: '#7df4ff'
  secondary-fixed-dim: '#00dbe9'
  on-secondary-fixed: '#002022'
  on-secondary-fixed-variant: '#004f54'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c7'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#131313'
  on-background: '#e2e2e2'
  surface-variant: '#353535'
typography:
  display-2xl:
    fontFamily: Anton
    fontSize: 120px
    fontWeight: '400'
    lineHeight: 110px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Anton
    fontSize: 64px
    fontWeight: '400'
    lineHeight: 72px
    letterSpacing: 0.02em
  headline-lg-mobile:
    fontFamily: Anton
    fontSize: 40px
    fontWeight: '400'
    lineHeight: 44px
  body-md:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
spacing:
  grid-border: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  glass-padding: 32px
---

## Brand & Style
The design system is a high-octane collision between the raw, industrial rigidity of **Neo-Brutalism** and the futuristic, ethereal depth of **Glassmorphism**. It is designed for a high-end college tech festival, targeting a Gen-Z audience that values both technical authenticity and premium digital aesthetics.

The brand personality is **aggressive, innovative, and structural**. It leverages heavy black strokes to ground the interface, while floating glass panels and radioactive neon accents provide a sense of high-tech sophistication. The emotional response is one of energy and "engineered" excitement—mimicking a developer terminal fused with a futuristic laboratory.

## Colors
The palette is built on a foundation of **Pure Black (#000000)** to maximize contrast and ensure neon elements appear "radioactive."

- **Primary (Neon Green):** Used for critical calls to action, successful states, and glowing structural highlights.
- **Secondary (Electric Cyan):** Used for interactive elements, data visualization, and secondary accents.
- **Neutral/Base:** The canvas is strictly black. Text is primarily white or off-white for maximum legibility against dark backgrounds.
- **Glass Specification:** Glass layers utilize a ultra-low opacity white fill with a high-strength backdrop blur to create a "frosted" separation from the underlying structural grid.

## Typography
The typography is built on extreme contrast. **Anton** provides massive, impactful headlines that echo brutalist poster design. **Geist** offers a clean, technical sans-serif for body content, ensuring readability within glass panels. **JetBrains Mono** is used for labels and technical metadata, reinforcing the "tech festival" theme.

All typography must be **strictly left-aligned**. Large display headers should use tight tracking to feel like a solid block of information.

## Layout & Spacing
The design system utilizes a **Rigid Fixed Grid**. The skeleton of the UI is defined by visible 4px solid black borders that divide the screen into functional zones.

- **Desktop:** A 12-column grid with 24px gutters. All primary containers must snap to these grid lines.
- **Glass Overlays:** Glass panels do not necessarily follow the grid's vertical lines but must be anchored to its intersections, creating a "floating over the blueprint" effect.
- **Spacing Rhythm:** Use a strict 8px base unit for internal padding. Glass containers require generous internal padding (32px+) to maintain their premium, airy feel against the heavy background borders.

## Elevation & Depth
Depth is achieved through a specific stacking order:
1.  **Base Layer:** The black canvas with visible 4px black/dark-grey grid lines.
2.  **Structural Layer:** Elements like sidebars or footer blocks that are "caged" by the 4px borders.
3.  **Glass Layer:** Interactive cards and modals. These use a `12px` backdrop blur and a subtle `1px` white border at 15% opacity.
4.  **Glow Layer:** Interactive elements (buttons/active tabs) emit an outer glow (`box-shadow`) using the primary neon green or electric cyan colors to indicate "power."

Shadows on glass elements are large and diffused: `0 8px 32px 0 rgba(0, 0, 0, 0.37)`.

## Shapes
In keeping with the Brutalist influence, the shape language is **predominantly sharp (0px)**. All structural grid containers and main buttons must have square corners to emphasize the "built" nature of the tech festival.

**Exception:** Glass panels may use a very slight softening (`rounded-sm` or 4px) only if necessary to prevent them from feeling visually "lethal" when floating over the background, but the preference remains sharp for a more aggressive, high-end technical look.

## Components
- **Buttons:** Sharp-edged. Primary buttons use a solid Neon Green fill with black text. On hover, they trigger a "glowing" state with a 20px spread neon shadow. Secondary buttons use a "Ghost" style with a 4px black border and white text.
- **Glass Cards:** The signature component. Transparent background with heavy blur. Content inside must be strictly aligned to a sub-grid.
- **Input Fields:** Thick 4px black bottom-border only. When focused, the border transitions to Electric Cyan with a subtle glow. Label text is always in JetBrains Mono.
- **Chips/Badges:** Monospaced text inside a solid black container with a 1px neon border.
- **Lists:** Separated by 4px black horizontal rules. Hovering over a list item transforms the background into a semi-transparent cyan tint.
- **Navigation:** Vertical orientation preferred, snapped to the left-most grid column, using massive display type for section headers.
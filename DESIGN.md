---
name: Bit-Perfect Retro
colors:
  surface: '#0c1609'
  surface-dim: '#0c1609'
  surface-bright: '#323c2d'
  surface-container-lowest: '#071105'
  surface-container-low: '#141e11'
  surface-container: '#182214'
  surface-container-high: '#222d1e'
  surface-container-highest: '#2d3828'
  on-surface: '#dae6d0'
  on-surface-variant: '#baccb0'
  inverse-surface: '#dae6d0'
  inverse-on-surface: '#293324'
  outline: '#85967c'
  outline-variant: '#3c4b35'
  surface-tint: '#2ae500'
  primary: '#efffe3'
  on-primary: '#053900'
  primary-container: '#39ff14'
  on-primary-container: '#107100'
  inverse-primary: '#106e00'
  secondary: '#72de58'
  on-secondary: '#053900'
  secondary-container: '#3aa625'
  on-secondary-container: '#043200'
  tertiary: '#fff8f7'
  on-tertiary: '#442927'
  tertiary-container: '#ffd3ce'
  on-tertiary-container: '#7a5955'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#79ff5b'
  primary-fixed-dim: '#2ae500'
  on-primary-fixed: '#022100'
  on-primary-fixed-variant: '#095300'
  secondary-fixed: '#8dfc71'
  secondary-fixed-dim: '#72de58'
  on-secondary-fixed: '#022100'
  on-secondary-fixed-variant: '#095300'
  tertiary-fixed: '#ffdad6'
  tertiary-fixed-dim: '#e7bdb8'
  on-tertiary-fixed: '#2c1513'
  on-tertiary-fixed-variant: '#5d3f3c'
  background: '#0c1609'
  on-background: '#dae6d0'
  surface-variant: '#2d3828'
typography:
  headline-lg:
    fontFamily: Space Mono
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Mono
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: 0em
  body-lg:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: 0em
  body-sm:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: 0em
  label-caps:
    fontFamily: Courier Prime
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
spacing:
  pixel-unit: 4px
  gutter: 16px
  container-max: 800px
  border-width: 4px
---

## Brand & Style
The design system adopts a **Retro-Brutalist 8-bit** aesthetic, specifically tailored for a developer profile. It evokes the nostalgia of late-80s arcade consoles and early home computing while maintaining the functional clarity required for a GitHub README.

The personality is energetic, technical, and unapologetically digital. It utilizes "lo-fi" visual constraints—such as limited color palettes and rigid pixel grids—to create a high-impact, memorable identity. The style relies on thick borders, dithered textures, and high-contrast color pairings to guide the eye through code snippets and personal projects.

## Colors
The palette is rooted in a "Night Mode" gaming environment. 
- **Primary (Neon Green):** Reserved for interactive elements, success states, and terminal-style text.
- **Background (Deep Black):** The foundation for the entire layout, ensuring maximum contrast.
- **Surface (Dark Purple):** Used for containers, card backgrounds, and secondary information blocks.
- **Accent (Hot Pink):** Used sparingly for alerts, highlights, or "New" badges to break the green/purple dominance.
- **Neutral (Slate Gray):** Employed for low-priority text and inactive borders.

## Typography
While true pixel fonts are often inaccessible in standard markdown, this design system utilizes **Monospaced** typefaces to simulate the grid-based alignment of terminal interfaces. 

Headlines should be set in bold, uppercase monospaced fonts to mimic 8-bit title cards. For body text, JetBrains Mono provides superior legibility for technical descriptions. Always align text to a strict 8px baseline to maintain the "blocky" feel.

## Layout & Spacing
The layout follows a **Fixed Pixel Grid**. Everything is based on increments of 4px and 8px.
- **Structure:** A single-column centered layout for readability, with occasional 2-column grids for "Stats" and "Languages" sections.
- **Margins:** Use a generous 32px outer margin to frame the content against the GitHub background.
- **Gutters:** Maintain a strict 16px gap between all cards and sections.
- **Dithering:** Where visual separation is needed without a solid line, use a checkerboard pattern of pixels (dithering) to transition between black and purple surfaces.

## Elevation & Depth
Depth is created through **Hard Shadows** rather than blurs. 
- **Shadows:** No Gaussian blurs are permitted. Use solid color offsets (usually Primary Green or Deep Purple) moved 4px down and 4px right to create a "pop-out" effect.
- **Borders:** Every container must have a minimum 2px (preferably 4px) solid border.
- **Tonal Layering:** The Background (#000000) is the lowest level. Surface (#2D0054) sits on top. Active elements like buttons or high-priority cards use the Primary color as a glowing border or thick shadow to indicate height.

## Shapes
The shape language is strictly **Rectilinear**. Curves are avoided entirely. 
- **Corners:** 0px radius. To simulate a "rounded" look in 8-bit style, use a "stepped" corner where the corner pixel is missing, creating a jagged 45-degree notch.
- **Connectors:** Use horizontal and vertical lines to connect related items (like a tech stack tree), mimicking motherboard traces.

## Components
- **Buttons:** Thick 4px borders. On hover/active, the background should invert (Text becomes Background, Background becomes Primary). Include a 4px bottom-right solid shadow.
- **Chips (Tags):** Small rectangular boxes with a 1px border. Use the Accent color for categories like "Languages" and Primary for "Tools."
- **Lists:** Use custom unicode characters (like `> ` or `■`) as bullet points. 
- **Cards:** Heavy 4px borders in Surface color. Titles within cards should be set against a "Header Bar" of a contrasting color.
- **Input Fields (Search simulation):** Black background with a Primary Green blinking cursor simulation (`_`).
- **Progress Bars (Skills):** Block-based bars where 10% increments are represented by solid blocks `[■■■■□□□□□□]`.
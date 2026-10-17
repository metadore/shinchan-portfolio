---
name: Mischief & Giggles
colors:
  surface: '#f4fafd'
  surface-dim: '#d4dbdd'
  surface-bright: '#f4fafd'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eef5f7'
  surface-container: '#e8eff1'
  surface-container-high: '#e2e9ec'
  surface-container-highest: '#dde4e6'
  on-surface: '#161d1f'
  on-surface-variant: '#5b403e'
  inverse-surface: '#2b3234'
  inverse-on-surface: '#ebf2f4'
  outline: '#8f6f6d'
  outline-variant: '#e4beba'
  surface-tint: '#ba1724'
  primary: '#b71422'
  on-primary: '#ffffff'
  primary-container: '#db3237'
  on-primary-container: '#fffbff'
  inverse-primary: '#ffb3ae'
  secondary: '#705d00'
  on-secondary: '#ffffff'
  secondary-container: '#fcd400'
  on-secondary-container: '#6e5c00'
  tertiary: '#80409b'
  on-tertiary: '#ffffff'
  tertiary-container: '#9b59b6'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad7'
  primary-fixed-dim: '#ffb3ae'
  on-primary-fixed: '#410004'
  on-primary-fixed-variant: '#930014'
  secondary-fixed: '#ffe16d'
  secondary-fixed-dim: '#e9c400'
  on-secondary-fixed: '#221b00'
  on-secondary-fixed-variant: '#544600'
  tertiary-fixed: '#f8d8ff'
  tertiary-fixed-dim: '#ebb2ff'
  on-tertiary-fixed: '#320047'
  on-tertiary-fixed-variant: '#692984'
  background: '#f4fafd'
  on-background: '#161d1f'
  surface-variant: '#dde4e6'
typography:
  headline-xl:
    fontFamily: Bricolage Grotesque
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 52px
    letterSpacing: -1px
  headline-lg:
    fontFamily: Bricolage Grotesque
    fontSize: 32px
    fontWeight: '800'
    lineHeight: 38px
  headline-lg-mobile:
    fontFamily: Bricolage Grotesque
    fontSize: 28px
    fontWeight: '800'
    lineHeight: 32px
  body-lg:
    fontFamily: Quicksand
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 28px
  body-md:
    fontFamily: Quicksand
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  label-sm:
    fontFamily: Quicksand
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 20px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The design system captures the chaotic, joyful, and irreverent spirit of 90s slice-of-life anime. It targets an audience that appreciates nostalgia, playfulness, and a break from corporate sterility. 

The aesthetic is a hybrid of **Modern-Brutalism** and **Tactile-Comic**. It utilizes heavy, deliberate strokes (2px to 3px outlines) to ground vibrant colors, creating a "sticker" effect where elements feel like they could be peeled off the screen. High-energy layouts with slight tilts and organic shapes evoke a sense of movement and mischief, while generous whitespace ensures the interface remains functional and readable.

## Colors
The palette is driven by high-saturation primary tones that command attention:
- **Shin-chan Red (#FF4D4D):** Used for primary actions, critical alerts, and brand-heavy moments.
- **Action Mask Yellow (#FFD700):** Used for warnings, highlights, and toggle states.
- **Buriburizaemon Purple (#9B59B6):** Used for secondary features, creative tools, or "premium" mischief.
- **Sky Blue (#87CEEB):** Acts as a grounding background wash or a secondary button color to prevent visual fatigue.
- **Ink Black (#2D3436):** Used for all outlines and body text to maintain the comic-book structure.

## Typography
The typography strategy balances character with legibility. 
- **Headlines:** Use Bricolage Grotesque for its expressive, slightly irregular curves that mimic hand-drawn signage. Large headlines should occasionally feature a -2 degree rotation to enhance the "playful" vibe.
- **Body & UI:** Use Quicksand. Its rounded terminals mirror the "soft corner" philosophy of the brand. Use "Medium" (500) as the base weight for body text to ensure it holds up against the heavy stroke weights of the UI elements.

## Layout & Spacing
The layout follows a **Fluid Comic Grid**. While content scales to the viewport, the containers themselves should feel distinct and separated by generous gutters.

- **Desktop:** 12-column grid with a maximum content width of 1280px. Use asymmetrical layouts (e.g., a 7-column main area and a 4-column sidebar) to keep the design dynamic.
- **Mobile:** 4-column grid. Margins are kept tight (16px) to maximize the "pop" of the card-based interface.
- **Rhythm:** Use the 8px base unit for all padding and margins. Vertical rhythm should be loose and airy.

## Elevation & Depth
In this design system, depth is not created with blurs or light-source shadows, but through **Hard-Edge Offsets**:

- **The "Sticker" Depth:** Elements do not "hover." Instead, they use a solid color offset (usually `Ink Black` or a darker shade of the primary color) positioned 4px to 8px down and to the right. 
- **Outlines:** Every interactive element must have a 2px solid border (`#2D3436`).
- **Layers:** Use "Sky Blue" for the lowest base layer, "White" for content containers, and "Action Mask Yellow" or "Red" for the most prominent interactive layers.

## Shapes
Everything is "squishy" yet structured. 
- **Standard Corners:** 0.5rem (8px) provides a friendly feel that matches the Quicksand typeface.
- **Interactive Elements:** Buttons and tags should use `rounded-xl` (1.5rem) to appear more "bouncy" and touchable.
- **Organic Accents:** Use CSS `blob` shapes or irregular `border-radius` (e.g., `60% 40% 30% 70% / 60% 30% 70% 40%`) for background decorative elements to mimic the messy, hand-drawn anime backgrounds.

## Components
- **Buttons:** Large, bold, and expressive. They must feature a 2px outline and a 4px solid "bottom-heavy" shadow offset. On `hover`, the shadow disappears as the button "pushes" into the screen.
- **Cards:** White backgrounds with a 2px black border. Use a "Shin-chan Red" or "Action Mask Yellow" header bar for internal categorizing.
- **Chips/Labels:** Use pill-shapes with a slightly tilted orientation (±1-3 degrees) to add a sense of energy.
- **Inputs:** High-contrast white backgrounds with thick outlines. The `focus` state should change the border color to "Buriburizaemon Purple" and increase the shadow offset.
- **Checkboxes:** Larger than standard (24px x 24px) with a heavy stroke. The "check" icon should look like a hand-drawn "X" or a playful squiggle.
- **Modals:** Use a heavy backdrop of "Sky Blue" (80% opacity) and ensure the modal container has a thick 3px black border and a large 12px solid shadow.
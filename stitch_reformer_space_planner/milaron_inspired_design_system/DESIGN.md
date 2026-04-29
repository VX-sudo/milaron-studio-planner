---
name: Milaron-Inspired Design System
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f4'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#4c4546'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f0f1f1'
  outline: '#7e7576'
  outline-variant: '#cfc4c5'
  surface-tint: '#5e5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1b1b1b'
  on-primary-container: '#848484'
  inverse-primary: '#c6c6c6'
  secondary: '#705d00'
  on-secondary: '#ffffff'
  secondary-container: '#fcd400'
  on-secondary-container: '#6e5c00'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#181c1e'
  on-tertiary-container: '#808487'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c6'
  on-primary-fixed: '#1b1b1b'
  on-primary-fixed-variant: '#474747'
  secondary-fixed: '#ffe16d'
  secondary-fixed-dim: '#e9c400'
  on-secondary-fixed: '#221b00'
  on-secondary-fixed-variant: '#544600'
  tertiary-fixed: '#e0e3e6'
  tertiary-fixed-dim: '#c3c7ca'
  on-tertiary-fixed: '#181c1e'
  on-tertiary-fixed-variant: '#43474a'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
typography:
  headline-xl:
    fontFamily: Manrope
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.25'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
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
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  data-mono:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.08em
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
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style

This design system is built upon the pillars of architectural precision and serene athleticism. It targets studio owners and fitness professionals who require a tool that balances high-end aesthetic appeal with rigorous functional utility. The visual narrative is "Airy Precision"—an environment where negative space is used as a functional element to prevent cognitive overload during complex studio planning tasks.

The style is **Minimalist with Subtle Tonal Depth**. It leverages the high-contrast relationship between deep obsidian tones and metallic gold accents, softened by a neutral, cool-grey foundation. The interface should feel like a premium pilates studio: spacious, orderly, and meticulously crafted. Every element serves a purpose, removing unnecessary ornamentation to focus on equipment measurements and spatial flow.

## Colors

The color palette is derived directly from a premium equipment aesthetic. 
- **Primary (#000000):** Used for primary actions, headlines, and structural boundaries. It provides the "weight" and authority needed for a professional tool.
- **Secondary (#FFD700):** This gold accent is used sparingly to denote "premium" status, highlighting active states, specialized equipment, or key milestones in the planning process.
- **Tertiary (#EEF1F4):** A soft, cool grey used for large background surfaces and "container" backgrounds to reduce eye strain and provide a canvas for measurements.
- **Neutral (#FFFFFF):** Pure white is reserved for high-level surfaces like cards and modals to create a sense of floating layers and airiness.

For data visualization and measurements, use the primary black for high-readability text against white or light grey backgrounds. Avoid using the gold for small text to ensure accessibility.

## Typography

This design system utilizes a dual-font strategy to balance elegance with technical clarity.
- **Manrope** is used for headlines and brand-heavy moments. Its geometric but refined curves reflect the modern industrial design of pilates reformers.
- **Inter** is the workhorse for measurements, equipment specifications, and interface labels. Its high x-height and neutral character ensure that "1200mm" is as legible as "Reformer Carriage."

A specific `data-mono` style is introduced for measurement inputs. While using Inter, it should be set with tabular lining figures (where numbers have equal width) to ensure that numerical data aligns perfectly in lists and planning grids.

## Layout & Spacing

The layout philosophy follows a **Fixed-Fluid Hybrid Grid**. For studio planning canvases, a 2D coordinate system is used (representing real-world floor space), while the management interface uses a traditional 12-column grid.

To achieve the "airy" feel, the system mandates generous external margins (64px on desktop) and significant vertical breathing room between sections (48px to 80px). Information density is kept low on overview pages but increases in "Spec Panels" where equipment data is critical. Use the 8px base unit for all component internal spacing to maintain a rhythmic, predictable flow.

## Elevation & Depth

Hierarchy is established through **Tonal Layering** rather than heavy shadows. The background is typically the Tertiary Grey (#EEF1F4), with functional cards and planning elements sitting on White (#FFFFFF) surfaces.

- **Level 0 (Floor):** Tertiary Grey (#EEF1F4) for the main application background.
- **Level 1 (Surface):** White (#FFFFFF) for cards and content containers. Use a 1px solid border of #000000 at 5% opacity instead of a shadow for a crisp, high-end feel.
- **Level 2 (Active):** When an equipment item is "picked up" or active in the studio planner, apply a soft, highly diffused ambient shadow (Color: #000000, Opacity: 8%, Blur: 20px, Y: 10px).
- **Overlays:** Modals use a backdrop blur (12px) with a 20% opacity black overlay to keep the user grounded in the "space" of the app while focusing on the task.

## Shapes

The shape language reflects the "Soft Industrial" nature of pilates equipment—where hard steel frames meet soft upholstered pads. 
- **Standard Elements:** Use a 0.5rem (8px) radius for buttons, input fields, and small cards. This feels modern and approachable without being overly "bubbly."
- **Equipment Blocks:** In the studio planner, equipment shapes should use a 0.25rem radius to emphasize their technical and structural nature.
- **Selection Indicators:** Use pill-shaped (full radius) buttons for toggle filters and status chips to distinguish them from action-oriented rectangular buttons.

## Components

### Buttons
- **Primary:** Solid Black (#000000) with White text. No border. High-end, authoritative.
- **Secondary/Action:** White background with a 1.5px Black border.
- **Accent:** Gold (#FFD700) is used only for "Upgrade" or "Special Edition" equipment prompts.

### Inputs & Measurement Fields
- Input fields should feature a clear label using `label-caps`. 
- Measurement inputs should include the unit (e.g., "mm" or "cm") as a suffix in a light grey tone, fixed to the right of the field.
- The focus state is a 2px solid Black border; never use default browser glows.

### Equipment Cards
- Cards used in the "Studio Library" should be white with a very thin, low-contrast border. 
- High-quality, cut-out (PNG/WebP) images of equipment should be centered with ample padding (at least 24px) to maintain the airy aesthetic.

### Planning Grid
- The floor planner uses a subtle dot-grid rather than solid lines to maintain a "clean" look. Dots should be #000000 at 10% opacity, spaced at 24px (standard 8px multiplier) intervals.

### Chips & Status
- Use subtle background tints for status (e.g., a very light gold tint for "Premium" or a light grey for "Draft"). Text remains black for readability.
---
name: AgentDesk Core
colors:
  surface: '#111827'
  surface-dim: '#0e1322'
  surface-bright: '#343949'
  surface-container-lowest: '#090e1c'
  surface-container-low: '#161b2b'
  surface-container: '#1a1f2f'
  surface-container-high: '#25293a'
  surface-container-highest: '#2f3445'
  on-surface: '#dee1f7'
  on-surface-variant: '#c3c6d7'
  inverse-surface: '#dee1f7'
  inverse-on-surface: '#2b3040'
  outline: '#8d90a0'
  outline-variant: '#434655'
  surface-tint: '#b4c5ff'
  primary: '#b4c5ff'
  on-primary: '#002a78'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#0053db'
  secondary: '#d0bcff'
  on-secondary: '#3c0091'
  secondary-container: '#571bc1'
  on-secondary-container: '#c4abff'
  tertiary: '#ffb596'
  on-tertiary: '#581e00'
  tertiary-container: '#bc4800'
  on-tertiary-container: '#ffede6'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d0bcff'
  on-secondary-fixed: '#23005c'
  on-secondary-fixed-variant: '#5516be'
  tertiary-fixed: '#ffdbcd'
  tertiary-fixed-dim: '#ffb596'
  on-tertiary-fixed: '#360f00'
  on-tertiary-fixed-variant: '#7d2d00'
  background: '#0e1322'
  on-background: '#dee1f7'
  surface-variant: '#2f3445'
  border: '#1E293B'
  text-primary: '#F8FAFC'
  text-muted: '#94A3B8'
  success: '#10B981'
  warning: '#F59E0B'
  accent-lime: '#E4F222'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
  panel-padding: 20px
  stack-gap: 8px
---

## Brand & Style

The design system is engineered for high-performance AI orchestration, targeting small business owners who require clarity amidst complexity. The brand persona is **authoritative and precise**, functioning as a "mission control" for automated workflows.

The visual style is **Premium SaaS Minimalism**, characterized by:
- **High-Density Information:** Maximizing screen real estate without compromising legibility.
- **Atmospheric Depth:** Using a dark-mode first approach to reduce eye strain and emphasize glowing AI status indicators.
- **Technical Sophistication:** Incorporating subtle glassmorphism and micro-interactions that provide immediate haptic-like feedback.
- **Precision:** Utilizing thin borders and monospaced accents to evoke a sense of "engineered" reliability.

## Colors

The color strategy relies on a **Deep Navy foundation** to provide a high-contrast backdrop for vibrant functional accents. 

- **Primary Electric Blue:** Reserved for high-priority actions and active agent states.
- **Secondary Violet:** Derived from the brand's sophisticated lineage, used for automated process indicators and AI-driven insights.
- **Surface & Borders:** A strict hierarchy of dark tones (`#0A0F1E` for global backgrounds and `#111827` for panels) ensures clear spatial containment.
- **Functional Accents:** Success and Warning colors are highly saturated to ensure they "pop" against the dark UI, providing immediate status recognition.

## Typography

This design system utilizes a dual-font approach to balance approachability with technical rigor.

- **Inter:** The primary workhorse. Use for all functional UI, headlines, and body copy. Tighten letter-spacing on larger headlines for a premium, "locked-in" feel.
- **JetBrains Mono:** Used sparingly for technical metadata, agent IDs, logs, and status labels to reinforce the "Agent/Developer" nature of the tool.
- **Scale:** Maintain a tight typographic scale. Given the density of a command center, `body-md` (14px) is the standard for most interface text.

## Layout & Spacing

The layout follows a **Fixed-Fluid Hybrid** model. Navigation and side-panels are fixed-width to ensure tool consistency, while the primary "Command Canvas" is fluid.

- **Grid:** Use a 12-column grid for the main content area.
- **Density:** Adopt a "Compact" density model. Use 8px (`base * 2`) for internal component spacing and 16px-24px for layout gaps.
- **Reflow:** On mobile, sidebars collapse into a bottom navigation bar or a hamburger drawer. Grid columns collapse to a single stack, but data-heavy cards should maintain horizontal scrolling for tables to preserve data integrity.

## Elevation & Depth

Depth is achieved through **Tonal Layering** and **Subtle Glassmorphism** rather than heavy shadows.

- **Layer 0 (Background):** `#0A0F1E` – The base canvas.
- **Layer 1 (Panels):** `#111827` – Content containers with a 1px border of `#1E293B`.
- **Layer 2 (Popovers/Menus):** Semi-transparent `#111827` (90% opacity) with a 12px backdrop blur and a slightly brighter border (`#334155`).
- **Shadows:** Use "Tight Elevation." A single 4px-8px blur shadow with 30% opacity, tinted with the primary color, is used only for floating elements like dropdowns and active tooltips.

## Shapes

The shape language is **Soft-Geometric**. 

- **Cards/Panels:** 8px (`rounded-lg`) provides a modern, professional look that isn't too clinical.
- **Buttons/Inputs:** 6px (standard) creates a tighter, more "engineered" aesthetic suitable for a command center.
- **Status Indicators:** Use perfect circles for "live" pulsing indicators to contrast against the rectangular grid.

## Components

- **Buttons:** 
  - *Primary:* Solid Electric Blue with white text. 
  - *Ghost:* 1px border with a glassmorphism hover state (background-color: `rgba(255,255,255,0.05)`).
- **Inputs:** Dark backgrounds (`#0A0F1E`) with 1px `#1E293B` borders. On focus, the border transitions to Primary Blue with a subtle 2px outer glow.
- **Chips/Badges:** Use JetBrains Mono for text. Backgrounds should be low-opacity versions of the status color (e.g., 10% Success Green) with 100% opacity text.
- **Command Palette:** A central floating component with high backdrop blur and a "Search" icon. Items within should have a 4px border-radius on hover.
- **Pulse Indicators:** AI agents in "active" status must feature a 2px pulsing ring around their status dot to indicate live processing.
- **Cards:** No shadows. Instead, use a subtle 1px border that brightens on hover to indicate interactivity.
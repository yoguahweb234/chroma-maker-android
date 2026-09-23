---
name: Dynamic Material Native
colors:
  surface: '#141317'
  surface-dim: '#141317'
  surface-bright: '#3a383d'
  surface-container-lowest: '#0e0e11'
  surface-container-low: '#1c1b1f'
  surface-container: '#201f23'
  surface-container-high: '#2b292d'
  surface-container-highest: '#353438'
  on-surface: '#e5e1e7'
  on-surface-variant: '#cac4d0'
  inverse-surface: '#e5e1e7'
  inverse-on-surface: '#313034'
  outline: '#948f9a'
  outline-variant: '#49454f'
  surface-tint: '#d0bcff'
  primary: '#e9ddff'
  on-primary: '#37265e'
  primary-container: '#d0bcff'
  on-primary-container: '#594983'
  inverse-primary: '#665590'
  secondary: '#ccc2dc'
  on-secondary: '#332d41'
  secondary-container: '#4a4359'
  on-secondary-container: '#bab1ca'
  tertiary: '#ffd9e3'
  on-tertiary: '#492532'
  tertiary-container: '#efb8c8'
  on-tertiary-container: '#704654'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#d0bcff'
  on-primary-fixed: '#210f48'
  on-primary-fixed-variant: '#4d3d76'
  secondary-fixed: '#e9def9'
  secondary-fixed-dim: '#ccc2dc'
  on-secondary-fixed: '#1e182b'
  on-secondary-fixed-variant: '#4a4359'
  tertiary-fixed: '#ffd9e3'
  tertiary-fixed-dim: '#efb8c8'
  on-tertiary-fixed: '#31111d'
  on-tertiary-fixed-variant: '#633b48'
  background: '#141317'
  on-background: '#e5e1e7'
  surface-variant: '#353438'
typography:
  display-lg:
    fontFamily: Roboto Flex
    fontSize: 57px
    fontWeight: '400'
    lineHeight: 64px
  display-md:
    fontFamily: Roboto Flex
    fontSize: 45px
    fontWeight: '400'
    lineHeight: 52px
  display-sm:
    fontFamily: Roboto Flex
    fontSize: 36px
    fontWeight: '400'
    lineHeight: 44px
  headline-lg:
    fontFamily: Roboto Flex
    fontSize: 32px
    fontWeight: '400'
    lineHeight: 40px
  headline-md:
    fontFamily: Roboto Flex
    fontSize: 28px
    fontWeight: '400'
    lineHeight: 36px
  headline-sm:
    fontFamily: Roboto Flex
    fontSize: 24px
    fontWeight: '400'
    lineHeight: 32px
  title-lg:
    fontFamily: Roboto Flex
    fontSize: 22px
    fontWeight: '400'
    lineHeight: 28px
  title-md:
    fontFamily: Roboto Flex
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  title-sm:
    fontFamily: Roboto Flex
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  body-lg:
    fontFamily: Roboto Flex
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Roboto Flex
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Roboto Flex
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-lg:
    fontFamily: Roboto Flex
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  label-md:
    fontFamily: Roboto Flex
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  label-sm:
    fontFamily: Roboto Flex
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  margin: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style

This design system delivers an authentic Android 14+ native experience rooted in Material Design 3 (Material You). Built to empower visual creators, UI designers, and illustrators, it combines structural rigor with expressive color synthesis. 

The interface maintains a neutral, content-forward canvas to ensure generated color palettes remain the focal hero. The design style balances modern utility with tactile physical logic: utilizing tonal elevation instead of skeuomorphic drop shadows, continuous curves, dynamic ripple surfaces, and purposeful fluid motion. Visual hierarchy is established via luminance shifts and tonal containers rather than loud chrome, allowing creative swatches and spectrums to dominate the visual landscape.

## Colors

The system uses an algorithmic dynamic palette model adhering to Material Design 3 color roles. While defaults are configured for dark mode to showcase high-luminance generated swatches, all tonal roles map symmetrically across light and dark contexts.

### Dynamic Role Assignments
- **Primary (`#D0BCFF` in dark / `#6750A4` in light):** Reserved for key focal actions, the Floating Action Button (FAB), active navigation pills, and primary selection states.
- **Secondary (`#CCC2DC` in dark / `#625B71` in light):** Deployed for supporting interface elements, secondary filter chips, and segmented button toggles.
- **Tertiary (`#EFB8C8` in dark / `#7D5260` in light):** Used for contrasting accents, specialty tag markers, and dynamic harmony highlights (e.g., complementary or triadic balance indicators).
- **Surface Roles:** The neutral scale is strictly segmented into five tonal tiers:
  - `surface`: Baseline background canvas (`#141218`).
  - `surface-container-lowest`: Deep recessed card slots and picker wells (`#0F0D13`).
  - `surface-container-low`: Broad non-interactive canvas groupings (`#1D1B20`).
  - `surface-container`: Standard default for cards, dialogs, and sheets (`#211F26`).
  - `surface-container-high`: Raised interactive pickers, expanded panels (`#2B2930`).
  - `surface-container-highest`: Highest contrast containers, search bars, and active input wells (`#36343B`).
- **On-Colors:** All interactive tokens strictly follow WCAG AAA contrast guidelines (`on-primary`, `on-surface`, `on-surface-variant`). Hero swatches must dynamically compute readable text overlays based on their computed APCA/WCAG contrast ratios.

## Typography

The typographic hierarchy implements the canonical Material 3 Type Scale using `Roboto Flex` (the standard Android variable system font). This ensures native rendering fidelity, responsive optical sizing, and optimal letterforms across Android display densities.

- **Display & Headlines:** Used selectively for full-screen color metrics, color science readouts (e.g., Hex, HSL, OKLCH values), and screen headers. On compact mobile screens, headers scale down to `headline-sm` or `title-lg` to prevent line wrapping over active generator viewports.
- **Titles & Labels:** Standardized for interactive components. `label-lg` drives standard button copy, FAB labels, and navigation item labels. `label-md` and `label-sm` govern filter chips, status badges, and color format tags.
- **Body:** Calibrated for descriptive metadata, color theory explanations, and accessibility contrast readouts. Monospace numeric behavior is achieved through tabular lining figures within `Roboto Flex` for dynamic color coordinates.

## Layout & Spacing

Layout geometry follows an 8dp baseline grid (with 4dp half-step substructures for icon alignment and fine chip padding) mapped to Android Jetpack Compose spatial primitives.

### Adaptability & Form Factors
- **Compact (< 600dp / Phones):** 
  - Margin: 16dp (`1rem`), Gutter: 16dp (`1rem`).
  - Swatch displays utilize a dynamic 1-column stack or vertical split strip occupying primary viewport height.
  - Controls are anchored via standard Bottom App Bars, Navigation Bars, and Modal BottomSheets.
- **Medium (600dp - 839dp / Foldables & Small Tablets):** 
  - Margin: 24dp (`1.5rem`), Gutter: 16dp (`1rem`).
  - Bottom navigation reflows into a persistent Navigation Rail docked on the start edge.
  - Palette canvas splits horizontally: interactive color generation sandbox on the left, adjustment sliders on the right.
- **Expanded (>= 840dp / Tablets & Desktops):** 
  - Margin: 24dp (`1.5rem`), Gutter: 24dp (`1.5rem`).
  - Employs a full persistent Navigation Drawer.
  - Multi-pane layout: 12-column fluid grid orchestrating side-by-side swatch comparison, gamut curves, and history boards.

## Elevation & Depth

This system discards legacy drop shadows in favor of Material 3 **Tonal Surface Elevation**. Depth is communicated through controlled shifts in surface luminance and primary color tinting.

### Elevation Levels & Surface Tinting
- **Level 0 (Flat, 0dp):** `surface` background color. Direct canvas area where swatches rest.
- **Level 1 (Card Default, 1dp):** `surface-container-low` with a 5% primary color tint blend. Used for non-interactive list cards and resting palette containers.
- **Level 2 (Scrolled App Bar / Hovered Card, 3dp):** `surface-container` with an 8% primary tint. Standard for docked bottom toolbars, search bars, and filter strips.
- **Level 3 (Modal BottomSheet / Dialog, 6dp):** `surface-container-high` with an 11% primary tint. Provides immediate physical hierarchy over base content.
- **Level 4 (Floating Action Button, 8dp):** `surface-container-highest` with a 12% primary tint. 
- **Level 5 (Dragging / Active Lift, 12dp):** High-luminance tonal container complemented by an ambient, low-opacity (8-12%) tinted contact shadow to indicate touch detachment during swatch reordering.

### Microinteractions & Surface Tint Response
All elevation state changes (resting, hovered, focused, pressed, dragged) transition using standard Material motion curves (`standard-easing`: cubic-bezier(0.2, 0.0, 0, 1.0) over 250ms). Touch down states produce bounded, semi-translucent primary ripples (`state-layer-pressed`, 12% opacity).

## Shapes

The shape system adopts Material 3 shape tokens, using distinct corner treatments to differentiate persistent containers from actionable components.

- **Extra-Small (4dp / 0.25rem):** Color swatch preview tags, inline badges, and slider thumbs.
- **Small (8dp / 0.5rem):** Text input containers, segmented button internal borders, and context menus.
- **Medium (12dp / 0.75rem):** Palette preview cards and color history thumbnails.
- **Large (16dp / 1.0rem):** Main container cards, modal dialogs, and color picker modal frames.
- **Extra-Large (28dp / 1.75rem):** Top corners of BottomSheets, search bars, and dynamic action cards.
- **Full (Pill, 9999dp):** Filter chips, segmented buttons, active navigation indicators, primary Floating Action Buttons, and lock/unlock toggle pills.

## Components

### Buttons & FABs
- **Extended FAB / Standard FAB:** Floating 56dp (standard) or 80dp (large) pill/rounded container (`shape-large` or `shape-full`). Tinted with `primary-container` and `on-primary-container`. Positioned anchored to the bottom-end or centered docked in BottomAppBar. Triggering generation provides a subtle haptic feedback burst (`HapticFeedbackType.LongPress`).
- **Segmented Buttons:** Unified container (`shape-full`) containing multiple toggle segments (e.g., "Monochromatic", "Analogous", "Triadic", "Complementary"). Active segment fills with `secondary-container` displaying an animated checkmark icon.

### Chips (Assist, Filter, Input)
- **Filter & Action Chips:** Height of 32dp with `shape-full` pill contours. Inactive chips use a 1dp outline (`outline-variant`) on transparent ground; selected chips use `secondary-container` with an active leading icon indicator.

### BottomSheets & Navigation
- **Modal BottomSheet:** Uses `shape-extra-large` (28dp) rounding strictly on top-left and top-right corners. Contains a centered 32x4dp pill drag handle in `on-surface-variant` (40% opacity). Backed by a scrim (`scrim` token, 32% black).
- **M3 NavigationBar:** Fixed 80dp height resting on `surface-container`. Active tab displays a 64x32dp pill indicator in `secondary-container` housing the icon, accompanied by a dedicated `label-medium` label underneath.

### Input Fields & Sliders
- **Text Fields (Hex / Color Value Entry):** Outlined variant with 8dp rounded corners (`shape-small`) and 1dp stroke (`outline`). Active focus expands border to 2dp in `primary`. Includes leading eyedropper icon and trailing copy-to-clipboard action.
- **Color Sliders (RGB, HSL, OKLCH):** Track height 16dp with continuous rounded pill ends. Active thumb is a 24dp elevated circle (`surface`) with dynamic inner fill corresponding to the live selected tone.

### Palette Swatch Cards
- Interactive canvas swatches span full width (compact) or columns (expanded). Each swatch contains actionable overlay pills for locking state, contrast status, and hex value copying. Reordering utilizes smooth physics-based drag-and-drop elevation shifts.
---
name: Apex Telemetry Rally
colors:
  surface: '#111317'
  surface-dim: '#111317'
  surface-bright: '#37393e'
  surface-container-lowest: '#0c0e12'
  surface-container-low: '#1a1c20'
  surface-container: '#1e2024'
  surface-container-high: '#282a2e'
  surface-container-highest: '#333539'
  on-surface: '#e2e2e8'
  on-surface-variant: '#e4beb2'
  inverse-surface: '#e2e2e8'
  inverse-on-surface: '#2f3035'
  outline: '#aa897e'
  outline-variant: '#5b4138'
  surface-tint: '#ffb59b'
  primary: '#ffb59b'
  on-primary: '#5b1a00'
  primary-container: '#ff5e14'
  on-primary-container: '#541800'
  inverse-primary: '#a93800'
  secondary: '#ffdb9d'
  on-secondary: '#412d00'
  secondary-container: '#feb700'
  on-secondary-container: '#6b4b00'
  tertiary: '#00e297'
  on-tertiary: '#003822'
  tertiary-container: '#00a86f'
  on-tertiary-container: '#00331f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdbcf'
  primary-fixed-dim: '#ffb59b'
  on-primary-fixed: '#380d00'
  on-primary-fixed-variant: '#812900'
  secondary-fixed: '#ffdea8'
  secondary-fixed-dim: '#ffba20'
  on-secondary-fixed: '#271900'
  on-secondary-fixed-variant: '#5e4200'
  tertiary-fixed: '#4dffb2'
  tertiary-fixed-dim: '#00e297'
  on-tertiary-fixed: '#002112'
  on-tertiary-fixed-variant: '#005234'
  background: '#111317'
  on-background: '#e2e2e8'
  surface-variant: '#333539'
  surface-card: '#181B21'
  surface-card-elevated: '#21262F'
  border-grid: '#2B323D'
  text-radar-dim: '#717D91'
  hazard-stripe: '#E53E3E'
typography:
  headline-xl:
    fontFamily: Chivo
    fontSize: 36px
    fontWeight: '900'
    lineHeight: 44px
  headline-xl-mobile:
    fontFamily: Chivo
    fontSize: 28px
    fontWeight: '900'
    lineHeight: 34px
  headline-lg:
    fontFamily: Chivo
    fontSize: 24px
    fontWeight: '800'
    lineHeight: 32px
  headline-md:
    fontFamily: Chivo
    fontSize: 20px
    fontWeight: '800'
    lineHeight: 28px
  headline-sm:
    fontFamily: Chivo
    fontSize: 16px
    fontWeight: '700'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-lg:
    fontFamily: Space Mono
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 18px
  label-md:
    fontFamily: Space Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
  label-sm:
    fontFamily: Space Mono
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 14px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-mobile: 0.75rem
  margin: 1.5rem
  margin-mobile: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
---

## Brand & Style

This design system translates the raw, high-stakes adrenaline of rally motorsport and tactical scavenger tracking into an aggressive, digital-first mobile telemetry interface. Rooted in competition, speed, and real-time field navigation, it rejects passive form design in favor of an active "co-pilot cockpit" ethos. 

The aesthetic is a hybrid of **Tactile High-Contrast** and **Motorsport Telemetry HUD**. It features ultra-dark graphite and asphalt backdrops, angled visual cuts, mechanical chamfers, luminous warning lamps, and military-grade cockpit data readouts. It evokes the urgency of a competitive rally stage: bold, direct, razor-sharp, and built to remain legible under direct outdoor sunlight or in moving vehicles.

## Colors

The palette is engineered around high-contrast optical beacons against light-absorbing tarmac surfaces:

- **Primary (`#FF5E14`) - Rally Orange**: Used for critical action anchors, active telemetry accents, stage start markers, and high-priority primary triggers.
- **Secondary (`#FFB800`) - Racing Amber / Tach Yellow**: Communicates pending checkpoints, active timing markers, standby status, and secondary navigational aids.
- **Tertiary (`#00E599`) - Verified Telemetry Green**: Denotes authenticated GPS lock, validated zone codes, clean split times, and mission checkpoints cleared.
- **Neutral (`#0F1115`) - Deep Asphalt / Graphite**: The deep, low-reflective cockpit ground. Avoid pure absolute black (`#000000`) except for recessed numerical cutouts.

Named semantic tokens include `surface-card` and `surface-card-elevated` for cockpit instruments, `border-grid` for crisp mechanical separations, and `text-radar-dim` for secondary technical telemetry copy.

## Typography

The typography strategy pairs industrial velocity with instrument-panel precision:

- **Headlines (Chivo)**: Heavy, aggressive, and aerodynamic. Used with uppercase tracking for section callouts, zone identifiers (`ZONA 01`), and stage milestones.
- **Data & Telemetry (Space Mono)**: Monospaced, technical, and tabular. Used for codes, coordinates, zone indexes (`[01/09]`), time splits, status indicators, and tactical input labels.
- **Interface & Prose (Inter)**: Clean, balanced, neutral grotesque. Delivers high-density readability for game rules, instructions, disclaimers, and hint callouts.

## Layout & Spacing

Layout conforms to a single-column, tactical feed architecture optimized for one-thumb field operation on mobile devices.

- **Grid & Alignment**: A 4-column fluid mobile grid upgrading to an 8-column tablet structure. The maximum layout container width is capped at 640px to mirror an automotive digital cluster or handheld rally computer.
- **Rhythm**: Vertical rhythm operates strictly on multiples of `0.5rem` (8px). Sections are demarcated by pronounced spacing (`space-xl`), while interactive checkpoint fields utilize tight mechanical internal padding (`space-md`).
- **Telemetry Header**: A sticky HUD pinned to the viewport top monitors overall progress (`ZONAS VALIDADAS: X / 09`) and quick-launch shortcuts without obscuring active input cards.

## Elevation & Depth

This system intentionally departs from soft, organic drop shadows, instead using **mechanical surface layering, hard ambient glow, and technical borders**:

- **Ground Level (Canvas)**: `#0F1115` matte asphalt finish.
- **Instrument Pods (Cards)**: Surface containers `#181B21` bound by crisp `1px` structural borders (`#2B323D`). 
- **Active State / Focused Element**: Border switches to `#FF5E14` with a tight, intense colored halo: `box-shadow: 0 0 12px rgba(255, 94, 20, 0.35)`.
- **Validated Checkpoint**: Border switches to `#00E599` with a glowing trace: `box-shadow: 0 0 12px rgba(0, 229, 153, 0.25)`.
- **Physical Depth**: Input fields use inset borders and a recessed, darker background (`#0A0B0E`) to simulate cockpit instrument displays.

## Shapes

Shapes reflect precision-machined industrial components:

- Structural elements maintain strict compact radii (`0.25rem` / `rounded-sm`) to avoid soft, toy-like forms.
- Buttons, zone headers, and badge indicators can incorporate mechanical chamfered / clipped corners (45-degree angled cuts of 6px to 8px via CSS clip-path) to reinforce the vehicle telemetry and carbon-chassis identity.

## Components

### Buttons & Telemetry Triggers
- **Primary Action (Stage Submit / Start)**: Heavy rectangular or chamfered block, solid `#FF5E14` fill, dark `#0F1115` bold typography (`Chivo`), uppercase with `letter-spacing: 0.05em`. Hover/Active produces a high-intensity orange optical surge.
- **GPS Shortcut / Launch Trigger**: Outlined secondary style with `#FFB800` border, glowing amber icon, and monospaced auxiliary label (`LAUNCH FAREJADOR GPS [EXT]`).
- **Destructive / Reset Action**: Subtle `ghost` button with muted gray text (`#717D91`), turning `#E53E3E` only on intentional touch state.

### Zone Checkpoint Cards (Zones 01 to 09)
- Structured as modular rally roadbook units.
- **Card Header**: Displays stage indicator (`ZONA 04 // PISTA`), checkpoint coordinates or clue prompt, and a real-time status pill (`PENDING`, `LOCKED`, or `VALIDATED`).
- **Accent Stripe**: Left-border color bar (4px thick): neutral gray for unreached zones, pulsing yellow for the current target, and solid neon green (`#00E599`) for submitted and verified zones.

### Input Fields (Code Entry)
- Recessed `#0A0B0E` background with a monospaced uppercase character display (`Space Mono`).
- Prefix block showing prompt icon or terminal bracket `>`.
- Generous touch target (min 48px height) with high visual contrast to ensure effortless thumb entry while navigating outdoors.

### Progress HUD Tracker
- Pinned horizontal dashboard component showing segmented bar blocks (1 through 9).
- Completed segments fill with `#00E599`; active segments flash with `#FFB800`; remaining segments stay muted `#2B323D`.

### Badges & Status Chips
- High-contrast, micro-monospaced labels wrapped in ultra-fine borders with semi-transparent tinted backgrounds (`rgba(255, 184, 0, 0.1)`).
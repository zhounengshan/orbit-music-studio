---
name: Orbit Music
description: A true-black, content-first personal music workspace built around a persistent playback desk.
colors:
  true-black: "#000000"
  surface: "#111111"
  raised: "#222222"
  active: "#1b1b1b"
  border: "#1a1a1a"
  rule: "#181818"
  control-border: "#454545"
  text-primary: "#ffffff"
  text-muted: "#b7b7b7"
  text-faint: "#929292"
  signal-orange: "#ff5a36"
  negative: "#e5566f"
typography:
  headline:
    fontFamily: "Inter, Noto Sans SC, system-ui, sans-serif"
    fontSize: "24px"
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: "-0.025em"
  title:
    fontFamily: "Inter, Noto Sans SC, system-ui, sans-serif"
    fontSize: "20px"
    fontWeight: 700
  body:
    fontFamily: "Inter, Noto Sans SC, system-ui, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "Inter, Noto Sans SC, system-ui, sans-serif"
    fontSize: "12px"
    fontWeight: 500
rounded:
  cover: "4px"
  kbd: "5px"
  media: "6px"
  control: "8px"
  panel: "20px"
  pill: "999px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "14px"
  lg: "22px"
  xl: "28px"
  2xl: "34px"
components:
  button-primary:
    backgroundColor: "{colors.text-primary}"
    textColor: "{colors.true-black}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "40px"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.text-muted}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 14px"
    height: "34px"
  input-search:
    backgroundColor: "#171717"
    textColor: "{colors.text-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "0 3px 0 12px"
    width: "min(620px, 100%)"
    height: "38px"
  nav-item:
    backgroundColor: "transparent"
    textColor: "{colors.text-muted}"
    rounded: "{rounded.control}"
    padding: "0 10px"
    height: "40px"
  nav-item-active:
    backgroundColor: "{colors.active}"
    textColor: "{colors.text-primary}"
    rounded: "{rounded.control}"
    padding: "0 10px"
    height: "40px"
  track-row:
    backgroundColor: "transparent"
    textColor: "{colors.text-primary}"
    padding: "8px 14px"
    height: "76px"
  track-row-current:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.text-primary}"
    padding: "8px 14px"
    height: "76px"
  transport-play:
    backgroundColor: "{colors.text-primary}"
    textColor: "{colors.true-black}"
    rounded: "{rounded.pill}"
    size: "38px"
  persistent-player:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.text-primary}"
    padding: "0 22px"
    height: "92px"
  lyrics-surface:
    backgroundColor: "#0a0a0a"
    textColor: "{colors.text-primary}"
    width: "calc(100vw - 224px)"
    height: "calc(100dvh - 92px)"
  dialog-card:
    backgroundColor: "#181818"
    textColor: "{colors.text-primary}"
    rounded: "{rounded.panel}"
    padding: "28px"
    width: "min(420px, 100%)"
  toast:
    backgroundColor: "{colors.text-primary}"
    textColor: "{colors.true-black}"
    rounded: "{rounded.pill}"
    padding: "11px 16px"
---

# Design System: Orbit Music

## Overview

**Creative North Star: "The Listening Desk"**

Orbit Music is a true-black, flat personal listening workspace. Search, the active library context, real track rows, synchronized lyrics, and playback controls occupy the first useful viewport; there is no promotional hero competing with the music task.

The persistent playback desk is the visual and interaction anchor. White carries ordinary primary actions, signal orange reports live playback and selected status, and album covers provide the richest color. On phones, navigation and lyrics become intentional full-screen surfaces rather than compressed desktop columns.

**Key Characteristics:**

- True-black ground with flat charcoal separation and one-pixel rules.
- White primary actions; orange reserved for playback and state.
- Real music content and cover art carry visual identity.
- Persistent player across desktop, tablet, and phone.
- Search-first composition with honest empty, loading, and error states.
- Full-screen mobile navigation and lyrics with 44px primary touch targets.

## Colors

The palette is deliberately achromatic so metadata stays legible and album artwork remains the expressive layer; signal orange appears only when the interface needs to communicate live music or state.

### Primary

- **Signal Orange:** Live playback markers, selected favorites, range progress, the brand orbit, and other explicit status signals.

### Neutral

- **True Black:** The page, sidebar, and strongest visual silence.
- **Surface:** The persistent player and current-track background.
- **Raised:** Hovered icon controls, close controls, and compact mobile utility surfaces.
- **Active:** Selected navigation rows.
- **Border / Rule:** Structural edges and track-row separators; these replace shadows.
- **Control Border:** Visible outlines for secondary buttons and selectors.
- **Primary Text:** High-priority copy and white primary actions.
- **Muted Text:** Artists, albums, helper copy, and resting controls.
- **Faint Text:** Table labels, timestamps, counts, and tertiary notes.

### Functional

- **Negative:** Destructive library-management actions only.

### Named Rules

**The Signal, Not Paint Rule.** Orange reports playback or state; it never becomes a large background, gradient, glow, or decorative wash.

**The Cover Art Owns Color Rule.** Keep application chrome achromatic so real album covers remain the richest color on screen.

## Typography

**Headline and Body Font:** Inter (with Noto Sans SC and system-ui fallbacks)

**Character:** The single sans-serif family is compact, direct, and neutral. Slightly tightened headings establish hierarchy without turning the workspace into an editorial poster; metadata uses weight and gray value instead of multiple typefaces.

### Hierarchy

- **Headline:** Active search, library, favorites, download, and playlist contexts.
- **Title:** Empty states, dialogs, track details, and lyric identity.
- **Body:** Explanatory copy and standard interface text.
- **Label:** Table headers, quality badges, counts, timestamps, and compact controls.

### Named Rules

**The Metadata Steps Back Rule.** Track identity leads; artist, album, duration, source, and helper copy recede through muted or faint text.

**The Interface Speaks Briefly Rule.** Use short, literal labels and status messages; typography clarifies work rather than selling the product.

## Layout

Desktop uses a fixed 224px library sidebar and a fluid main workspace above a persistent 92px player. The top bar is 64px high; the scrollable content area uses 28px horizontal padding and caps its music view at 1320px. Track rows form a six-column desktop table with a 76px working rhythm.

Below 980px the sidebar becomes a full-height navigation sheet with a dimmed scrim. Below 700px the player compresses to 76px, search becomes a three-part compact control, tracks become two-line rows with visible 44px actions, and secondary metadata collapses before music identity or playback.

Lyrics open above the workspace as a dedicated reading surface: two columns on desktop, edge-to-edge on phone. The content surface never makes room for a campaign hero; the first viewport always answers the current music task.

**The First Viewport Works Rule.** Search, navigation, the list or empty state, and the playback desk must be immediately usable without scrolling past promotional content.

## Elevation & Depth

This is a shadow-free system. Depth comes from adjacent true-black and charcoal fills, one-pixel borders, opaque overlays, and state changes. The modal backdrop and mobile navigation scrim dim the underlying workspace without blur, glass, glow, or gradients.

### Named Rules

**The Flat Means Flat Rule.** Do not add box shadows, glass effects, gradients, or glow; use fill, rule, and visibility changes to communicate layers.

## Shapes

The form language is precise and functional. Album covers use small corners, rectangular fields and dialogs use restrained rounding, and compact controls use full pills or circles. The large panel radius belongs to modal cards, not every container.

**The Pill Is a Control Rule.** Pills identify actionable controls, filters, range-adjacent tools, and transient feedback; content rows and page regions remain rectilinear.

## Components

### Buttons

- **Primary:** White fill with black text; used for search, empty-state recovery, and confirmation.
- **Secondary:** Transparent black-ground control with a visible gray border and muted copy; hover brightens border and text.
- **State:** Orange communicates selected or playing state, not ordinary primary action.
- **Focus:** All interactive elements receive a 2px white outline with a 3px offset.

### Inputs / Fields

- **Search:** A compact dark pill with search icon, flexible input, optional shortcut hint, and white action button.
- **Modal Field:** A rectangular dark field with a visible control border and 8px corners.
- **Range:** Native range controls use signal orange for current progress or volume.

### Navigation

Navigation rows are 40px tall, quiet at rest, and filled with the active neutral when selected. Counts align right with tabular numerals. Below 980px the entire rail becomes a scrim-backed sheet and inactive off-canvas content is removed from keyboard navigation.

### Track Rows

Track rows are the core working component: 76px on desktop with artwork, title, artist, album, quality, duration, and actions. The current row gains a flat surface and a 2px orange edge marker. On phone, each row becomes a compact identity-and-actions composition; play, favorite, download, and management actions remain 44px where shown.

### Persistent Player

The player is a stable three-zone desk: current track, centered transport and progress, and right-aligned tools. The main play control is a white circle; orange belongs to live progress and selected state. On phone, the player reduces to track identity, lyrics, play/pause, next, and a full-width progress hit area.

### Lyrics

Lyrics are an on-demand reading surface, hidden and inert at rest. Opening moves focus to the close control; Escape or close returns focus to the player trigger. The active lyric is white while surrounding lines recede; mobile lyrics fill the screen with cover and track identity compacted above the reading flow.

### Dialogs & Toasts

Dialogs use a true-black backdrop, a charcoal card, restrained rectangular inputs, and a white confirmation action. Keyboard focus is trapped inside until dismissal. Toasts use a compact white pill above the player and animate only opacity plus a short vertical translation.

## Do's and Don'ts

### Do:

- **Do** keep search, playback, lyrics, and library actions visible and immediate.
- **Do** let album covers and real music metadata provide visual richness.
- **Do** keep orange scarce and tied to live playback or explicit state.
- **Do** preserve 44px mobile actions, visible focus, inert off-canvas surfaces, and focus return.
- **Do** collapse secondary metadata before compressing track identity or playback.
- **Do** honor reduced-motion preferences for sheets, lyrics, and transient feedback.

### Don't:

- **Don't** add a poster-style hero, campaign copy, decorative equalizer, or cassette illustration.
- **Don't** introduce gradients, glass, glow, ambient orange, or ornamental shadows.
- **Don't** fabricate recommendations, testimonials, audience metrics, or listening statistics.
- **Don't** use orange for ordinary primary buttons when white already communicates action.
- **Don't** treat the phone as a squeezed desktop table.
- **Don't** hide essential playback or library actions behind undersized targets.

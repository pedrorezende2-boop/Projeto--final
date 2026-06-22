---
name: Frenchy Design System
colors:
  surface: '#141122'
  surface-dim: '#141122'
  surface-bright: '#3a374a'
  surface-container-lowest: '#0e0c1d'
  surface-container-low: '#1c192b'
  surface-container: '#201d2f'
  surface-container-high: '#2a283a'
  surface-container-highest: '#353245'
  on-surface: '#e5dff8'
  on-surface-variant: '#c6c4d9'
  inverse-surface: '#e5dff8'
  inverse-on-surface: '#312e40'
  outline: '#908fa2'
  outline-variant: '#454556'
  surface-tint: '#c0c1ff'
  primary: '#c0c1ff'
  on-primary: '#0c00aa'
  primary-container: '#2f2fe4'
  on-primary-container: '#bdbfff'
  inverse-primary: '#3f42f1'
  secondary: '#bac3ff'
  on-secondary: '#04228a'
  secondary-container: '#273ca0'
  on-secondary-container: '#a3b0ff'
  tertiary: '#ffb4a1'
  on-tertiary: '#611300'
  tertiary-container: '#9b2400'
  on-tertiary-container: '#ffb19d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#04006d'
  on-primary-fixed-variant: '#201cdb'
  secondary-fixed: '#dee1ff'
  secondary-fixed-dim: '#bac3ff'
  on-secondary-fixed: '#001159'
  on-secondary-fixed-variant: '#273ca0'
  tertiary-fixed: '#ffdbd2'
  tertiary-fixed-dim: '#ffb4a1'
  on-tertiary-fixed: '#3c0800'
  on-tertiary-fixed-variant: '#891f00'
  background: '#141122'
  on-background: '#e5dff8'
  surface-variant: '#353245'
  surface-elevated: '#1A1953'
  text-primary: '#FFFFFF'
  text-secondary: '#9CA3AF'
  border-subtle: '#2F2FE433'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '800'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 28px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 22px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-lg:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '600'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '600'
    lineHeight: 18px
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  margin-mobile: 1rem
  gutter-mobile: 0.75rem
  stack-sm: 0.25rem
  stack-md: 0.5rem
  stack-lg: 1rem
  feed-gap: 1px
---

## Brand & Style

The design system is built for a fast-paced, real-time microblogging environment. It prioritizes information density and immediate legibility, catering to a global audience that demands professional yet modern aesthetics.

The visual style is **Minimalist / High-Contrast**, drawing inspiration from contemporary social platforms. It emphasizes a "content-first" philosophy through a dark-mode-centric interface, where the deep navy and black backgrounds allow vibrant blue accents and crisp white text to command attention. The aesthetic is sleek and precise, utilizing thin borders and strategic whitespace to organize complex streams of data without visual clutter.

## Colors

The color palette is anchored in a "Deep Dark" spectrum to reduce eye strain during prolonged scrolling. 

- **Primary (#2F2FE4):** Used for high-priority actions like "Post," active navigation states, and verified badges.
- **Secondary (#162E93):** Employed for secondary buttons or hovered states of primary elements.
- **Dark (#1A1953):** Serving as the elevated surface color for cards, modals, or nested threaded conversations.
- **Background (#080616):** The base canvas color, providing a rich, high-contrast foundation for the entire UI.

Text should primarily be white (#FFFFFF) for maximum readability, with a muted gray (#9CA3AF) used for timestamps, handles, and metadata.

## Typography

This design system utilizes **Inter** for its exceptional legibility and neutral, systematic feel. Since microblogging relies on short-form content, the type scale is tight and efficient.

- **Headlines:** Use heavy weights (700-800) with slight negative letter-spacing for a bold, "breaking news" feel.
- **Body:** The standard post size is `body-md` (15px), optimized for the high density of a mobile feed.
- **Labels:** Used for navigation items, buttons, and metadata. `label-md` is often used for section headers or secondary actions to provide clear hierarchy.

## Layout & Spacing

The layout follows a **Fluid Grid** model optimized for mobile-first consumption.

- **Feed Architecture:** Posts are separated by a 1px border (`border-subtle`) rather than large gaps, maximizing vertical space.
- **Margins:** A consistent 16px (1rem) side margin is maintained for all main content.
- **Hierarchy:** Use `stack-md` (8px) for internal component spacing (e.g., between a username and the post text) and `stack-lg` (16px) for major section breaks.
- **Touch Targets:** All interactive elements must maintain a minimum 44x44px touch area, even if the visual asset is smaller.

## Elevation & Depth

This system avoids traditional shadows to maintain a sleek, modern aesthetic. Instead, it uses **Tonal Layers** and **Low-Contrast Outlines**.

- **Level 0 (Base):** The Background color (#080616).
- **Level 1 (Surface):** The Dark color (#1A1953) for items that need to sit "above" the feed, such as bottom sheets or floating search bars.
- **Borders:** 1px solid strokes are the primary method of separation. Use the Primary color at 20% opacity for a subtle, tech-forward "glow" effect on borders without adding physical weight.

## Shapes

The design system uses **Soft** roundedness to balance the aggressive high-contrast color palette.

- **Standard Elements:** Buttons and input fields use a 0.25rem (4px) radius.
- **Containers:** Post cards and media attachments use a 0.5rem (8px) radius to softly frame user-generated content.
- **Avatars:** User profiles are strictly circular (pill-shaped) to distinguish people from content containers.

## Components

- **Buttons:** 
  - **Primary:** Solid #2F2FE4 with White text. Bold weight.
  - **Secondary:** Outlined with Primary color or solid #162E93.
- **Chips:** Small, #1A1953 background with `label-sm` text for categories or hashtags.
- **Input Fields:** Dark (#1A1953) background with a 1px border that turns #2F2FE4 on focus.
- **Lists/Feed Items:** Minimalist items with a 1px bottom border. Interaction states (hover/tap) should trigger a subtle background highlight of #1A1953.
- **Cards:** Used sparingly for quoted posts or link previews, featuring a thin border and 8px corner radius.
- **Icons:** Use linear, 2px stroke icons. Active navigation states may transition to solid "filled" versions of the same icon set.
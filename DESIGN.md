---
name: AIOS Clínicas Landing
description: Premium operations layer for Brazilian medical clinics — landing voice as a clinic director's signed report.
colors:
  background: "#FFFFFF"
  surface: "#F8F8FA"
  surface-sec: "#EFEFF2"
  foreground: "#0E0F14"
  muted: "#5C5C66"
  muted-soft: "#878793"
  border: "#E5E5EA"
  border-strong: "#D0D0D8"
  signature-ink: "#1A8FA0"
  signature-ink-deep: "#147280"
  signature-ink-soft: "#E7F4F8"
  signature-ink-archive: "#0A4F65"
  aios-green: "#338A60"
  aios-green-soft: "#EBF7F0"
  aios-magenta: "#C73A60"
  aios-magenta-soft: "#FBE9EE"
typography:
  display:
    fontFamily: "Bricolage Grotesque, system-ui, sans-serif"
    fontSize: "clamp(2.75rem, 5vw + 1rem, 3.75rem)"
    fontWeight: 800
    lineHeight: 0.96
    letterSpacing: "-0.05em"
    fontVariation: "'wdth' 100, 'opsz' 96, 'wght' 800"
  headline:
    fontFamily: "Bricolage Grotesque, system-ui, sans-serif"
    fontSize: "clamp(2rem, 3vw + 0.5rem, 3rem)"
    fontWeight: 800
    lineHeight: 1.02
    letterSpacing: "-0.035em"
  title:
    fontFamily: "Bricolage Grotesque, system-ui, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.025em"
  body:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "normal"
  label:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "0.6875rem"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "0.1em"
rounded:
  hairline: "4px"
  control: "8px"
  card: "12px"
  pill: "9999px"
spacing:
  hair: "1px"
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "48px"
  xl: "96px"
  xxl: "176px"
components:
  button-primary:
    backgroundColor: "{colors.signature-ink}"
    textColor: "{colors.background}"
    rounded: "{rounded.control}"
    padding: "0 24px"
    height: "44px"
  button-primary-hover:
    backgroundColor: "{colors.signature-ink-deep}"
    textColor: "{colors.background}"
  button-primary-active:
    backgroundColor: "{colors.signature-ink-deep}"
    textColor: "{colors.background}"
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.control}"
    padding: "0 24px"
    height: "44px"
  button-ghost-hover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.card}"
    padding: "32px"
  card-inverse:
    backgroundColor: "{colors.foreground}"
    textColor: "{colors.background}"
    rounded: "{rounded.card}"
    padding: "32px"
  eyebrow-pill:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.muted}"
    rounded: "{rounded.pill}"
    padding: "6px 12px"
  input:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.control}"
    padding: "10px 14px"
    height: "44px"
---

# Design System: AIOS Clínicas Landing

## 1. Overview

**Creative North Star: "The Clinic Director's Desk"**

The visual world is a clinic director's working desk at the end of a quiet afternoon: heavy uncoated paper, a fountain pen capped beside a signed report, a single screen showing only what matters. Decisions get *signed*, not announced. The system carries the same posture toward the visitor — calm, criterious, finished. Every CTA should feel like the director's signature: weighted, infrequent, conclusive.

The aesthetic is restrained but emphatically not gentle. Bricolage Grotesque at weight 800 with expanded width carries the headline like a letterhead pressed into the page; DM Sans body sets evidence at reading distance; JetBrains Mono labels mark margin annotations in a typewriter register, not a developer register. The single accent — a deep teal-cyan we call **Signature Ink** — appears only where the director would actually mark the page: a key noun, a stat that closes the argument, a primary CTA. Its rarity is the point.

This system explicitly rejects the SaaS landing-page reflexes (three icon-title cards, centered hero stack, generic illustrations) and pharma-clinic reflexes (azul-pharma, smiling stock photography, red cross iconography). It also rejects tech-bro IA tropes (purple gradients, neon glow, mascot robots) and editorial-magazine pastiche (Fraunces italic, drop caps, broadsheet rules).

**Key Characteristics:**

- Generous left-aligned hierarchy; centered hero stacks are template territory.
- Bricolage Grotesque at 800 weight, expanded width — letterhead, not display-serif elegance.
- Hairline borders (1px) doing the work that drop shadows usually do; cards earn shadows only when elevation is functional.
- Signature Ink (teal-cyan, HSL 187 72% 36%) is load-bearing and rare — used as ink, not as paint.
- Mono labels in typewriter register, never as developer-tech shorthand.
- Numbers are bottom-line; copy is verb-spare and never imperative.

## 2. Colors

A near-white warm-neutral surface holding warm-black type, ruled with cool hairlines, signed in a single teal-cyan ink. The palette is **Restrained** by Stitch's taxonomy, but the Signature Ink is treated as Committed in the moments it appears.

### Primary

- **Signature Ink** (`#1A8FA0` / `hsl(187 72% 36%)`): The one ink the director uses. Appears on the primary CTA, on the eyebrow status dot, on the single accent word inside the H1 (`<em class="not-italic">`), on the active state of stats badges, and on integration accent strokes. Never used for decorative gradient fills. Never used as a background on more than 8% of any fold.
- **Signature Ink Deep** (`#147280` / `hsl(187 72% 28%)`): Hover and pressed state for the primary CTA. The pen pressing harder into the paper.
- **Signature Ink Soft** (`#E7F4F8` / `hsl(187 72% 95%)`): Used exclusively as the fill behind floating badges and inline icon backgrounds. Never as a full-section wash. Carries the ink's hue at low chroma.
- **Signature Ink Archive** (`#0A4F65` / `hsl(192 80% 22%)`): The darkest form of the ink, reserved for charts, data viz, and any inverse-on-foreground placement where the ink needs to remain visible.

### Neutral

- **Background** (`#FFFFFF` / `hsl(0 0% 100%)`): The paper. Always.
- **Surface** (`#F8F8FA` / `hsl(240 6% 97.5%)`): Cards, eyebrow pills, secondary nav backgrounds. A second sheet of paper laid behind the first.
- **Surface Sec** (`#EFEFF2` / `hsl(240 6% 94%)`): Hover state for cards, ledger blocks, integration tiles. The carbon-copy beneath.
- **Foreground** (`#0E0F14` / `hsl(240 10% 6%)`): All primary type, the AIOS logo glyph, inverse cards. Warm-black, not pure black. The fountain-pen ink.
- **Muted** (`#5C5C66` / `hsl(240 5% 38%)`): Body paragraphs, supporting copy, mono labels. Must hold ≥ 4.5:1 contrast against Background.
- **Muted Soft** (`#878793` / `hsl(240 5% 55%)`): Annotation-only — caption text, mono stat suffixes, helper text under inputs. Never used for primary reading text.
- **Border** (`#E5E5EA` / `hsl(240 6% 90%)`): The ruled lines of the ledger. Every separator. Default hairline.
- **Border Strong** (`#D0D0D8` / `hsl(240 6% 82%)`): Used only when a hairline is competing with surface tint and needs to win. Rare.

### Secondary Logo-Bridge Accents

The official AIOS logo carries a vibrant gradient (magenta · green · navy). Two desaturated colors are pulled from that gradient and used **strictly as semantic micro-accents** — never as paint, never as primary chrome. They exist to create discreet visual bridges between the logo and the page without breaking the Restrained color strategy.

- **AIOS Green** (`#338A60` / `hsl(150 50% 38%)`): Used exclusively where the meaning is **human or money-positive** — the "100% Humano" stat in the Gestor CRM section, the "+R$ 18k" testimonial outcome. Never on chrome, CTAs, or backgrounds.
- **AIOS Magenta** (`#C73A60` / `hsl(348 60% 48%)`): Used exclusively to **mark distinction** — the "Recomendado" badge on the Clínica Pro pricing tier. Never as a background wash, never on body text.

Both colors carry soft variants (`-soft`, ~95% lightness) reserved for icon-tile backgrounds analogous to `signature-ink-soft`.

### Named Rules

**The One Ink Rule.** The Signature Ink appears on no more than ~8% of any visible viewport. If three accent uses are already in frame, the fourth must defer to Foreground or Muted. Saturation of ink is what gives it authority — abundance dilutes it.

**The Three-Color Maximum Rule.** In any given viewport, no more than three named accent colors may appear (Signature Ink + at most one of: AIOS Green, AIOS Magenta). The logo-bridge accents are micro-semantic, not co-equal with the Ink. A page that uses all three at once breaks the Restrained strategy.

**The No-Pharma-Blue Rule.** Healthcare-blue (`#0066CC`, `#3B82F6`, any cobalt) is forbidden. The Signature Ink is deliberately teal-cyan to escape the pharma association. If a screenshot in the page contains pharma-blue UI, mute it via opacity or replace it.

**The Warm-Black Rule.** `#000000` is banned. Foreground is `#0E0F14` (HSL 240 10% 6%) — a warm-tinted near-black. Borders, dividers, and mono labels all derive from the same warm neutral hue family (240, 5-6% saturation).

## 3. Typography

**Display Font:** Bricolage Grotesque (with system-ui fallback)
**Body Font:** DM Sans (with system-ui fallback)
**Label/Mono Font:** JetBrains Mono (with ui-monospace fallback)

**Character:** Bricolage at weight 800 with expanded width (`wdth: 100`, `opsz: 96`) is the director's letterhead — large, structural, opinionated, never decorative. DM Sans body is the prose of a signed report: legible, neutral, generous in line-height. JetBrains Mono labels are typewriter margin notes — not developer chrome. The three families never overlap roles.

### Hierarchy

- **Display** (Bricolage Grotesque, weight 800, `clamp(2.75rem, 5vw + 1rem, 3.75rem)`, line-height 0.96, letter-spacing -0.05em): H1 only. Hero headline. Used exactly once per page.
- **Headline** (Bricolage Grotesque, weight 800, `clamp(2rem, 3vw + 0.5rem, 3rem)`, line-height 1.02, letter-spacing -0.035em): H2 section openers. May also appear as DM Sans semibold at scale `text-3xl md:text-4xl` for softer section transitions — the editorial choice is intentional.
- **Title** (Bricolage Grotesque, weight 800, 20-22px, line-height 1, letter-spacing -0.025em): Card titles and Bento tile headers. Tight, declarative.
- **Body** (DM Sans, weight 400, 17px, line-height 1.55, max-width 65ch): Hero lead, paragraph copy, section explanatory text. Always capped at 65ch. Mobile minimum 16px.
- **Label** (JetBrains Mono, weight 500, 10-11px, letter-spacing 0.1em, UPPERCASE): Stat captions, eyebrow text, integration source labels, badge categories. Never used for sentences.

### Named Rules

**The Letterhead Rule.** H1 is Bricolage at weight 800 with expanded width. No exception. No alternative serif. No italic. The single permitted accent inside H1 is a `<em class="not-italic">` switching the type color to Signature Ink — that is the director's pen circling the load-bearing noun.

**The No-Inter Rule.** Inter is forbidden, even via fallback. The fallback chain is `system-ui, sans-serif` — never Inter explicitly.

**The Typewriter Mono Rule.** Mono is used in margin-annotation register — stat captions, eyebrow lines, integration source labels. Mono is never used for primary CTAs, body paragraphs, or technical-tech-bro signaling ("</code>", "$ npm install" theatrics on the landing). If a section uses mono for any sentence-length copy, it's miscast.

**The 65ch Body Rule.** Paragraph elements default to `max-width: 65ch`. The hero lead caps at 55ch for tighter framing. Long-form copy that needs more width must be opted-in by class (`p.full`).

## 4. Elevation

The system is **flat with intentional weighting** — depth is conveyed primarily through hairline borders and tonal surface shifts, not through ambient shadows. Floating elements (badges, the inverse metric pill, signed-result cards) earn a shadow only when their function is "this paper sits on top of the desk."

### Shadow Vocabulary

- **glass** (`box-shadow: 0 1px 2px 0 rgba(20, 24, 30, 0.04), 0 1px 0 0 rgba(20, 24, 30, 0.03) inset`): Default for input fields and pinned navigation bars. The barest hint of edge — a sheet of paper pressed against the desk, no gap.
- **soft** (`box-shadow: 0 1px 2px rgba(20, 24, 30, 0.04), 0 6px 24px -10px rgba(20, 24, 30, 0.08)`): Inline content cards and tertiary surfaces. A loose sheet resting on the desk.
- **card** (`box-shadow: 0 1px 3px rgba(20, 24, 30, 0.04), 0 8px 32px -16px rgba(20, 24, 30, 0.12)`): Floating badges, dialog headers, the inverse metric pill. A document lifted to be signed.
- **accent-subtle** (`box-shadow: 0 0 0 1px rgba(7, 158, 187, 0.08), 0 12px 32px -12px rgba(7, 158, 187, 0.18)`): Reserved for the single most important interactive element on a fold (the primary CTA in a high-priority section, the active integration tile). Tints the shadow with Signature Ink, never a generic gray.

### Named Rules

**The Flat-by-Default Rule.** Surfaces are flat at rest. Shadows appear only as a response to function — floating, hovering, signing — not as decoration. A card without a shadow is the default, not an exception.

**The Tinted-Shadow Rule.** When a shadow is used near the Signature Ink (e.g. on the primary CTA in hover), it is tinted with the ink (rgba(7, 158, 187, alpha)), never neutral gray. The ink touches everything it touches.

**The Ambient Glow Rule.** Cyan radial gradients are permitted only as ambient atmosphere fixed to the top/bottom of the page (`.ambient-glow-top`, `.ambient-glow-bottom`), with `pointer-events: none` and `z-index: 0`. They are background light, not foreground emphasis. Maximum two glows per page. Never on a card. Never animated.

## 5. Components

### Buttons

- **Shape:** Gently rounded rectangle (8px radius, the `control` token).
- **Primary:** Signature Ink background, Background text, 44px height, 24px horizontal padding. Used once per fold. The director's signature.
- **Hover:** Background shifts to Signature Ink Deep. Optional `accent-subtle` shadow on the highest-priority CTA only.
- **Active:** `transform: translateY(1px)` — the pen pressing into paper. Easing `cubic-bezier(.16,1,.3,1)`, duration 150ms.
- **Focus:** 2px solid Signature Ink ring, 2px offset, on `:focus-visible`. Never inset, never glow.
- **Ghost/Secondary:** Transparent background, 1px Border outline, Foreground text. Hover shifts border to Signature Ink and background to Surface. Used for "Diagnóstico gratuito" / supporting CTAs.

### Cards / Containers

- **Corner Style:** 12px radius (the `card` token). Larger radii (rounded-2xl, ~16px) only on the hero mockup frame and integration tiles where the visual weight needs to read as "device frame" or "tile."
- **Background:** Background (white) for primary cards, Surface for secondary, Foreground for inverse cards used to carry contrarian statements.
- **Shadow Strategy:** Flat by default. Apply `soft` only when the card is floating above content. Apply `card` only for floating overlapping mockup badges. Never apply both a strong shadow and a strong border — one or the other.
- **Border:** 1px Border by default. Border Strong only when a card sits against a Surface tint.
- **Internal Padding:** 32px (the `lg` spacing token) for primary content cards. 24px for compact tiles. Never < 16px.
- **Hover (when interactive):** Border shifts to Signature Ink at 40% opacity. Background shifts to Surface Sec. 300ms ease.

### Inputs / Fields

- **Style:** 1px Border stroke, Background fill, 8px radius, 44px height, 14px horizontal padding.
- **Focus:** Border shifts to Signature Ink. Optional `glass` shadow.
- **Label position:** Above the input, DM Sans 14px semibold Foreground.
- **Helper text:** Below the input, DM Sans 12px Muted Soft.
- **Error:** Border shifts to a desaturated warm red (`hsl(0 55% 50%)`), helper text adopts the same hue.

### Navigation

- **Style:** Fixed top, 56px height, `Background/80` with `backdrop-blur-md`, 1px Border bottom.
- **Logo:** 20x20 Foreground square with a 12x12 Signature Ink triangle in the bottom-right corner — the "signed" mark.
- **Links:** JetBrains Mono, 13-14px, Muted; hover shifts to Foreground in 200ms. No underline.
- **Primary CTA:** Compact 32px height variant of the primary button — Signature Ink background, Background text, 8px radius.
- **Mobile:** Links collapse into a slide-down panel; the primary CTA always remains visible.

### Eyebrow Pill

- **Style:** Border outline, Surface fill, rounded-full (`pill`), 6px×12px padding.
- **Composition:** 6px Signature Ink dot (pulse-soft animation) + JetBrains Mono 11px UPPERCASE Muted label.
- **Use:** Above H1 in the hero, above each H2 in major sections. A single label per fold.

### Stats Rail (signature component)

- **Style:** Full-width Border-y grid, 1-3 columns at md, each cell padded 28px × 24px.
- **Composition:** JetBrains Mono UPPERCASE 10px Muted caption + Bricolage Grotesque 800 weight 48-56px stat number + JetBrains Mono 11px Muted suffix.
- **Behavior:** Hairlines only — no card backgrounds, no shadows. The rail is "ledger lines" between bottom-line numbers.

### Floating Mockup Badges (signature component)

- **Style:** Background fill, 12px radius, 1px Border, `card` shadow, 8-10px padding.
- **Composition:** 32x32 Signature Ink Soft icon container + JetBrains Mono 9-10px UPPERCASE caption + DM Sans 12-13px Foreground value.
- **Animation:** `fade-in-up` on load with staggered delays (380ms, 540ms, 700ms). Reduced-motion fallback is the final static state.
- **Position:** Overlap the mockup edge by ~16-32px to break the rectangular frame.

## 6. Do's and Don'ts

### Do:

- **Do** lead H1 with a declarative statement followed by a Signature Ink `<em class="not-italic">` accent on the load-bearing noun. *"Sua clínica vende. A IA multiplica."* — the ink is on "multiplica."
- **Do** open every major section with a single eyebrow pill (status dot + Mono UPPERCASE 11px label) before the headline.
- **Do** use stats as evidence in their own ruled-line rail — `+40%`, `−68%`, `+340 clínicas`, `24/7`. Always with a Mono caption above and a Mono suffix beside.
- **Do** anchor the primary CTA in the right rail of the hero (asymmetric, not centered) with a paired ghost CTA labeled with action verb + Lucide icon.
- **Do** float two or three labelled metric badges over the product mockup to break the rectangular frame. Each badge: small Signature-Ink-Soft icon tile + Mono caption + value.
- **Do** preserve the warm-black `#0E0F14` Foreground everywhere. The warm tint is what makes the page feel like paper, not screen.
- **Do** keep paragraph bodies at `max-width: 65ch` (55ch in the hero lead).
- **Do** respect `prefers-reduced-motion` on every animation — marquee, fade-in-up, pulse-soft. Fallback is the final static state.

### Don't:

- **Don't** produce the SaaS-genérico-PT-BR pattern: centered hero stack, flat illustrations of smiling people, three identical icon-title-text cards in a row. This is the HubSpot / RD Station / Pipedrive / Bling reflex and it is forbidden.
- **Don't** produce the pharma-clinic pattern: azul-pharma (`#0066CC`, cobalt blues, generic medical blue), gradient-white backgrounds, stock photography of doctors in lab coats, cruz vermelha, estetoscópio icons. The Signature Ink is deliberately teal-cyan to escape this lane.
- **Don't** drift into tech-bro IA aesthetics: purple/lila gradients, neon glow, robot mascots, "Elevate / Unleash / Transform" verbs, animated mesh blobs. This is the 2024-2026 AI-tool slop.
- **Don't** ever use `#000000` — Foreground is `#0E0F14`, warm-black, always. Pure black is banned.
- **Don't** use Inter, Roboto, Arial, or generic system sans for display or body. The fallback chain is `system-ui, sans-serif` — never Inter explicitly.
- **Don't** stack three same-size cards horizontally with icon + heading + paragraph. Use 2-column zig-zag, asymmetric bento, or hairline-divided rows instead.
- **Don't** use border-left or border-right greater than 1px as a colored accent. Side stripes are forbidden.
- **Don't** apply `background-clip: text` with a gradient to headlines or hero text. The Signature Ink is solid, always.
- **Don't** use glassmorphism / backdrop-blur as decoration. Backdrop-blur is permitted only on the fixed top navigation (functional) and on the rare scrim under a modal.
- **Don't** use mono fonts for body or sentence-length copy. Mono is margin-annotation register only — labels, eyebrow text, stat captions, integration source names.
- **Don't** use the Signature Ink as a flat background fill on a card or section. The ink is ink, not paint. Maximum ~8% of viewport.
- **Don't** generate fake or generic names ("João da Silva", "Clínica Exemplo") or round numbers (`50%`, `100`, `999`). Use organic numbers (`+340 clínicas`, `−68%`, `+47 consultas`) and contextually-real Brazilian clinic names.
- **Don't** invent claims. Every stat on the page must trace to a real source. *"−68% no-show"* requires evidence; the legend "lembretes ativos" beneath it should hint at how the number was measured.

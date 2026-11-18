# Design system (redesign branch)

## Palette
One warm black ground for the whole page, so the photos carry the colour.

| Role | Value | Use |
|---|---|---|
| Canvas | `#0E0D0C` | Page background, everywhere |
| Raised | `#181614` | Image placeholders while loading |
| Text | `#ECE8E1` | Headings, body, links |
| Muted | `#A29C93` | Facts lines, captions, process notes (7:1 on canvas) |
| Line | `#2C2A27` | The one hairline above the contact details |
| Accent | `#E9B44C` | Interaction only: focus ring, text selection, hovered link underline |

No accent in static content. Link underlines rest at `#55504A` and turn amber on hover.

## Type
- Archivo (variable), hosted with the site in `fonts/` (SIL Open Font License). Latin and Latin Extended files; latin is preloaded.
- Section titles: 26–38px, weight 620, width 104, tracking -0.02em, balanced.
- Body: 16.5px / 1.62. Facts and captions: 13.5–14.5px, muted.
- Contact statement: 32–66px, weight 560, tracking -0.028em.
- Dates use tabular numerals.

## Layout
- Max width 1320–1640px (86vw), side padding 18–48px.
- Section head: title and facts in the left third, one short paragraph in the right two thirds. The header uses the same columns.
- Space between sections: 96–168px. No rules, no numbers, no containers.
- Poster pairs: photo and poster at equal height, sized to the viewport, process note beside them. On phones the pair becomes a swipe row with the note below.

## Components
- Text link / text button (`.tl`): underlined text, one SVG arrow icon set (stroke 1.7).
- Reel: 4:5 frame, caption below (title with arrow, role and date).
- Process note: label, first four lines faded, the rest on hover (desktop) or on "Read the process".
- Album strip: six square thumbnails, the last one shows "+N"; all open the lightbox.

## Motion
- Reels and the animated poster play continuously while on screen and pause off screen. Video files download only when near the screen. The background film keeps its pause button. Nothing autoplays with reduced motion on.
- One authored moment: text opening on hover (process notes, live photography text), 0.55s, exponential ease-out.
- Hover on images: slight brightening only.

## Phones
- Header shows the name, "About" (opens the intro) and the internship link. The poster section paragraph moves below the first photo and poster.

## Sharing
- Share image `img/og.jpg` (1200×630, first photo and poster), Open Graph tags, `favicon.svg`.

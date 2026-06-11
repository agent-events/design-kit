# Agent Events — brand assets

Mark concept: an agent run is an append-only **stream of events**. Three growing
nodes flow into a forward arrowhead (immutable progression); the lead node carries
a concentric "reasoning" ring signalling inference/compute — the AI cue.

Wordmark: Space Grotesk Medium, lowercase `agentevents`. Outlined to paths, so no
font dependency. Primary teal: #0F6E56 / #1D9E75 / #5DCAA5 / #9FE1CB.

## Files

SVG (vector, scalable):
- `agentevents-mark.svg`          — primary mark, no ring (clean default)
- `agentevents-mark-ring.svg`     — primary mark with static reasoning ring
- `agentevents-mark-animated.svg` — pulsing ring, includes prefers-reduced-motion guard
- `agentevents-lockup.svg`        — mark + wordmark + tagline (light)
- `agentevents-lockup-dark.svg`   — lockup on dark surface
- `favicon-source.svg`            — detailed favicon (use >=48px)
- `favicon-source-small.svg`      — simplified favicon (use <=32px)

PNG (raster, in /png):
- `mark.png`, `mark-ring.png`     — logo, transparent bg
- `lockup.png`, `lockup@2x.png`, `lockup-dark.png`
- `favicon-16/32/48/64/180.png`   — 16/32 from simplified source, 48+ detailed

ICO:
- `favicon.ico`                   — multi-res 16/32/48 for legacy browsers

## Web embed (agentevents.dev <head>)

```html
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="icon" href="/favicon-source.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/favicon-180.png">
```

Modern browsers pick the SVG; legacy fall back to .ico; iOS uses the 180px PNG.
The SVG favicon stays sharp at any DPI. Note the SVG favicon uses the *detailed*
art — if you want the simplified mark below 32px, ship the small PNGs instead and
drop the SVG line.

## Animation note
`agentevents-mark-animated.svg` is for the site header/hero, not the favicon
(favicons don't reliably animate). Reduced-motion users get a static ring.

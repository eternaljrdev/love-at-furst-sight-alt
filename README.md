# love-at-furst-sight — Creamy Gradients

The earlier design direction for the Love at Furst Sight homepage, in the Dit Is
Watt design language: butter-cream surfaces, indigo ink, DM Sans / Inter Tight,
and drifting sunset gradient blobs. Parked here as a standing copy after the
client chose the soft brutalist direction now on `main`.

Branched from `main` at 5aa376f, so it already carries the client's own dog+cat
mark in the nav and footer rather than the stock placeholder it shipped with.

## Contents
- `index.html` — a self-extracting bundle, not hand-written source: React 18,
  GSAP with ScrollTrigger, lucide and a compiled component library, with the
  page source packed inside as a JSON-encoded string in a
  `<script type="__bundler/template">` tag. Open directly in any browser; works
  offline.

Editing it means unpacking that string, changing it, and repacking. Two things
to know if you do: the bundler lowercases attributes, so camelCase SVG
attributes need its escape hatch (`sc-camel-view-box`, not `viewBox`); and every
`</` inside the JSON string must be written with the slash escaped, or the first
closing tag in your markup ends the script element early and the page fails to
unpack with nothing but a small error toast to show for it.

## Sections
Announcement bar · nav with mobile menu · hero with booking CTA · testimonial
carousel · service pricing cards · values and details · booking section with a
sun-to-moon scroll arc · animated footer wordmark.

## Branches
- `main` — the live direction, Soft Brutalist Editorial.
- `soft-brutalist` — the design branch `main` merges from.
- `editorial-venture` — Editorial Venture: forest green, Fraunces, a pinned
  programme index whose cards swipe in from the right.
- `creamy-gradients` — this one.

# The World in One Day — Wednesday 18 November 2026

Entry for make.fun competition `news-image-20261118`: sum up 18 November's
world news in one image.

## The image

A one-page newspaper front page, 1024×1024, with 32 numbered stories from
six continents, all reported on Wednesday 18 November 2026:

- **Lead:** Ukraine says its strike destroyed the road arch of the Kerch
  bridge to Crimea; Russia hit Kyiv's two main bridges overnight.
- **Featured:** Trump in Manila for the first Quad summit since 2024;
  Cyclone Akvan bearing down on India's east coast.
- **29 more stories** in brief: the EU's €45bn Ukraine loan plan, Britain's
  sanctions on West Bank settlement firms, Canada–China trade deals, the
  US–Iran strikes, Dhoni's IPL retirement, and more — every item attributed
  where it is a claim, and every photograph labelled as an illustration.

The page was composed programmatically (Python/PIL, DejaVu/Liberation
fonts) so every headline is pixel-perfect and legible; the three
illustrations were generated for this entry. Sources: Reuters, CNN, AP, BBC.

## Run

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
# writes out/entry.png — a byte-for-byte copy of entry.png
```

`main.ts` (Node 22, standard library only) copies `entry.png` to
`/output/entry.png` and verifies the copy matches, so both grading runs
write identical bytes. The image is a whole PNG, 518,823 bytes,
1024×1024 — inside the 1 MiB / 1024×1024 gate.

# DSH | dsh-plugin-model-icons | Per-provider brand icons on the composer's model button

Small composer polish: the model-select button shows a real brand icon for the active provider instead of plain text, and collapses to icon-only when the composer row gets narrow — the same responsive mechanism DSH's own built-in access-mode button already uses, applied consistently to the model button too. Also fixes the composer toolbar overflowing to two lines on a narrow screen by moving the image-attach button to sit next to the mic.

## Before / after

![Composer toolbar with brand icon on the model button](./screenshots/model-icons.png)

## How it integrates with DSH

A pure client-side patch (`src/client.js`, no build step) - it doesn't add any host-side behavior, just visual composer polish layered on top of DSH's existing model-select seat.

## Install

```sh
dsh plugin --profile web add @gz2016/dsh-plugin-model-icons
```

No configuration - it works out of the box for any provider already in your model catalog.

---
*Unofficial project, independently developed and maintained by a community member. Not affiliated with or endorsed by DeepSeek.*

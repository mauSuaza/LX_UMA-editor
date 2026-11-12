# LX_UMA editors

Web editors for the Plaits models in **LX_UMA**, an unofficial custom firmware for the Erica Synths LXR Eurorack
module. Make a wavetable or a wave terrain in the browser, hear it, and download a `.bin` file for the module's SD
card.

**Open the editors:** https://mausuaza.github.io/LX_UMA-editor/

| Page | Saves | Used by |
|---|---|---|
| Wavetable editor | a `.bin` (4,096 bytes: the 8 × 8 map, then 15 custom waves); imports Vital / Serum wavetables (15 frames, evenly spread) | the wavetable model (`wav`), as bank D, from the card's `WAVES/` |
| Wave terrain editor | a `.bin` (4,096 bytes: 64 × 64 signed bytes) | the wave terrain model (`ter`), as a 9th terrain, from the card's `TERRAIN/` |
| DX7 patch bank editor | a 32-voice DX7 `.syx` (name it with up to 8 letters or digits) | the 6-op (`dx7`), from the card's `DX7/` folder (LX_UMA 0.34 on) |

Where to put the files on the card is in the LX_UMA manual.

## Credits

These are Mutable Instruments' [Plaits editors](https://github.com/pichenettes/plaits-editor) by Emilie Gillet,
MIT licence, adapted for LX_UMA: the audio data transfer for a real Plaits (the `.wav` files played into its
TIMBRE input) is replaced by file downloads, and the wave terrain page gets a `.bin` download. The terrain file
holds the heights exactly as previewed. Changes are in the git history.

LX_UMA is a community project, not affiliated with or endorsed by Erica Synths or Mutable Instruments.

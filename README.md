# NoiseBow

*your rainbow of noise colours*

A single-file, in-browser noise generator. Build a **stack** of **layers**, each one a noise you shape yourself, and mix them.

## Per layer

- **Tilt** from -24 to +6 dB/oct: white (0), pink (-3), brown (-6), blue (+3), violet (+6), and steeper "black" slopes.
- **Low cut / high cut**: band-limit the noise (green is a band around 500 Hz).
- **Density**: from dense noise down to sparse crackle (black1, velvet).
- **Grey**: blends in an approximate equal-loudness curve.
- **Level** from 0 to 11. 10 is loudness-matched across colours; 11 is one louder.
- Built-in presets for all of the above, plus your own saved layer presets.

## Stacks

- Add layers with the big **+**; each layer has its own play/pause.
- **Save stack** keeps the whole mix. **Share** sends it (email, messages) as text; **Save JSON** and **Import** move stacks between devices.
- **Save audio** exports WAV or MP3: 5 whole loops (about 55 to 60 s) that repeat seamlessly. WAV is best for looping; MP3 adds a small gap at the loop point.

## Notes

- Everything runs in your browser. Saved presets and stacks live in that browser's local storage, per site address.
- MP3 export loads the [lamejs](https://github.com/zhuker/lamejs) encoder (LGPL) from a CDN the first time you use it.
- Keep the volume low. Deep presets carry a lot of bass and can stress small speakers.

## Hosting

It is one file: `index.html`. Put it on any static host, for example GitHub Pages (repo settings, Pages, deploy from `main`, root).

## Credits

Concept, direction and testing: whimsick-al.
Code: Claude (Anthropic), Sr. Dev. It started with the question "what colour is off-station radio static?"

## Install

Installable as an app: open the site in Chrome, then menu, **Install app**. It needs `manifest.webmanifest`, `sw.js` and the two icons next to `index.html`.

# Image Converter

Convert images to PNG, JPEG or WebP with resizing, quality controls, batch processing and shared history.

## Install

Requires a running [Ink OS](https://github.com/siliconjungle/ink-os-platform) instance and its `ink-os` CLI. Use Node.js 24 or later for development.

```sh
git clone https://github.com/siliconjungle/ink-app-image-converter.git
cd ink-app-image-converter
npm test
# Select your Ink instance using its CLI connection profile.
ink-os deploy .
```

The CLI deploys committed source from your checkout. Commit any edits before deploying them. No credentials or personal instance configuration belong in this repository.

## Behaviour and limits

Processing runs in the open browser window. Animated inputs produce a still image. Inputs/outputs are limited to 24 MiB and decoded images to 16 million pixels.

## Development

`npm run dev` opens a local development server. Preview fixtures are separate from live Ink data.

## License

MIT for app code. Bundled third-party components retain their own licenses and notices.

## Quick preview

Displays supported files without starting the normal editing workflow. Ink OS can select this reader through `desktop.preview.fileTypes`, independently of Open with. Space opens the temporary preview from a selection; Escape or Space dismisses it, and arrow keys browse the supplied item order.

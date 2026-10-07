# NOVA

NOVA is a futuristic AI companion that runs on GitHub Pages with no API key.

Live site: https://dhairya1611.github.io/nova-ai-companion/

## Free AI model

- WebLLM loads Llama 3.2 1B Instruct directly in the browser through WebGPU.
- The first model initialization downloads the model once; the browser caches it locally.
- If WebGPU is unavailable, NOVA uses a graceful offline reply mode instead of failing.
- Browser speech synthesis gives replies a voice without a paid speech API.

## Avatar behavior

The neural face is stored in assets/neural-face.svg. NOVA changes its expression label and animated face state while it is thinking or speaking: head motion, blinking, eye glow, scanline, and lip-sync animation are all handled in index.html.

## Hosting

This is a zero-build static GitHub Pages site. The complete UI, client-side model integration, animation logic, and avatar asset are present in this repository.

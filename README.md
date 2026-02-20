FRAKTAALI STUDIO

Real-time GPU-raymarched fractal explorer with sacred geometry, MIDI control, audio reactivity, and a full VJ performance system — in a single HTML file.

Features
Fractals — Mandelbulb, 4D Julia, Menger Sponge, Mandelbox, Sierpinski, Hybrid. Full 4D rotation, folding, symmetry, and Julia constant control.

Sacred Geometry — Torus, Flower of Life, Octahedron, Icosahedron, Sri Yantra, Metatron's Cube. Smooth-blended with fractal SDFs via domain repetition and animated rotation.

Color & Atmosphere — 7 blendable palettes (Rainbow → Fire → Ocean → Neon → Mono → Sacred Gold → Earth). Shader-level warmth, film grain, vignette, depth of field, colored fog, soft focus.

Canvas FX — Feedback trails with hue rotation, spatial delay, reverb blur, bloom, kaleidoscope. Layered via offscreen canvas compositing.

Performance System — 8 LFOs (sine/tri/saw/sq/S&H) with tempo sync and tap tempo. Full modulation matrix routing any source (LFO, audio band, MIDI CC) to any parameter. 8 performance macros.

MIDI — Plug and play. Left-click any parameter label to matrix-learn, right-click to direct CC bind. Note triggers for camera presets. Universal across all parameter systems.

Audio — Mic input or file playback with 8-band FFT, RMS/peak tracking, beat detection, and BPM auto-detection via onset autocorrelation.

Granular Randomization — 12 independent toggle groups (Shape, Dims, Folding, Julia, Color, Light, Geometry, Atmosphere, Camera, FX, LFOs, Matrix). Lock what you like, randomize everything else. Quick combos for Colors, Mood, Motion, Modulation.

Presets — 10 curated scenes, 8 atmosphere presets, 8 geometry presets, FX quick presets. Save/load/rename/export/import user presets as JSON. localStorage persistence.

Recording — WebM capture with configurable quality and FPS. Optional audio mux.

Tech Stack
Layer | Technology -- | -- Rendering | WebGPU (WGSL raymarching shader, 80-slot uniform buffer) FX compositing | Offscreen with 2D context feedback loop UI | Vanilla JS, event delegation, innerHTML panel swapping Audio | Web Audio API, AnalyserNode FFT, onset-based BPM detection MIDI | Web MIDI API with learn/bind system Recording | MediaRecorder + captureStream() State | Single mutable state object, no framework

Run
Open in Chrome or Edge (WebGPU required). That's it.

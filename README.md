# COSMOTION MVP

An inclusive space exploration game built with React, TypeScript, and Vite. The ASTRA mission supports camera hand tracking through MediaPipe Tasks Vision, plus mouse, touch, and keyboard controls. Profile choices, language, accessibility settings, and mission progress are stored only in the browser.

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed by Vite (normally `http://localhost:5173`). Camera access is available on localhost and HTTPS. The first camera session downloads the MediaPipe WASM and hand landmark model from their public CDNs. If camera permission, model download, or camera hardware is unavailable, choose mouse/touch or use the arrow keys.

To create and preview a production build:

```bash
npm run build
npm run preview
```

## Play

Start exploring, choose an astronaut name and avatar, open ASTRA, then select camera or pointer controls. Move onto stars to collect them. The pause/settings controls change the mission target count, target size, tracking sensitivity, one/two-hand detector setting, contrast, and sound. Arrow keys move the astronaut cursor. Seated play works with the same controls and there is no timer.

English, Kazakh, and Russian are available from the header. ASTRA is playable; ORBIT and NOVA are labeled as upcoming missions.

## Privacy

Camera frames are processed in the browser and are not recorded or uploaded by this app. Mission statistics and profile preferences stay in localStorage on the current browser. Clearing site storage resets local progress.

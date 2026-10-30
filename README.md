# Zombie Eaters — Aether Edition

Zombie Eaters is a cartoon pixel-art survival arcade game made with HTML, CSS, JavaScript, and Electron.

## Gameplay
Dodge the goofy pixel ghouls, dash out of crowded areas, collect glowing energy orbs, and survive as many waves as possible. The game uses non-graphic cartoon visuals.

## Controls
- **WASD / Arrow keys:** Move
- **Shift / Space:** Dash
- **Mobile touch controls:** Direction buttons and Dash

## Build the Windows game folder
1. Open the repository's **Actions** tab.
2. Select **Build Zombie Eaters for Aether (Windows)**.
3. Select **Run workflow**.
4. Wait for the build to finish.
5. Download the artifact named **Zombie-Eaters-Aether-Windows-Folder**.
6. Extract it. Keep the complete folder together; do not separate the EXE from its runtime files.

The folder contains the Windows executable, Electron runtime files, game assets, and `aether.manifest.json`. Upload the EXE and the complete extracted folder to the Aether Developer Portal. The manifest already contains the Aether public authentication key configured for this build.

The public key is an identifier for Aether authentication, not a password. Never put a Supabase service-role key or other backend secret in this game.

## Project files
- `index.html` — game screen and styling
- `game.js` — gameplay, enemies, collectibles, controls, and pixel rendering
- `electron/main.cjs` — Windows desktop wrapper
- `.github/workflows/build.yml` — automated Windows folder build
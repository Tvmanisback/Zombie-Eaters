# Zombie Eaters

A pixel-art, top-down arcade brawler made with HTML, CSS, and JavaScript.

## Play in a browser
Open `index.html` in a modern browser. The game is self-contained and does not need a server.

## Controls
- **WASD / Arrow keys:** Move
- **Space / J:** Close-range energy strike
- **Shift / K:** Quick dash

Survive waves of goofy pixel zombies. Keep moving, time your strikes, dash away from crowds, and build a high score. The art is intentionally cartoony and non-graphic.

## Windows build
Open the repository's **Actions** tab, select **Build Zombie Eaters for Windows**, and run the workflow. Download the artifact named **Zombie-Eaters-Windows-Game-Folder**.

Extract the artifact. It contains the Windows executable, Electron runtime files, game assets, and `aether.manifest.json`. Keep the entire folder together; do not move the EXE by itself.

Before submitting the folder to Aether, replace `ADD_YOUR_CURRENT_AETHER_PUBLIC_KEY_HERE` in `aether.manifest.json` with the public key currently shown in your Aether Developer Portal. The key is an identifier, not a password. Never put a Supabase secret or service-role key in the game.

## Project files
- `index.html` — game screen and styling
- `game.js` — gameplay, enemies, controls, and pixel rendering
- `electron/main.cjs` — Windows desktop wrapper
- `.github/workflows/build.yml` — automated Windows folder build
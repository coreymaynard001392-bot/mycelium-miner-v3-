# Mycelium Miner v0.3.0 (experimental)

Fabric Minecraft Java 1.21.11 client-side single-player prototype.

## Features
- O opens the multi-page HUB (Mycelium / Stone Generator / Settings / Help).
- F7 records a walking route and stores jump coordinates when Space is pressed.
- F6 toggles Mycelium mode; when the player reaches recorded jump positions, the macro tries to jump.
- Mine selected blocks. If no route points exist, the macro walks toward mining target coordinates.
- Eased turning with velocity/acceleration controls in Settings. Turning is still updated per client tick, so this is not true per-frame camera interpolation.
- Separate stone-generator macro for manually selected block positions, including concave layouts. Stand close enough to reach them.

## Build
Upload the CONTENTS of this ZIP to the root of a GitHub repository, including the hidden `.github` directory. Actions -> Build Mycelium Miner -> Run workflow. Download the artifact and install only `mycelium-miner-0.3.0.jar`, not the sources JAR.

## Limitations
Experimental and untested in a running Minecraft client. No pathfinding, collision avoidance, guaranteed block breaking or automatic navigation around obstacles. Routes and settings are not persisted between game restarts. The block selection and jump recorder require in-game testing. Test in a backup single-player world. Only one version of the mod should be installed at a time.

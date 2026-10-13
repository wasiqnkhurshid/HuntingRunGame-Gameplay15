# Hunting Run — Gameplay15 Arrow Lab

[Play the experiment](https://wasiqnkhurshid.github.io/HuntingRunGame-Gameplay15/). No installation or login required.

Choose **SHOOTING LAB**, compare **A Minimal / B Balanced / C Strong**, then **START / RESTART TEST**. Choose the correct lane and tap Shoot as animals approach. Arrows travel physically at high speed with a shallow arc. Assistance predicts a same-lane animal at release and applies a bounded correction; arrows never home. Actual swept collision decides hits, including blocking obstacles. Wrong-lane, out-of-range, overlapping/behind and outside-cone shots remain invalid. Difficult valid shots can still miss.

Defaults: Balanced, 125 m/s, gravity 0.8 m/s², assistance 75%, base range 40 m, Accuracy 50 and Range 40. Minimal: 140 m/s, 0.6 gravity, 35% strength, 5° base cone, 0.09 m arrow radius. Balanced: 10° base cone, 0.14 m radius. Strong: 115 m/s, 1.0 gravity, 100% strength, 15° base cone, 0.18 m radius. Accuracy scales the cone; Range extends engagement and velocity without increasing accuracy. Configuration adjusts speed, gravity, strength, base range, bow stats, seed and straight/curved road. Optional diagnostics are OFF by default. No timing meter, crosshair game, charging, target-lock interaction or manual aiming.

Swipe anywhere, including on/across Shoot, to move/jump/duck. One tap fires once on release; holding never repeats; independent fingers can move and shoot. Keyboard: A/D or arrows, W/Space, S, Enter, Escape. Mouse click Shoot is supported. Enter fires once even after mouse selection. The normal run HUD is unchanged. **Pause → SHOOTING LAB → START / RESTART TEST** repeats the seed with 99 arrows and full health. RESET LAB restores defaults. Each test has zero cooldown and normal 90-second / 2,880 m gameplay at 32 m/s with Closer camera, natural animals, obstacles and pickups. Shoot remains 84 dp; swipes remain 18 dp.

Source `ed724b12abe48d939261cd7fb4eafb080a7ed77f`, branch `codex/gameplay15-redesigned-shooting`; compiled WebGL only. Gameplay12, Gameplay13 and Gameplay14 remain unchanged. Gameplay15 has separate IndexedDB `HuntingRun.Gameplay15:/idbfs`, save key and native filename. Experimental rewards/resume snapshots are not committed.

Unity and desktop Chrome touch/keyboard simulation passed. Physical Android/iPhone, Safari, thumb feel, human shooting difficulty and sustained mobile performance remain untested. WebGL2 and WebAssembly required. Loading/storage depend on browser and device. Fixture hit percentages are engineering comparisons, not predicted player hit rates.

## Rollback

Unpublish only this repository's Pages site to withdraw Gameplay15. After future changes, restore tag `gameplay15-redesigned-shooting` into a new main commit and push; do not force-push. Earlier sites remain available independently: [Gameplay12](https://wasiqnkhurshid.github.io/HuntingRunGame-WebGL/), [Gameplay13](https://wasiqnkhurshid.github.io/HuntingRunGame-Gameplay13/), [Gameplay14](https://wasiqnkhurshid.github.io/HuntingRunGame-Gameplay14/).

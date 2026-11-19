# shipdesign-starship

Model Series 02 concept starship, rebuilt from scratch in Blender from the reference pack (interior orthographic master + six-view cutaway sheet).
96 m hull (117.6 m overall incl. the swept tail blades), 2 decks (Z 0 / +3.6 m), 12 crew; organic purple hull with copper rib lattice, cyan glows.
Full modelled interior laid out to the master: sensor nose, bridge / avionics, 6 crew cabins (C1–C6), mess / med / galley / life-WC,
lift + stairs, kitchen / stowage, cargo with hatch pairs at X 52, control / airlock, Ø 6 m core at X 69 Z +2, three drives (Y −3.2 / 0 / +3.2).

- **Current version:** v36 (previous: v35 GLB kept at `models/model_v35_web.glb`)
- **Live preview:** https://xuzhiming.github.io/shipdesign-starship/  (cutaway buttons: side Y / top Z / section X + slider, deck toggles; `?cut=side` opens cut, `?light=dark` dark look)
- **Web GLB (embeddable):** https://xuzhiming.github.io/shipdesign-starship/models/model_v36_web.glb
- **Hero render:** https://xuzhiming.github.io/shipdesign-starship/renders/v36_01_hero.png
- **Cutaway render:** https://xuzhiming.github.io/shipdesign-starship/renders/v36_02_cutaway.png  ·  top cut: https://xuzhiming.github.io/shipdesign-starship/renders/v36_03_cutaway_top.png
- **Six-view comparison:** https://xuzhiming.github.io/shipdesign-starship/renders/v36_compare_6view.png

GLB node names: `<GROUP>__<MATERIAL>[__NC]` with GROUP = EXT (hull/fins), INT_S (shared structure), INT_U (upper deck), INT_L (lower deck), CORE, DRV; `__NC` = not clipped by the cutaway.

Pipeline: Blender bpy → GLB → gltf-transform (dedup + meshopt) → Three.js r170 viewer.

# shipdesign-starship

Model Series 02 concept starship, rebuilt from scratch in Blender from the reference pack (interior orthographic master + six-view cutaway sheet).
96 m hull (117.6 m overall incl. the swept tail blades), 2 tall decks (lower floor Z −4.2, upper floor Z +1.6, 5.8 m pitch / ~5.5 m clear, measured from the LEFT/RIGHT/FRONT cutaways), 12 crew; organic purple hull with copper rib lattice, cyan glows; swept side tail blades are open crescent skeletons: smooth spline ribs + struts with filleted joints, gold knuckles and gold-clad points; built on one side and mirrored exactly across Y=0. Dorsal / central / keel blade tips carry heavier gold trim. v39: dorsal fin and keel are spline-outlined lens solids faired into the hull, the central tail spike is one lofted streamlined body with a sharp point, side-blade ribs are merged into continuous spline sweeps, and all thorns are tapered curved horns; every paired exterior part is an exact Y=0 mirror. v40: the dorsal fin and the central tail spike are one continuous lens mesh (fin flows into the spike, one unbroken gold rim to the point, spike openings as flush dark recesses); the hull is refit from fair C2 cubic B-spline stations (flutes / ring bulges removed, smooth zebra) with the copper lattice, glows and canopy re-seated on it; underneath only the keel fin and the largest ventral fin pair remain (all small ventral thorns removed).
Full modelled interior laid out to the master: sensor nose, bridge / avionics, 6 crew cabins (C1–C6), mess / med / galley / life-WC,
lift + stairs, kitchen / stowage, cargo with hatch pairs at X 52, control / airlock, Ø 6 m core at X 69 Z +2, three drives (Y −3.2 / 0 / +3.2).

- **Current version:** v40 (previous GLBs kept: `models/model_v39_web.glb`, `models/model_v38_web.glb`, `models/model_v37_web.glb`, `models/model_v36_web.glb`, `models/model_v35_web.glb`)
- **Live preview:** https://xuzhiming.github.io/shipdesign-starship/  (cutaway buttons: side Y / top Z / section X + slider, deck toggles; `?cut=side` opens cut, `?light=dark` dark look)
- **Web GLB (embeddable):** https://xuzhiming.github.io/shipdesign-starship/models/model_v40_web.glb
- **Hero render:** https://xuzhiming.github.io/shipdesign-starship/renders/v40_01_hero.png
- **Cutaway render:** https://xuzhiming.github.io/shipdesign-starship/renders/v40_02_cutaway.png  ·  top cut: https://xuzhiming.github.io/shipdesign-starship/renders/v40_03_cutaway_top.png
- **Six-view comparison:** https://xuzhiming.github.io/shipdesign-starship/renders/v40_compare_6view.png
- **v39 → v40 before/after (fin–spike junction close-up + zebra, hull zebra, underside view):** https://xuzhiming.github.io/shipdesign-starship/renders/v40_before_after.png
- v38 → v39 before/after: https://xuzhiming.github.io/shipdesign-starship/renders/v39_before_after.png

GLB node names: `<GROUP>__<MATERIAL>[__NC]` with GROUP = EXT (hull/fins), INT_S (shared structure), INT_U (upper deck), INT_L (lower deck), CORE, DRV; `__NC` = not clipped by the cutaway.

Pipeline: Blender bpy → GLB → gltf-transform (dedup + meshopt) → Three.js r170 viewer.

# 3D Figure Animation Test

Testrepo for å animere 3D-figurer i nettleseren med **Three.js**.

## Hva er her

- `index.html` – interaktiv viewer med OrbitControls
- Offentlig demo-modell: [Soldier.glb](https://threejs.org/examples/models/gltf/Soldier.glb) med flere animasjoner (idle, walk, run osv.)
- `boy_fbx.b64.txt` – base64 av `Boy.fbx` fra det private repoet `night-mansion` (assets/models/figures_v2/Boy.fbx)

## Se det live

1. Gå til **Settings → Pages** i dette repoet
2. Source: Deploy from a branch → `main` / `/ (root)`
3. Etter noen minutter: `https://olebee.github.io/3d-figure-anim-test/`

Eller bare åpne `index.html` lokalt (men da trenger du en lokal server pga. CORS/modules).

## Bruke din egen modell (Boy.fbx)

I `index.html` kan du bytte til FBXLoader og laste den innebygde base64-filen. 

FBX fra night-mansion er ofte i cm-skala, så `model.scale.setScalar(0.01)` er vanlig.

Det finnes også separate animasjonsfiler (`Anim_Run.fbx`, `Anim_Fall.fbx` osv.) i `assets/models/figures_v2/` som kan lastes og spilles av med `AnimationMixer`.

## Tips

- For produksjon: eksporter til **GLB** fra Blender (bedre støtte, mindre fil, innebygde animasjoner).
- Three.js FBXLoader fungerer, men GLTF/GLB er anbefalt.

Laget som test for OleBee.

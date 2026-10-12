# 3D Figure Animation Test

Testrepo for å animere 3D-figurer i nettleseren med **Three.js**.

## Hva er her

- `index.html` – interaktiv viewer som laster **Boy.fbx** fra night-mansion og animerer den (idle bob + rotasjon)
- `boy_fbx.b64.txt` – base64 av Boy.fbx (assets/models/figures_v2/Boy.fbx)

## Se det live

1. Gå til **Settings → Pages** i dette repoet
2. Source: Deploy from a branch → `main` / `/ (root)`
3. Etter noen minutter: `https://olebee.github.io/3d-figure-anim-test/`

## Hvis modellen ikke laster

`boy_fbx.b64.txt` må inneholde den faktiske base64-strengen. Du kan generere den lokalt:

```bash
base64 -w 0 Boy.fbx > boy_fbx.b64.txt
```

og committe filen.

FBX er ofte i cm, derfor `scale.setScalar(0.01)`.

Det finnes også egne animasjonsfiler (Anim_Run.fbx etc.) i night-mansion som kan lastes med AnimationMixer.

## Tips

- GLB er bedre for web enn FBX.
- Laget som test for OleBee.

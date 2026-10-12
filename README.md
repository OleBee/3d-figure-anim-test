# 3D Figure Animation Test

Testrepo for å animere 3D-figurer i nettleseren med **Three.js**.

## Status

**Klar.** `boy_fbx.b64.txt` inneholder nå den ekte Boy.fbx fra night-mansion, og `index.html` laster den direkte.

## Se det live

1. Gå til **Settings → Pages**
2. Source: Deploy from a branch → `main` / `/ (root)`
3. URL: `https://olebee.github.io/3d-figure-anim-test/`

## Hva som skjer

- Laster Boy.fbx (skala 0.01 fordi FBX ofte er i cm)
- Enkel idle-animasjon (bob + mild rotasjon)
- OrbitControls for å se rundt
- Fallback til Soldier-modell hvis noe går galt

## Animasjoner

Det finnes egne animasjonsfiler (`Anim_Run.fbx`, `Anim_Fall.fbx` osv.) i `night-mansion` som kan lastes med `AnimationMixer`.

Laget som test for OleBee.

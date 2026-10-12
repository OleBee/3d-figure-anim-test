# 3D Figure Animation Test

Testrepo for å animere 3D-figurer i nettleseren med **Three.js**.

## Status

Viewer-en er klar. Den prøver å laste **Boy.fbx** fra `boy_fbx.b64.txt`. Hvis filen er placeholder eller mangler, faller den automatisk tilbake til en offentlig Soldier-modell med ekte animasjoner.

## Få din egen Boy.fbx inn

Last ned den ferdige base64-filen (se chat) og erstatt `boy_fbx.b64.txt` i repoet:

```bash
# Etter at du har lastet ned boy_fbx.b64.txt
git add boy_fbx.b64.txt
git commit -m "Add real Boy.fbx base64"
git push
```

Etter push vil siden bruke din modell.

## Se det live

1. Gå til **Settings → Pages**
2. Source: Deploy from a branch → `main` / `/ (root)`
3. URL: `https://olebee.github.io/3d-figure-anim-test/`

## Animasjoner

Det finnes egne animasjonsfiler (`Anim_Run.fbx`, `Anim_Fall.fbx` osv.) i `night-mansion`. De kan lastes med `AnimationMixer` når base64-en er på plass.

Laget som test for OleBee.

/opt/homebrew/Library/Homebrew/cmd/shellenv.sh: line 18: /bin/ps: Operation not permitted
# Transposeur de tonalité

Application audio autonome pour Mac et iPad, réalisée pour **Steeve Langevin — Folk Guitare & Ukulélé**.

Elle permet notamment de :

- transposer une chanson sans modifier sa durée ni son tempo;
- estimer la tonalité originale et le BPM;
- écouter l’original et le résultat;
- régler indépendamment la vitesse de lecture;
- enregistrer la chanson transposée en WAV.

## Utilisation immédiate

Télécharger `transposeur.html`, puis l’ouvrir dans un navigateur moderne. Le traitement audio s’effectue localement dans le navigateur : la chanson n’est pas envoyée sur un serveur.

Sur iPad, la version hébergée dans Safari demeure généralement plus fiable qu’un fichier HTML ouvert depuis l’application Fichiers, car iPadOS peut limiter certaines fonctions audio des fichiers locaux.

## Développement

Le projet utilise React, Vinext et SoundTouchJS. Le fichier HTML autonome est produit à partir de `standalone-entry.tsx` et `standalone-shell.html`.

```bash
npm install
npm run build
```

## Avertissement

La tonalité et le BPM détectés sont des estimations et peuvent nécessiter une correction manuelle, particulièrement pour les chansons à tempo variable, en mesure ternaire ou dont la tonalité change.

Copyright © 2026 Steeve Langevin. Aucun droit de réutilisation n’est accordé sans autorisation explicite.

# Fichiers du dépôt `siquane.github.io`

Ces fichiers ne servent pas au jeu lui-même. Ils vont dans un **autre dépôt GitHub**, nommé exactement `siquane.github.io`, qui publie la racine de l'adresse `https://siquane.github.io/`.

| Fichier | Rôle |
| --- | --- |
| `404.html` | Renvoie vers le jeu les adresses mal écrites, par exemple `…/neko-odyssey/` en minuscules (GitHub tient compte des majuscules). Pour toute autre adresse inconnue, affiche un bouton « Jouer à Neko Odyssey ». |
| `index.html` | `https://siquane.github.io/` tout court ouvre le jeu. |
| `.nojekyll` | Fichier vide : il permettra de publier le dossier `.well-known` (fichier `assetlinks.json` pour le Play Store, plus tard). |

## Mise en place

1. Sur GitHub : **New repository**, nom exact `siquane.github.io`, **Public**, puis **Create repository**.
2. **Add file › Upload files** : envoyer `404.html`, `index.html` et `.nojekyll`, puis **Commit changes**.
3. **Settings › Pages** : **Deploy from a branch**, branche `main`, dossier `/ (root)`, **Save**.
4. Après une minute, tester `https://siquane.github.io/neko-odyssey/` : on doit arriver sur le jeu.

Pour le Play Store, on ajoutera plus tard dans ce même dépôt le fichier `.well-known/assetlinks.json` (voir `store/PLAY-STORE.md`).

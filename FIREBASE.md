# Activer le classement en ligne

Le classement entre amis utilise **Firebase**, un service gratuit de Google. Les joueurs n'ont pas besoin de compte : chacun choisit seulement un pseudo. Il te faut un compte Google pour créer le projet, une seule fois (environ 10 minutes).

Le classement marche sur la version du jeu publiée sur **GitHub Pages**. Il ne marche pas dans la version Claude, qui ne peut contacter aucun serveur extérieur.

## 1. Créer le projet Firebase

1. Va sur <https://console.firebase.google.com> et connecte-toi avec ton compte Google.
2. Clique sur **Créer un projet**. Donne-lui un nom, par exemple `siquane-escape-cat`. Tu peux désactiver Google Analytics, il ne sert pas.
3. Dans le projet, clique sur l'icône **Web** (`</>`) pour ajouter une application web. Donne-lui un nom et ne coche pas Firebase Hosting.
4. Firebase affiche un bloc `firebaseConfig`. Garde de côté deux valeurs : `apiKey` et `projectId`.

## 2. Activer la connexion anonyme

1. Dans le menu de gauche, ouvre **Créer › Authentication**, puis clique sur **Commencer**.
2. Onglet **Mode de connexion** : choisis **Anonyme**, active-le, puis enregistre.

Les joueurs reçoivent ainsi un identifiant invisible, gardé dans leur navigateur. Il empêche qu'un autre joueur modifie leurs scores ou prenne leur pseudo.

## 3. Créer la base de données

1. Ouvre **Créer › Firestore Database**, puis clique sur **Créer une base de données**.
2. Choisis un emplacement en Europe (par exemple `europe-west1`), puis le **mode production**.
3. Onglet **Règles** : remplace tout le texte par le contenu du fichier [`firestore.rules`](firestore.rules) de ce dépôt, puis clique sur **Publier**.

## 4. Brancher le jeu

Dans `index.html`, tout en haut du script, remplis la ligne :

```js
const FIREBASE = { apiKey: 'ta-clé', projectId: 'ton-projet' };
```

Tu peux aussi me donner ces deux valeurs et je fais la modification. La clé `apiKey` n'est pas un secret : elle identifie seulement le projet. Ce sont les règles de l'étape 3 qui protègent les données.

## 5. Publier le jeu sur GitHub Pages

1. Sur GitHub, ouvre le dépôt, puis **Settings › Pages**.
2. Dans **Source**, choisis **Deploy from a branch**. Prends la branche `main` (ou la branche du jeu tant que la pull request n'est pas fusionnée) et le dossier `/ (root)`, puis enregistre.
3. Après une minute, GitHub affiche le lien du jeu, du type `https://<compte>.github.io/Siquane-Escape-Cat/`. Partage ce lien avec tes amis.

## Bon à savoir

- Le plan gratuit de Firebase (Spark) suffit largement pour un groupe d'amis : 50 000 lectures et 20 000 écritures par jour.
- Un pseudo fait 3 à 16 caractères (lettres, chiffres, espaces, `-` et `_`) et ne peut appartenir qu'à un seul joueur. On peut le changer depuis l'écran du classement.
- Pour retirer un joueur, supprime son document dans `players` (et son pseudo dans `pseudos`) depuis la console Firestore.
- Les scores sont envoyés par le jeu lui-même : un joueur très motivé qui sait programmer pourrait tricher. Les règles limitent seulement les valeurs possibles.

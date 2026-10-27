# Plan des achats · Neko Odyssey

Brouillon pour une future mise à jour. Rien n'est encore dans le jeu.

## Les règles qu'on se fixe

Le jeu vise aussi les enfants. Les achats doivent donc être **honnêtes, optionnels et sans pression** :

1. **On ne vend que du décoratif.** Rien qui aide à gagner, à aller plus loin ou à répondre aux questions. Un joueur qui ne paie jamais a exactement le même jeu.
2. **On ne vend pas la monnaie du jeu.** Pas de croquettes, pas de poissons d'or, pas de seconde chance, pas de pouvoirs, pas d'expérience. Vendre de la monnaie pousse à « recharger » et c'est mal vu par Google pour les jeux pour enfants.
3. **Pas de pression.** Pas de compte à rebours, pas de « offre spéciale qui disparaît », pas de fenêtre qui s'ouvre toute seule, pas de message pendant la course.
4. **Toujours clair.** Le prix en euros est écrit sur le bouton, et un écran de confirmation précise « Demande à un parent avant d'acheter ».
5. **Tout ce qui existe aujourd'hui reste gratuit** et se gagne en jouant.

## Le catalogue proposé

| Achat | Contenu | Prix | Tu touches (après les 15 % de Google) |
| --- | --- | --- | --- |
| **Pack Ami de Neko** (soutien) | 1 chat exclusif « Mécène » (pelage doré à étoiles, aura dorée) + chapeau « Cœur d'or » + remerciement dans l'histoire | 1,99 € | ≈ 1,40 € |
| **Pack Chats du monde** | 3 chats exclusifs : Maine Coon, Sphynx, Scottish Fold | 2,49 € | ≈ 1,75 € |
| **Pack Chats de l'espace** | 3 chats exclusifs : Astro (combinaison), Robot (métallique, yeux lumineux), Galaxie (pelage étoilé animé) | 2,49 € | ≈ 1,75 € |
| **Pack Chapeaux de luxe** | 5 chapeaux exclusifs : couronne de diamants, casque d'astronaute, chapeau de magicien qui scintille, tiare de fleurs lumineuses, casquette néon | 0,99 € | ≈ 0,70 € |
| **Pass Toutes les fêtes** | Rend achetables toute l'année les chapeaux et déguisements de fête (au prix habituel en croquettes et poissons d'or) | 1,99 € | ≈ 1,40 € |
| **Décor Neige éternelle** | Le décor enneigé de Noël, à choisir quand on veut | 0,99 € | ≈ 0,70 € |

Les montants nets sont approximatifs : Google encaisse le prix TTC, reverse la TVA à l'État pour toi, puis garde 15 % du reste. En France (TVA 20 %), 1,99 € donne environ 1,40 € sur ton compte.

**Pourquoi ces prix ?** Entre 0,99 € et 2,49 €, ce sont des montants qu'un parent accepte facilement, et chaque pack se suffit à lui-même. Pas d'abonnement, pas de « pack à 19,99 € ».

## Ce qui reste gratuit, pour toujours

Les 22 chats (dont les 5 chats spéciaux de l'histoire) et les 30 chapeaux actuels, les déguisements de fête pendant leur fête, le voyage complet (35 villes, 280 rues, la carte, les 35 chapitres de l'histoire), les quelque 850 questions, les missions, le cadeau du jour, le classement, les poissons d'or trouvés en jouant.

## Dans le jeu

- Un 4e onglet **« Spécial »** dans la boutique, à côté de Chats, Chapeaux et Poissons d'or, dans la barre d'onglets qui reste en haut de l'écran. On n'y voit que les packs, avec un aperçu animé et le prix en euros.
- Le bouton d'achat ouvre la fenêtre de paiement Google Play. Sur un compte Google enfant (Family Link), c'est le parent qui valide.
- Les objets achetés vont dans l'album avec la mention « Exclusif ».
- Un bouton **« Restaurer mes achats »** pour les retrouver après un changement de téléphone.
- Les achats ne marchent que dans l'appli du Play Store. Sur le site web, l'onglet « Spécial » indique « Disponible dans l'appli Android ».

## Ce qu'il faudra mettre en place

| Quoi | Pourquoi | Coût |
| --- | --- | --- |
| Profil de paiement Google Play | Recevoir l'argent | Gratuit |
| Micro-entreprise : modification au Guichet unique (adresse de domiciliation, nom commercial Siquane Lab, activité d'édition de jeux 58.21Z) | La micro-entreprise existe déjà : il faut qu'elle couvre l'édition de jeux et ne montre pas ton adresse personnelle | Gratuit |
| Dépôt de la marque « Neko Odyssey » à l'INPI | Protéger le nom avant de vendre (nom vérifié libre le 27 octobre 2026) | 190 €, + 40 € pour une 2e classe |
| Produits dans la Play Console | Déclarer chaque pack et son prix | Gratuit |
| Achats Google Play dans le jeu (interface « Digital Goods ») | Ouvrir la fenêtre de paiement Google | Développement |
| Petit serveur de vérification (Firebase Functions) | Vérifier chaque achat auprès de Google, sinon on pourrait tricher | Forfait Firebase Blaze, quasi gratuit à petite échelle |
| Mise à jour de la politique de confidentialité et du formulaire « Sécurité des données » | Déclarer les achats | Gratuit |
| Dessin des nouveaux chats et chapeaux | Le contenu vendu | Développement |

## Ordre conseillé

1. **Publier le jeu gratuit** sur le Play Store et réunir des joueurs.
2. **Observer** quels chats et chapeaux plaisent le plus (dans le classement Collection, par exemple).
3. **Déposer la marque** « Neko Odyssey » à l'INPI avant de vendre quoi que ce soit.
4. **Commencer petit** : seulement le Pack Ami de Neko et le Pack Chapeaux de luxe.
5. **Ajouter les autres packs** si les premiers marchent.

# Siquane Escape Cat

Un petit jeu de course (*runner*) où tu incarnes un chat qui court la nuit sur les toits de la ville.

## Comment jouer

Ouvre `index.html` dans un navigateur (sur ordinateur ou sur téléphone). Il n'y a rien à installer.

| Action | Clavier | Tactile |
| --- | --- | --- |
| Changer de couloir | `←` `→` ou `Q` `D` (`A` `D` en QWERTY) | Swipe gauche / droite |
| Sauter | `↑`, `Z` (`W` en QWERTY) ou `Espace` | Swipe vers le haut |
| Roulade | `↓` ou `S` | Swipe vers le bas |
| Pause | `Échap` ou `P` | Bouton pause |

Pendant un saut, la roulade fait retomber le chat plus vite et il roule dès qu'il touche le toit.

## Sur les toits

- **Croquettes en forme de poisson** : attrape-les, chacune rapporte 10 points.
- **Flaque d'eau** : si le chat marche dedans, la partie est perdue. Saute par-dessus ou change de couloir.
- **Antenne basse** : saute par-dessus.
- **Grande antenne** : passe dessous en roulade.
- **Cheminée** : trop haute pour sauter, il faut changer de couloir.

La vitesse augmente au fil de la partie et les obstacles deviennent plus nombreux. Le score compte la distance parcourue et les croquettes. Le meilleur score est enregistré dans le navigateur.

## Interface

- **Accueil** : le bouton **Jouer** reste toujours visible en bas de l'écran. Les missions, le défi du jour, la bannière de fête et « Comment jouer » se déplient d'un geste. Boutique, Album, Histoire et Classe sont des tuiles avec icône. Les boutons de musique et de bruitages sont en haut à droite.
- **Fin de partie** : le score et le bouton **Rejouer** d'abord, puis l'expérience, le prochain chat à débloquer et les missions.
- **Système de design** : toutes les couleurs, tailles de texte (7), arrondis (4) et espacements viennent de variables CSS. Les textes font au moins 13 px et chaque bouton au moins 44 px de haut.

## L'histoire

Une nuit d'orage, un petit chat s'abrite dans un camion de livraison et se réveille au cœur d'une ville inconnue, loin de sa famille. Pour rentrer, il court de toit en toit. Au premier lancement, le joueur donne un nom à son chat (« Siquane » par défaut). Il peut le changer ensuite dans l'écran **Histoire**.

L'histoire compte 10 chapitres, qui se débloquent avec le **niveau du joueur** : Gaston le pigeon, Filou le chat errant, le ruban rouge, Plume la petite sœur… jusqu'au retour à la maison.

## Niveau du joueur

Chaque partie donne de l'expérience (XP) selon la distance parcourue, les croquettes, les bonnes réponses et les missions réussies. Chaque nouveau niveau rapporte des croquettes et peut débloquer un chapitre de l'histoire.

## Écran de fin de partie

- L'expérience gagnée et la barre du niveau du joueur.
- « Encore 48 croquettes avant le chat Gris » : ce qu'il manque pour débloquer le prochain chat (puis le prochain chapeau).
- Le record avec le chat utilisé : chaque chat a son propre record.
- **Partager mon score** : une image avec le chat, son chapeau, son nom et le score, à enregistrer ou à partager.

## Album

L'album montre tous les chats et tous les chapeaux, avec des silhouettes pour ceux qui manquent, un compteur (par exemple « 5/12 chats · 7/25 chapeaux ») et le record de chaque chat. Les chapeaux en édition limitée indiquent pendant quelle fête ils sont en vente.

## Surprises sur les toits

- **Étoile filante dorée** : de temps en temps, elle traverse le ciel puis tombe sur le toit, devant le chat. Il faut sauter pour l'attraper : +25 croquettes et 250 points.
- **Pigeons** : ils se posent sur le rebord du toit et s'envolent au passage du chat.
- **Filou, le chat errant** : il court quelques secondes à côté du chat sur le rebord, puis repart en le saluant (+30 points).

## Quartiers et questions de culture générale

La ville est découpée en quartiers. À chaque nouveau quartier, la course fait une pause et propose jusqu'à 3 questions de culture générale (sciences et nature, histoire et géographie, français et maths, arts et culture). Chaque bonne réponse rapporte 1 croquette. En cas d'erreur, le jeu donne la bonne réponse et une explication. Ensuite, un compte à rebours 3-2-1 relance la course.

Au premier lancement, le joueur choisit sa classe (du CP à la 3e, ou « Lycée et + »). Elle se change avec la tuile **Classe** de l'écran d'accueil. Le jeu ajuste ensuite un peu la difficulté : après 3 bonnes réponses d'affilée, les questions deviennent plus difficiles, et après 2 erreurs d'affilée, plus faciles. Les calculs sont générés automatiquement et changent à chaque fois.

## Missions, défi du jour et cadeau du jour

- **3 missions** à la fois (par exemple « Saute 5 antennes basses » ou « Donne 3 bonnes réponses »). Chaque mission réussie rapporte de 25 à 60 croquettes et est remplacée par une nouvelle, un peu plus difficile au fil du temps.
- **Défi du jour** : un objectif plus difficile qui change chaque jour, pour 100 croquettes.
- **Cadeau du jour** : des croquettes offertes une fois par jour, de plus en plus nombreuses au fil des jours de jeu (de 25 à 70). On ne perd pas sa progression si on rate un jour.

## Bonus et sensations

- **Bonus** à attraper sur les toits : l'aimant attire les croquettes, le parapluie protège des flaques, les croquettes x2 comptent double, et le super-saut permet de passer au-dessus des cheminées.
- **Combos** : ramasser des croquettes d'affilée fait monter un multiplicateur de points (jusqu'à x5).
- **« Ouf ! »** : éviter un obstacle de justesse déclenche un petit ralenti et rapporte 20 points.
- L'écran tremble quand le chat se cogne, un message s'affiche quand on bat son record, et la fin de partie indique combien de points il manquait pour le battre.

## Musique

Une musique chiptune originale accompagne le jeu. Elle est générée dans le navigateur, sans fichier audio.

- Dans les menus et pendant les questions, une version calme et plus lente.
- Pendant la course, la version complète avec batterie, dont le tempo accélère avec le chat (environ 130 → 160 BPM).
- Pendant un bonus, des arpèges plus aigus et un rythme plus serré. Après un nouveau record, la musique monte d'un ton jusqu'à la fin de la partie.
- Chaque fête a sa variante : clochettes à Noël, orgue en mineur à Halloween, gamme pentatonique et wood-block au Nouvel An chinois, steel drum en été, etc.
- La musique et les bruitages se coupent séparément, avec les boutons en haut à droite pendant la course, ou sur l'écran d'accueil et l'écran de pause. Ces réglages sont enregistrés.

## Les chats à débloquer

Les croquettes ramassées pendant les parties vont dans une tirelire. Dans la **Boutique**, tu peux les dépenser pour débloquer de nouveaux chats, puis choisir celui avec lequel tu cours. La tirelire et les chats débloqués sont enregistrés dans le navigateur.

| Chat | Prix |
| --- | --- |
| Roux | offert |
| Gris | 50 |
| Noir | 80 |
| Blanc | 120 |
| Tigré brun | 160 |
| Tuxedo | 250 |
| Siamois | 350 |
| Calico | 450 |
| Rose | 550 |
| Bleu nuit (avec des étoiles) | 650 |
| Doré (qui brille) | 800 |
| Arc-en-ciel (qui change de couleur) | 1000 |

## Les chapeaux

Dans l'onglet **Chapeaux** de la boutique, les croquettes servent aussi à acheter des chapeaux. Chaque chapeau va sur n'importe quel chat.

| Chapeau | Prix |
| --- | --- |
| Bonnet à pompon | 30 |
| Bob de pêcheur (avec un petit poisson qui pend) | 60 |
| Toque de chef | 90 |
| Pastèque | 120 |
| Béret baguette | 150 |
| Cow-boy | 200 |
| Haut-de-forme | 260 |
| Couronne | 320 |
| Bonnet de nuit étoilé | 380 |
| Mini-antenne (avec une lumière qui clignote) | 420 |
| Casque de ramoneur (avec une lampe qui éclaire devant) | 480 |
| Sorcière | 560 |
| Viking | 650 |
| Corne de licorne | 750 |
| Auréole | 900 |

## Les thèmes de fête

Le jeu change tout seul de décor pendant les fêtes, selon la date de l'appareil. Pendant un thème, le ciel, les toits, les obstacles et les objets à ramasser changent d'apparence (les règles restent les mêmes), et un chapeau en **édition limitée** est en vente dans la boutique à 150 croquettes. Une fois acheté, il reste à toi toute l'année.

| Thème | Dates | Objets à ramasser | Les flaques deviennent | Chapeau limité |
| --- | --- | --- | --- | --- |
| Nouvel An | 29 décembre → 3 janvier | étoiles dorées | champagne renversé | Chapeau de fête |
| Saint-Valentin | 10 → 15 février | chocolats en cœur | sirop de fraise | Serre-tête à cœurs |
| Nouvel An chinois | la veille → 7 jours après (date qui change chaque année) | enveloppes rouges | eau | Coiffe de dragon |
| Poisson d'avril | 31 mars → 2 avril | poissons en papier | eau | Poisson d'avril |
| Pâques | 6 jours avant → lundi de Pâques | œufs en chocolat | chocolat fondu | Oreilles de lapin |
| Fête de la musique | 19 → 22 juin | notes de musique | eau | Casque audio |
| Été et 14 Juillet | 1er juillet → 31 août | glaces | eau de piscine | Chapeau de paille |
| Journée internationale du chat | 7 → 9 août | pelotes de laine | lait renversé | Oreilles de souris |
| Halloween | 20 octobre → 2 novembre | bonbons | potion | Citrouille |
| Noël | 1er → 28 décembre | cadeaux | neige fondue | Bonnet de Père Noël |

Pour voir un thème en dehors de ses dates (par exemple pour tester), ajoute `#theme-noel` à la fin de l'adresse du jeu (ou `#theme-halloween`, `#theme-paques`, etc., et `#theme-aucun` pour le décor normal).

Tout le jeu tient dans un seul fichier, `index.html` (HTML, CSS et JavaScript, dessin sur `<canvas>`, sons générés avec la Web Audio API).

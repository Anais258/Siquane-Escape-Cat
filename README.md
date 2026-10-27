# Neko Odyssey

Un petit jeu de course (*runner*) où tu incarnes un chat qui court la nuit sur les toits, à travers toute la France, de Marseille à Besançon, pour retrouver sa famille.

Jeu en ligne : <https://siquane.github.io/Neko-Odyssey/>

## Comment jouer

Ouvre `index.html` dans un navigateur (sur ordinateur ou sur téléphone).

**Installer le jeu comme une application** : sur la version publiée sur GitHub Pages, ouvre le menu du navigateur et choisis **Installer** (Chrome, Edge) ou **Partager › Sur l'écran d'accueil** (Safari sur iPhone). Le jeu s'ouvre alors en plein écran avec son icône, et marche aussi sans connexion (sauf le classement).

| Action | Clavier | Tactile |
| --- | --- | --- |
| Changer de couloir | `←` `→` ou `Q` `D` (`A` `D` en QWERTY) | Swipe gauche / droite |
| Sauter | `↑`, `Z` (`W` en QWERTY) ou `Espace` | Swipe vers le haut |
| Roulade | `↓` ou `S` | Swipe vers le bas |
| Pause | `Échap` ou `P` | Bouton pause |

Pendant un saut, la roulade fait retomber le chat plus vite et il roule dès qu'il touche le toit. Après une pause, un compte à rebours 3-2-1 relance la course.

## Écran d'accueil

L'accueil s'inspire de Subway Surfers, avec le style de Neko Odyssey. Ton chat est debout en grand sur le toit, avec son chapeau et son déguisement, sous le titre **Neko Odyssey**. Il suffit de toucher le décor (ou « Touche pour jouer », ou `Espace`) pour lancer une partie.

- **En haut** : les croquettes, les poissons d'or, la musique et les bruitages.
- **À gauche** : le meilleur score avec le portrait du chat, le niveau et sa barre d'expérience, le cadeau du jour (quand il est disponible) et l'album.
- **À droite** : la fête en cours, le défi du jour avec sa progression, le classement et la carte du voyage (avec la ville actuelle).
- **En bas** : quatre gros boutons, **Missions** (défi du jour et missions, avec le nombre de missions en cours), **Moi** (nom du chat, classe, album, comment jouer), **Boutique** et **Histoire**.

## Sur les toits

- **Croquettes en forme de poisson** : attrape-les, chacune rapporte 10 points.
- **Flaque d'eau** : si le chat marche dedans, la partie est perdue. Saute par-dessus ou change de couloir.
- **Antenne basse** : saute par-dessus.
- **Grande antenne** : passe dessous en roulade.
- **Cheminée** : trop haute pour sauter, il faut changer de couloir.

La vitesse augmente au fil de la partie et les obstacles deviennent plus nombreux. Le score compte la distance parcourue et les croquettes. Le meilleur score est enregistré dans le navigateur.

## Interface

- **Accueil** : voir « Écran d'accueil » plus haut. Téléphone couché, les cartes passent sur les côtés, avec le titre, le chat et « Touche pour jouer » au milieu.
- **Fenêtres** : chaque fenêtre (Histoire, Album, Carte, Classement, Boutique, Missions, Moi, Ta classe, Partage, « D'où repars-tu ? ») a une petite croix ✕ en haut à droite pour la fermer. Elle reste visible quand on fait défiler et fait la même chose que le petit bouton « Retour » (ou « Fermer ») centré en bas de la fenêtre. Dans la boutique, les onglets Chats, Chapeaux et Poissons d'or restent en haut de l'écran avec la croix quand on descend.
- **Fin de partie** : le chat de face, la ville et la rue atteintes, le score et le bouton **Rejouer** d'abord, puis l'expérience, la nouvelle ville éventuelle, le prochain chat à débloquer et les missions.
- **Système de design** : toutes les couleurs, tailles de texte (7), arrondis (4) et espacements viennent de variables CSS. Les textes font au moins 13 px et chaque bouton au moins 44 px de haut.

## L'histoire

Au premier lancement, le joueur donne un nom à son chat (« Neko » par défaut). Pour le changer ensuite, il suffit de toucher le nom sur l'écran d'accueil.

L'histoire suit le voyage à travers la France et compte **35 chapitres, un par ville** : une nuit d'orage, Neko s'endort dans un camion à Besançon et se réveille au port de Marseille. Il suit la piste de Plume, sa petite sœur, le long de la Méditerranée et jusqu'à Bordeaux, remonte la côte atlantique et la Bretagne avec le Capitaine, passe par Paris, le Nord et l'Alsace, puis rattrape Maman Chat dans les Alpes avant de rentrer à Besançon au niveau 171. En chemin : Gaston le pigeon, Filou le chat errant, la chouette du Capitole, l'éléphant de Nantes, les cigognes de Colmar… Chaque chapitre se lit aussi depuis la fiche de sa ville sur la carte.

**Cinq chats spéciaux de l'histoire sont offerts en chemin** : Filou (niveau 16, Gordes), Comète (41, Carcassonne), Plume (61, Bordeaux), Capitaine (81, Quimper) et Légende (171, Besançon). Chacun a une aura et laisse une traînée pendant la course : fumée pour Filou, étoiles pour Comète, plumes pour Plume, bulles pour Capitaine et paillettes dorées pour Légende.

## Niveau du joueur

Chaque partie donne de l'expérience (XP) selon la distance parcourue, les croquettes, les bonnes réponses et les missions réussies. Il faut quelques parties par niveau. Arriver à Besançon (niveau 171) demande environ une fois et demie le temps qu'il fallait pour l'ancien niveau 100. Le niveau maximum est 175. Chaque nouveau niveau rapporte des croquettes (50 + 5 par niveau, au maximum 250).

### Le voyage à travers la France

Neko traverse la France de toit en toit : **35 villes, une nouvelle tous les 5 niveaux**. Le voyage part de Marseille, longe la Côte d'Azur et la Provence, passe par le Sud-Ouest, la Bretagne, la Normandie, Paris, le Nord, l'Alsace, l'Auvergne et les Alpes, et se termine à Besançon (niveau 171).

Marseille, Saint-Tropez, Nice, Gordes, Avignon, Arles, Nîmes, Montpellier, Carcassonne, Toulouse, Lourdes, Biarritz, Bordeaux, La Rochelle, Nantes, Carnac, Quimper, Saint-Malo, le Mont-Saint-Michel, Étretat, Rouen, Paris, Amiens, Lille, Reims, Strasbourg, Colmar, Vesoul, Dijon, Clermont-Ferrand, Lyon, Grenoble, Annecy, Chamonix, Besançon.

Chaque ville a son décor : ses monuments à l'horizon (la Bonne Mère, la tour Eiffel, le Mont-Saint-Michel, le mont Blanc…), la mer, un lac, une rivière, des montagnes ou des champs de lavande, la forme de ses toits (toits provençaux, haussmanniens, pignons flamands, maisons alsaciennes, chalets…) et la couleur des toits sur lesquels court le chat (tuiles, ardoise, zinc, briques…). Pendant la course, le compteur affiche la ville et la rue où court le chat. Les rues sont de vrais lieux connus de chaque ville, 8 par ville (la Canebière, la promenade des Anglais, les Champs-Élysées, la Petite France…), et une bulle annonce chaque nouvelle rue. L'écran de fin rappelle la ville et la rue atteintes, et annonce chaque nouvelle ville avec un bouton « Voir la carte ». Pendant les fêtes, le décor de la fête garde ses couleurs et ses objets, et la ville garde ses monuments et ses toits.

Au départ de chaque course, le nom de la ville et sa région s'affichent en grand.

**La carte** (bouton *Carte* sur l'accueil) montre la France, le trajet de Neko et un point par ville : orange pour les villes traversées, le point qui pulse pour la ville actuelle, gris pour les villes à venir. Touche la carte près d'une ville (ou utilise les flèches, aussi au clavier) pour ouvrir sa fiche : une illustration de nuit avec son monument, sa région, ses niveaux et une anecdote. Le bouton **Rejouer à …** relance une ville déjà traversée, avec les obstacles de ses niveaux ; le niveau du joueur ne baisse jamais et l'expérience gagnée compte toujours. « Rejouer » reste dans cette ville, le retour à l'accueil ramène à la ville actuelle. Les villes à venir restent cachées : leur fiche indique combien de niveaux il reste avant d'y arriver. Le bouton **Lire le chapitre** ouvre le chapitre de l'histoire de la ville.

En haut de l'écran de fin, le chat apparaît de face : triste après une chute, tout content avec des étoiles quand il bat son record.

### Ce qui change sur les toits avec le niveau

Plus le joueur monte de niveau, plus les toits sont chargés : un peu plus d'obstacles, des enchaînements plus serrés et une vitesse de départ un peu plus élevée, jusqu'au niveau 60. De nouvelles choses apparaissent aussi :

| Niveau | Nouveauté | Comment faire |
| --- | --- | --- |
| 5 | Cordes à linge | roule dessous |
| 8 | Croquettes dorées | elles valent 5 croquettes |
| 12 | Climatiseurs | ils sont hauts : saute au bon moment |
| 18 | Pelotes de laine | +300 points |
| 20 | Pots de fleurs qui roulent vers toi | saute par-dessus |
| 25 | Panneaux solaires | monte sur la rampe et cours en hauteur (attention à ne pas foncer dans le côté) |
| 30 | Sacs de croquettes | +15 croquettes |
| 35 | Trous entre deux toits, sur toute la largeur | saute par-dessus |
| 45 | Lucarnes qui s'ouvrent et se ferment | passe quand elles sont fermées, ou saute |

L'écran de fin annonce la nouveauté quand elle se débloque.

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

## Poissons d'or

Les poissons d'or sont des objets très rares : il y a **1 chance sur 15** qu'un poisson d'or se cache dans chaque rue. Il brille et flotte au-dessus du toit, et rapporte aussi 100 points. On les garde d'une partie à l'autre.

- **Seconde chance** : quand le chat perd, une fenêtre propose pendant 10 secondes d'utiliser 1 poisson d'or pour repartir au même endroit (l'obstacle disparaît, un bouclier protège 2 secondes, puis compte à rebours 3-2-1). C'est possible **une seule fois par partie**. Un bouton « Passer » permet de refuser.
- **Déguisements de fête** (6 poissons d'or) : un ou deux par fête, en vente seulement pendant sa fête, gardé ensuite toute l'année. Ils se portent avec n'importe quel chat et n'importe quel chapeau.

| Fête | Déguisement |
| --- | --- |
| Halloween | Vampire (cape et col), Fantôme (drap avec des yeux) |
| Noël | Renne (bois et écharpe), Lutin (tunique et col à grelots) |
| Pâques | Poussin, Abeille (rayures, ailes et antennes) |
| Saint-Valentin | Cupidon (ailes et carquois) |
| Nouvel An chinois | Dragon (écailles et crête) |
| Nouvel An | Tenue de soirée |
| Été et 14 Juillet | Bouée, Marin (marinière et col de marin) |
| Fête de la musique | Rock star (guitare) |
| Poisson d'avril | Sardine (écailles et nageoires) |
| Journée du chat | Super-chat (cape) |

- **Pouvoirs pour la prochaine partie** : bonus deux fois plus longs (3 poissons), départ rapide une rue plus loin avec un bouclier de 5 secondes (3), indice qui élimine une mauvaise réponse à chaque question (2), aimant de départ de 30 secondes (2).
- **Changer une mission** : 1 poisson d'or, avec le bouton « Changer » sous chaque mission.
- **Échange** : 1 poisson d'or contre 500 croquettes.

Tout se trouve dans l'onglet **Poissons d'or** de la boutique. L'album montre aussi les déguisements obtenus.

## Rues et questions de culture générale

Toutes les 30 secondes, la course fait une pause et propose jusqu'à 3 questions, tirées parmi 7 sujets (sciences et nature, histoire et géographie, français et maths, arts et culture, **les chats**, **anglais** et **la France**), soit environ 850 questions réparties sur 4 niveaux de classe. Dans le sujet « La France », certaines questions portent sur la ville où court le chat (2 par ville). Une question bien répondue ne revient plus. Une question ratée revient 3 pauses-questions plus tard. Quand l'enfant a bien répondu à toutes les questions de son niveau dans un sujet, il reçoit celles du niveau au-dessus ; quand tout est réussi, les plus anciennes reviennent. Chaque bonne réponse rapporte 1 croquette. Chaque question passée retire 2 croquettes du compteur de la partie (jamais en dessous de 0). En cas d'erreur, le jeu donne la bonne réponse et une explication. Ensuite, un compte à rebours 3-2-1 relance la course. Le chat passe ensuite de rue en rue (sans pause) : la 1re rue fait 1 km, puis chaque rue fait 500 m de plus que la précédente (1,5 km, 2 km, 2,5 km…).

**Reprendre à la rue atteinte** : le jeu retient la rue la plus loin que tu as atteinte. Dès que tu as atteint la 2e rue, « Jouer » et « Rejouer » te proposent de « Reprendre à la Ne rue » ou de « Repartir de la 1re rue ». Quand tu reprends plus loin, tu as 3 secondes de bouclier, et les points ne comptent que pour la distance que tu cours vraiment. Le record reste donc juste.

## Classement entre amis

Le bouton **Classement** (sur l'accueil et l'écran de fin) ouvre un classement en ligne. Chaque joueur s'inscrit avec un pseudo, sans compte ni mot de passe. Quatre onglets : **Score** (meilleur score), **Plus loin** (distance la plus longue atteinte), **Niveau** (niveau du joueur) et **Collection** (chats, chapeaux et déguisements obtenus). Le jeu envoie les résultats à la fin de chaque partie. Si tu n'es pas dans les 30 premiers, ta place s'affiche en bas de la liste.

Le classement utilise Firebase et marche sur la version publiée sur GitHub Pages. Pour l'activer, suis le guide [FIREBASE.md](FIREBASE.md).

## Classe et difficulté des questions

Au premier lancement, le joueur choisit sa classe (du CP à la 3e, ou « Lycée et + »). Elle se change dans **Moi › Classe**, sur l'écran d'accueil. Le jeu ajuste ensuite un peu la difficulté : après 3 bonnes réponses d'affilée, les questions deviennent plus difficiles, et après 2 erreurs d'affilée, plus faciles. Les calculs sont générés automatiquement et changent à chaque fois.

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

Pour que la collection dure, on peut avoir **au maximum 5 chats le premier jour de jeu** (Roux compris), puis un de plus chaque nouveau jour où l'on joue. Les chats spéciaux offerts par l'histoire ne comptent pas dans cette limite.

| Chat | Prix |
| --- | --- |
| Roux | offert |
| Gris | 500 |
| Noir | 800 |
| Crème | 1 000 |
| Blanc | 1 200 |
| Tigré brun | 1 600 |
| Tigré argenté | 2 000 |
| Tuxedo | 2 800 |
| Chartreux | 3 400 |
| Siamois | 4 200 |
| Calico | 5 600 |
| Écaille de tortue | 6 400 |
| Rose | 7 300 |
| Bengal (tacheté) | 8 200 |
| Bleu nuit (avec des étoiles) | 9 200 |
| Doré (qui brille) | 11 600 |
| Arc-en-ciel (qui change de couleur) | 15 000 |

## Les chapeaux

Dans l'onglet **Chapeaux** de la boutique, les croquettes servent aussi à acheter des chapeaux. Chaque chapeau va sur n'importe quel chat.

| Chapeau | Prix |
| --- | --- |
| Bonnet à pompon | 300 |
| Casquette à l'envers | 450 |
| Bob de pêcheur (avec un petit poisson qui pend) | 600 |
| Toque de chef | 900 |
| Couronne de fleurs | 1 100 |
| Pastèque | 1 200 |
| Béret baguette | 1 500 |
| Cow-boy | 2 000 |
| Casque de pompier | 2 300 |
| Haut-de-forme | 2 600 |
| Couronne | 3 200 |
| Chapeau de pirate | 3 500 |
| Bonnet de nuit étoilé | 3 800 |
| Mini-antenne (avec une lumière qui clignote) | 4 200 |
| Bonnet à hélice (qui tourne) | 4 500 |
| Casque de ramoneur (avec une lampe qui éclaire devant) | 4 800 |
| Sorcière | 5 600 |
| Viking | 6 500 |
| Corne de licorne | 7 500 |
| Auréole | 9 000 |

## Les thèmes de fête

Le jeu change tout seul de décor pendant les fêtes, selon la date de l'appareil. Pendant un thème, le ciel, les toits, les obstacles et les objets à ramasser changent d'apparence (les règles restent les mêmes), et un chapeau en **édition limitée** est en vente dans la boutique à 1 500 croquettes. Une fois acheté, il reste à toi toute l'année.

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

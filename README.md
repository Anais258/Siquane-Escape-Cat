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

Tout le jeu tient dans un seul fichier, `index.html` (HTML, CSS et JavaScript, dessin sur `<canvas>`, sons générés avec la Web Audio API).

# Publier Neko Odyssey sur le Google Play Store

Ce dossier contient tout ce qu'il faut pour la fiche du Play Store :

| Fichier | Où le mettre dans la Play Console |
| --- | --- |
| `icone-512.png` | Fiche principale › Icône de l'appli (512 × 512) |
| `banniere-1024x500.png` | Fiche principale › Image de présentation (1024 × 500) |
| `capture-1-accueil.png` … `capture-5-boutique.png` (accueil, course à Paris, carte de France, questions, boutique) | Fiche principale › Captures d'écran du téléphone (1080 × 2160), dans cet ordre |

Politique de confidentialité : `https://siquane.github.io/Neko-Odyssey/confidentialite.html`

## Avant de commencer : protéger ta vie privée (micro-entreprise)

Avec un compte développeur **entreprise**, Google affiche sur la fiche le nom et l'adresse de l'entreprise. Une micro-entreprise porte ton nom et a ton adresse personnelle : il faut donc d'abord les remplacer.

1. **Prendre une domiciliation d'entreprise** (environ 10 à 30 € par mois, par exemple Kandbaz, SeDomicilier ou Legalstart). Tu reçois un contrat de domiciliation et une nouvelle adresse professionnelle.
2. **Faire une seule modification sur le Guichet unique** : <https://formalites.entreprises.gouv.fr> › *Modifier une entreprise*. Dans la même demande :
   - **transfert d'adresse** vers l'adresse de domiciliation (joindre le contrat) ;
   - **nom commercial** : `Siquane Lab` ;
   - **activité complémentaire** : *Édition de jeux électroniques* (code APE 58.21Z).
   C'est gratuit pour une micro-entreprise.
3. **Attendre le nouvel avis de situation INSEE** (sur <https://avis-situation-sirene.insee.fr>) avec la nouvelle adresse et le nom commercial. Comptez une à quelques semaines.
4. **Demander le numéro D-U-N-S** une fois l'avis à jour, depuis le lien proposé par la Play Console à la création du compte (gratuit, quelques jours à 2 semaines). Le nom et l'adresse doivent être **exactement** ceux de l'avis INSEE.
5. **Déposer la marque « Neko Odyssey »** à l'INPI (190 € pour une classe, + 40 € pour la 2e : classes 9 et 41), idéalement avant la sortie sur le Play Store, au plus tard juste après.

Où on en est : ✅ domiciliation prise, ✅ nom « Neko Odyssey » vérifié libre à l'INPI et jeu archivé (Software Heritage, Wayback Machine) le 27 octobre 2026. Prochaine étape : la modification au Guichet unique.

Détail de la modification au Guichet unique :
- *Modifier une entreprise* › choisir la micro-entreprise, cocher les trois changements dans la même demande.
- **Transfert d'adresse** : adresse de domiciliation + nom et SIREN du domiciliataire (sur le contrat).
- **Nom commercial** : `Siquane Lab`.
- **Ajout d'activité** : « Conception et édition de jeux vidéo et d'applications mobiles » (l'INSEE attribue le code, normalement 58.21Z).
- Joindre le contrat de domiciliation, signer, envoyer (gratuit).
- Après validation : vérifier le nouvel avis de situation INSEE (adresse et nom commercial) **avant** de demander le D-U-N-S. Mettre à jour l'adresse auprès de la banque pro, de l'URSSAF et sur les factures.

Points à vérifier :
- Le **nom légal** d'une micro-entreprise reste ton nom : Google peut l'afficher dans les détails du développeur à côté du nom commercial. Seule une société (SASU, EURL…) permettrait de ne plus du tout l'afficher.
- Ne jamais utiliser ton adresse personnelle dans la Play Console, le D-U-N-S ou le profil de paiement.
- Pour la fiscalité des futurs achats (catégorie de revenus, plafonds), faire valider par l'URSSAF ou un comptable.

## Étapes

1. **Compte développeur entreprise** : sur <https://play.google.com/console>, créer un compte développeur de type **Organisation** (25 $ une seule fois). Renseigner le nom commercial `Siquane Lab`, l'adresse de domiciliation, le numéro D-U-N-S, le site `https://siquane.github.io/Neko-Odyssey/` et l'e-mail `siquane.lab@gmail.com`. Google vérifie l'organisation (quelques jours).
2. **Paquet Android** : sur <https://www.pwabuilder.com>, coller `https://siquane.github.io/Neko-Odyssey/`, puis *Package for stores* › *Android* › *Generate package*.
   - Package ID : `io.github.siquane.nekoodyssey`
   - App name : `Neko Odyssey`, Launcher name : `Neko Odyssey`
   - Display mode : `Fullscreen`, Orientation : `Portrait`
   - Signing key : *Create new*. **Garder précieusement** le fichier de clé (`signing.keystore`) et ses mots de passe (`signing-key-info.txt`) : sans eux, impossible de publier une mise à jour.
   - PWABuilder donne un `.aab` (à envoyer sur Google Play) et un `assetlinks.json`.
3. **Prouver que le site est à toi (assetlinks)** : le fichier doit être servi à `https://siquane.github.io/.well-known/assetlinks.json`, à la racine du domaine. Le jeu étant dans le sous-dossier `/Neko-Odyssey`, il faut créer sur GitHub un dépôt public nommé exactement `siquane.github.io` et y mettre `.well-known/assetlinks.json` (plus un fichier vide `.nojekyll` pour que GitHub publie le dossier `.well-known`). Après l'envoi du `.aab`, ajouter aussi l'empreinte SHA-256 de la clé de Google (Play Console › Intégrité de l'appli › Certificat de la clé de signature). Sans ce fichier, l'appli marche mais affiche une barre d'adresse Chrome en haut.
4. **Créer l'appli** dans la Play Console : nom `Neko Odyssey`, langue par défaut français, *Jeu*, *Gratuit*.
5. **Remplir la fiche** avec les textes ci-dessous et les images de ce dossier.
6. **Test interne (conseillé)** : avec un compte entreprise, le test fermé de 14 jours n'est pas obligatoire. Envoyer quand même le `.aab` d'abord en *Test interne* pour l'installer sur ton téléphone et celui de quelques amis, et vérifier que tout marche.
7. **Production** : envoyer le même `.aab` en *Production*, puis *Envoyer pour examen*. Google examine l'appli (de quelques heures à quelques jours) avant qu'elle apparaisse sur le Play Store.

## Textes de la fiche

**Nom de l'appli** (30 caractères max)
> Neko Odyssey

**Description courte** (80 caractères max)
> Traverse la France de toit en toit et ramène ton chat chez lui !

**Description complète**
> Une nuit d'orage, Neko s'est endormi dans un camion de livraison… et s'est réveillé à Marseille, à l'autre bout de la France. Pour retrouver sa famille à Besançon, il n'y a qu'un chemin : courir de toit en toit !
>
> 🐾 **Une course pleine de surprises**
> Change de couloir, saute par-dessus les flaques et les antennes, roule sous les cordes à linge, grimpe sur les panneaux solaires… Plus tu montes de niveau, plus les toits réservent de surprises. Tu as perdu ? Reprends ta course à la rue où tu t'es arrêté.
>
> 🐟 **Ramasse, collectionne, habille ton chat**
> Ramasse des croquettes pour débloquer plus de 20 chats (siamois, calico, bengal, arc-en-ciel…), 30 chapeaux et des déguisements de fête. Attrape les rares poissons d'or pour une seconde chance.
>
> 🧠 **Apprends en jouant**
> Toutes les 30 secondes, la course fait une pause pour 3 questions adaptées à ta classe, du CP au lycée. Près de 850 questions : sciences, histoire, français, maths, arts, anglais, la France (avec des questions sur chaque ville traversée)… et les chats !
>
> 🗺️ **Un voyage à travers la France**
> De Marseille à Besançon, 35 villes à traverser : la Côte d'Azur, la Provence, le Pays basque, la Bretagne, le Mont-Saint-Michel, Paris, l'Alsace, les Alpes… Chaque ville a ses monuments, ses toits et une anecdote à découvrir sur la carte.
>
> 📖 **Une histoire en 35 chapitres**
> Un chapitre par ville. Rencontre Gaston le pigeon, Filou le chat errant, le vieux Capitaine et bien d'autres, retrouve Plume ta petite sœur, et gagne des chats spéciaux en chemin.
>
> 🎃 **Des fêtes toute l'année**
> Halloween, Noël, Nouvel An chinois, Pâques, l'été… le décor, la musique et les objets changent, avec des chapeaux et déguisements en édition limitée.
>
> 🏆 **Défie tes amis**
> Missions, défi du jour, cadeau quotidien et classement entre amis avec un simple pseudo.
>
> ✅ Gratuit, sans publicité et sans achat intégré. Jouable hors connexion.

**Catégorie** : Jeux › Arcade
**Tags** : Course infinie, Arcade, Éducatif, Animaux, Hors connexion
**E-mail de contact** : siquane.lab@gmail.com
**Site web** : `https://siquane.github.io/Neko-Odyssey/`

## Questionnaires de la Play Console

**Publicités** : Non, l'appli ne contient pas de publicité.

**Accès à l'appli** : Toutes les fonctionnalités sont disponibles sans restriction (pas de connexion).

**Public cible** : choisir les tranches d'âge visées. Si des moins de 13 ans sont inclus, l'appli suit le règlement *Familles* (déjà compatible : pas de pub, pas d'achat, aucune donnée personnelle demandée).

**Classification du contenu** (questionnaire IARC) : jeu, pas de violence (le chat glisse ou se cogne, sans blessure), pas de langage grossier, pas de contenu sexuel, pas de drogues, pas de jeux d'argent. Interaction entre utilisateurs : non (seulement un classement avec pseudo, pas de chat ni d'échange). Résultat attendu : *Tout public / PEGI 3*.

**Sécurité des données** :
- L'appli collecte-t-elle des données ? **Oui** (seulement pour le classement, facultatif).
- Types : *Identifiants de l'appareil ou autres* › identifiant utilisateur (anonyme, créé par Firebase) ; *Activité dans l'appli* › autres actions (pseudo et scores).
- Partagées avec des tiers : **Non** (Firebase agit pour le compte de l'appli).
- Collecte facultative : **Oui** (seulement si le joueur choisit un pseudo).
- Finalité : *Fonctionnalités de l'appli* (classement).
- Chiffrées en transit : **Oui** (HTTPS).
- Suppression possible : **Oui**, dans le jeu (*Classement › Supprimer mes données du classement*).

**Appli d'actualités / santé / finance / gouvernement** : Non.

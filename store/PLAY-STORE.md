# Publier Neko Odyssey sur le Google Play Store

Ce dossier contient tout ce qu'il faut pour la fiche du Play Store :

| Fichier | Où le mettre dans la Play Console |
| --- | --- |
| `icone-512.png` | Fiche principale › Icône de l'appli (512 × 512) |
| `banniere-1024x500.png` | Fiche principale › Image de présentation (1024 × 500) |
| `capture-1-accueil.png` … `capture-4-questions.png` | Fiche principale › Captures d'écran du téléphone (1080 × 2160) |

Politique de confidentialité : `https://siquane.github.io/Neko-Odyssey/confidentialite.html`

## Étapes

1. **Compte développeur** : sur <https://play.google.com/console>, créer un compte développeur personnel (25 $ une seule fois, vérification d'identité, 18 ans ou plus).
2. **Paquet Android** : sur <https://www.pwabuilder.com>, coller `https://siquane.github.io/Neko-Odyssey/`, puis *Package for stores* › *Android* › *Generate package*.
   - Package ID : `io.github.siquane.nekoodyssey`
   - App name : `Neko Odyssey`, Launcher name : `Neko Odyssey`
   - Display mode : `Fullscreen`, Orientation : `Portrait`
   - Signing key : *Create new*. **Garder précieusement** le fichier de clé (`signing.keystore`) et ses mots de passe (`signing-key-info.txt`) : sans eux, impossible de publier une mise à jour.
   - PWABuilder donne un `.aab` (à envoyer sur Google Play) et un `assetlinks.json`.
3. **Prouver que le site est à toi (assetlinks)** : le fichier doit être servi à `https://siquane.github.io/.well-known/assetlinks.json`, à la racine du domaine. Le jeu étant dans le sous-dossier `/Neko-Odyssey`, il faut créer sur GitHub un dépôt public nommé exactement `siquane.github.io` et y mettre `.well-known/assetlinks.json` (plus un fichier vide `.nojekyll` pour que GitHub publie le dossier `.well-known`). Après l'envoi du `.aab`, ajouter aussi l'empreinte SHA-256 de la clé de Google (Play Console › Intégrité de l'appli › Certificat de la clé de signature). Sans ce fichier, l'appli marche mais affiche une barre d'adresse Chrome en haut.
4. **Créer l'appli** dans la Play Console : nom `Neko Odyssey`, langue par défaut français, *Jeu*, *Gratuit*.
5. **Remplir la fiche** avec les textes ci-dessous et les images de ce dossier.
6. **Test fermé** : pour un nouveau compte personnel, Google demande un test fermé avec au moins 12 testeurs pendant 14 jours avant la production. Envoyer le `.aab` dans *Test fermé*, ajouter les adresses Gmail des amis testeurs, leur envoyer le lien d'inscription.
7. **Production** : après les 14 jours, demander l'accès à la production et publier.

## Textes de la fiche

**Nom de l'appli** (30 caractères max)
> Neko Odyssey

**Description courte** (80 caractères max)
> Cours sur les toits, saute les obstacles et ramène ton chat perdu chez lui !

**Description complète**
> Une nuit d'orage, Neko s'est endormi dans un camion de livraison… et s'est réveillé au cœur d'une ville inconnue. Pour retrouver sa famille, il n'y a qu'un chemin : courir de toit en toit !
>
> 🐾 **Une course pleine de surprises**
> Change de couloir, saute par-dessus les flaques et les antennes, roule sous les cordes à linge, grimpe sur les panneaux solaires… Plus tu montes de niveau, plus les toits réservent de surprises.
>
> 🐟 **Ramasse, collectionne, habille ton chat**
> Ramasse des croquettes pour débloquer plus de 20 chats (siamois, calico, bengal, arc-en-ciel…), 30 chapeaux et des déguisements de fête. Attrape les rares poissons d'or pour une seconde chance.
>
> 🧠 **Apprends en jouant**
> Toutes les 30 secondes, la course fait une pause pour 3 questions adaptées à ta classe, du CP au lycée : sciences, histoire, français, maths, arts, anglais… et les chats !
>
> 📖 **Une histoire en 21 chapitres**
> Chaque niveau rapproche Neko de chez lui. Rencontre Gaston le pigeon, Filou le chat errant et bien d'autres, et gagne des chats spéciaux en chemin.
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
**E-mail de contact** : à renseigner (obligatoire, visible sur la fiche)
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

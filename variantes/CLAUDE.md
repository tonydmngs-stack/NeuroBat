# Variantes — règles d’identité visuelle (à respecter strictement)

Ce dossier sert à proposer des **variantes de design** du site NEUROBAT. Les faits, le périmètre des services et les
données (contact, Web3Forms, mentions légales) restent ceux du `CLAUDE.md` à la racine : on change la forme, pas le fond.

Demande de Tony (12/11/2026) : le site principal fait « trop généré par une IA ». Toute variante ici doit avoir une
identité **ancrée dans le métier du bâtiment**, qui ne ressemble ni à un site de start-up tech, ni à une maquette
produite par une IA. En cas de doute entre « joli et générique » et « juste et métier », choisir **juste et métier**.

## 1. Le principe directeur : le dossier de chantier

Le site doit ressembler à un **document de chantier bien tenu**, pas à une application : papier, encre, traits fins,
cartouche, lots numérotés, tableaux, plans avec leurs conventions de dessin. Les références sont celles que Tony manipule
tous les jours : plans d’exécution, CCTP, DPGF, planning de chantier, DOE, carnet de chantier, signalisation de chantier.

## 2. Interdits (les signes d’un site « fait par une IA »)

### Visuel
- Fond noir ou bleu nuit, effets lumineux (glow, halo, néon), dégradés, flous, effet verre (glassmorphism).
- Réseaux de points reliés, constellations, particules, « circuits imprimés », globes, ondes, hexagones.
- Grilles de cartes arrondies à bordure fine toutes identiques, ombres portées, coins très arrondis.
- Icônes décoratives, pictogrammes génériques, emojis.
- Animations décoratives (apparitions au défilement, éléments qui flottent, compteurs qui défilent).
- La police Inter (et Poppins, Montserrat, Space Grotesk, et les polices « tech » à chasse fixe utilisées pour faire moderne).
- Étiquettes en petites majuscules espacées au-dessus de chaque titre (« VOLET 1 · LE BÂTI »).
- Hero centré « grand titre + sous-titre + deux boutons » ; encadrés « En bref » ; numérotation décorative 01 / 02 / 03.

### Images
- **Aucune image générée par IA**, aucune photo de banque d’images (open spaces lumineux, mains sur un clavier, casques blancs souriants).
- Seulement : de **vraies photos** prises par Tony ou Lorenzo (chantier, matériel, baie, plans), ou des **dessins techniques**
  qui respectent les conventions du métier. Tant qu’une photo n’existe pas, on montre un cadre vide avec sa légende
  (« Photo à venir »), jamais une image de remplacement.

### Texte
- Vocabulaire de plaquette : solution, innovant, sur mesure, clé en main, accompagner, optimiser, synergie, expertise,
  écosystème, au cœur de, booster, révolutionner, « à l’ère de… », « dans un monde où… ».
- Tournures typiques de l’IA : « Pas seulement X, mais Y », « X. Y. Z. » en trois mots, les énumérations systématiques
  par trois, les questions rhétoriques en ouverture, les tirets cadratins (—) au milieu des phrases.
- Promesses vagues ou superlatives (« le meilleur », « une expérience unique »), chiffres non sourcés.
- Phrases toutes de la même longueur et de la même construction.

### Structure
- Le gabarit « hero / 3 cartes / bandeau / 3 cartes / appel à l’action » répété.
- Des sections qui disent toutes la même chose avec des mots différents.

## 3. Ce qu’on utilise à la place

### Couleurs (palette « papier et encre »)
| Rôle | Valeur |
|---|---|
| Papier (fond) | `#efece4` |
| Papier foncé (zones, cloisons) | `#e2ddd1` |
| Encre (texte, traits) | `#1b1a17` |
| Encre secondaire | `#4a463e` |
| Trait fin / filets | `#b9b2a4` |
| **Orange signalisation** (seule couleur d’accent : réseau, numéros de section, liens) | `#b8410e` |

Une seule couleur d’accent. Pas de deuxième couleur vive. Le contraste du texte doit rester lisible (AA minimum).

### Typographie
- Titres et éléments « documents » (cartouche, tableaux, légendes) : **Archivo** en largeur étroite (`font-stretch` ~75 %),
  qui rappelle la signalétique de chantier.
- Texte courant : **Source Serif 4**, une vraie police de lecture, comme un document imprimé.
- Pas de texte en majuscules espacées ; les majuscules sont réservées aux sigles (LAN, CCTP, DOE).

### Mise en page
- Une seule colonne de lecture, avec une **marge de gauche** qui porte les numéros de section et des notes, comme un
  document annoté. Filets horizontaux épais entre les sections (comme un changement de lot dans un CCTP).
- Coins droits, traits pleins, pas d’ombre. Les tableaux sont de vrais tableaux.
- Peu de boutons : des liens soulignés suffisent. Un seul bouton : envoyer le formulaire.

### Éléments graphiques métier (à privilégier)
- **Cartouche** (le bloc d’identification en bas à droite des plans) pour présenter le projet : projet, objet, secteur,
  phase, indice de révision, date.
- **Lots** (A, B, C…) et **descriptif** sous forme de tableau : ce qu’on fait / ce que le client reçoit.
- **Planning** de type diagramme de Gantt, sans durées inventées (axe du temps sans unité).
- **Plan de principe** dessiné avec les conventions : murs existants hachurés, cloisons neuves en trait plein, portes
  avec leur arc, flèche du nord, légende, mention « sans échelle ».

### Mouvement
- Aucune animation décorative. Seules les transitions utiles (survol d’un lien, focus d’un champ) sont autorisées.

## 4. Le ton : comme Tony parle d’un chantier
- Phrases concrètes, avec des mots du métier : cloison, saignée, goulotte, faux plancher, baie, tirage de câbles, réception.
- « On » ou « nous », au présent. Des phrases de longueurs différentes. Une idée par phrase.
- Partir de ce qu’on voit sur le terrain, pas d’un concept.
- Dire honnêtement où en est le projet : l’entreprise n’est pas encore créée.

Exemples :
- ✗ « Nous accompagnons les entreprises avec une solution clé en main innovante. »
- ✓ « On rénove vos bureaux, et on tire le réseau pendant que les cloisons sont encore ouvertes. »
- ✗ « Pas seulement un chantier — une vision. »
- ✓ « Quand l’informaticien arrive après nous, il perce là où on vient de peindre. On veut éviter ça. »

## 5. Check-list avant de livrer une variante
1. Aucun élément de la liste « Interdits » (relire visuel, images, texte, structure).
2. Relire chaque phrase : un chef de chantier pourrait-il l’avoir écrite ? Sinon, la réécrire.
3. Les faits respectent le `CLAUDE.md` racine (périmètre Wi-Fi / LAN, pas de NIS 2, pas de badges ni caméras, Décret
   Tertiaire bien précisé, pas de chiffres non sourcés).
4. Formulaire de contact fonctionnel (Web3Forms, case « Je ne suis pas un robot », lien vers les mentions légales).
5. Testé sur téléphone, tablette et grand écran, sans débordement.
6. Le fichier s’ouvre directement dans un navigateur, sans étape de construction.

## 6. Variantes présentes
- `dossier-chantier.html` : variante « dossier de chantier » (papier, encre, orange signalisation, cartouche, lots,
  planning, plan de principe). Créée le 12/11/2026. Proposition, pas encore validée par Tony.

# NEUROBAT — site vitrine

Projet d'entreprise de Tony Laranjeiro Domingues (apprenti ingénieur travaux, FISA BTP 24-27, CESI Nanterre) :
réhabilitation tertiaire hybride **BTP + cybersécurité** (bureaux), avec son associé Lorenzo Biffi (5ᵉ année, cybersécurité).
Contexte détaillé : `docs-source/` (étude de marché + dossier de candidature « Option Entrepreneuriat »).

## État actuel
- `index.html` : **version de référence retenue par Tony**. Site mono-fichier HTML/CSS/JS, sans dépendance
  hormis la police Inter (Google Fonts). 4 pages en routage par hash : `#accueil`, `#projet` (tag « Projet à venir »),
  `#a-propos`, `#contact`. Fond canvas « réseau de nœuds » (`#net`), câble qui se remplit au scroll dans la section
  « La méthode » (`scrollFx()`), thème noir fixe, formulaire de contact en `mailto:`.
- `variantes/parcours-2d.html` : autre version (canvas 2D vue de dessus, câble qui avance de pièce en pièce).
  Mise de côté, pas retenue pour l'instant. La 3D (Three.js) et le serpent SVG ont été essayés et abandonnés.
- `logo/` : logo final **noir et gris** (chauve-souris dans un projecteur ovale à la place du « O » de NEURO).
  `neurobat-logo-clair.svg` (pour fond clair), `neurobat-logo-sombre.svg` / `-avec-fond.svg` (fond sombre),
  `neurobat-icone.svg`. Lettres converties en tracés : pas de police nécessaire.

## Décisions de design
- Sur mesure, codé à la main, pas de Wix ni de modèle. « Univers réseau » : nœuds, câble, flux.
- Couleurs : noir / gris pour la marque ; bleu électrique (`--blue:#2f7bff`, `--blue2:#4fc3ff`) pour les flux.
- Peu de scroll, fiches d'information lisibles (opaques, pas de fondu faible).
- Mise en page large (`.wrap` max 1440 px) : accueil en 2 colonnes (titre + encadré « En bref »), méthode avec titre fixe à gauche et étapes à droite ; tout repasse sur 1 colonne sous 1000 px.
- Thème noir conservé (essais clair et anthracite refusés). Fond : nœuds qui dérivent lentement + courant électrique discret (1 à la fois, opacité réduite). Page Contact seule : rangée d’immeubles au trait avec réseau intégré (colonnes montantes, branchements, antennes) sur dégradé noir → anthracite, sans nœuds, fonction `city()`/`drawCity()`. Pas de bandes pleine largeur qui masquent le fond.

## À faire (proposé, pas encore validé par Tony)
1. Renommer/garder `index.html` et mettre en ligne (GitHub Pages, Netlify ou Cloudflare Pages).
2. Remplacer l'adresse du formulaire (`Tony.laranjeirodomingues@viacesi.fr`) par une adresse professionnelle.
3. Vérifier et sourcer les chiffres cités (48 %, 4 M m², -50 %) avant toute diffusion externe.
4. Si le site grossit : séparer CSS/JS, ajouter des images (photos de chantier), et éventuellement un vrai backend de formulaire.

## Conventions
- Réponses et textes du site en français.
- Garder le site fonctionnel en ouvrant simplement `index.html` dans un navigateur (pas d'étape de build).

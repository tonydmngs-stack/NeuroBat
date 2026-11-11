# NEUROBAT — site vitrine

Projet d'entreprise de Tony Laranjeiro Domingues (apprenti ingénieur travaux, FISA BTP 24-27, CESI Nanterre) :
réhabilitation tertiaire hybride **BTP + cybersécurité** (bureaux), avec son associé Lorenzo Biffi (5ᵉ année à Oteria, école spécialisée en cybersécurité).
Contexte détaillé : `docs-source/` (étude de marché + dossier de candidature « Option Entrepreneuriat »).

## État actuel
- `index.html` : **version de référence retenue par Tony**. Site mono-fichier HTML/CSS/JS, sans dépendance
  hormis la police Inter (Google Fonts). 4 pages en routage par hash : `#accueil`, `#projet` (tag « Projet à venir »),
  `#a-propos`, `#contact`. Fond canvas « réseau de nœuds » (`#net`), câble qui se remplit au scroll dans la section
  « La méthode » (`scrollFx()`), thème noir fixe, formulaire de contact envoyé directement via **Web3Forms** (clé d’accès publique dans le JS, ~250 messages/mois en gratuit, URL déclarée : le lien GitHub Pages) vers `neurobat.contact@gmail.com` ; champ anti-robot caché ; en cas d’échec, lien de repli `mailto:`. Au passage à `neurobat.fr`, mettre à jour l’URL du site dans Web3Forms.
- `variantes/parcours-2d.html` : autre version (canvas 2D vue de dessus, câble qui avance de pièce en pièce).
  Mise de côté, pas retenue pour l'instant. La 3D (Three.js) et le serpent SVG ont été essayés et abandonnés.
- `logo/` : logo final **noir et gris** (chauve-souris dans un projecteur ovale à la place du « O » de NEURO).
  `neurobat-logo-clair.svg` (pour fond clair), `neurobat-logo-sombre.svg` / `-avec-fond.svg` (fond sombre),
  `neurobat-icone.svg`. Lettres converties en tracés : pas de police nécessaire.

## Décisions de design
- Sur mesure, codé à la main, pas de Wix ni de modèle. « Univers réseau » : nœuds, câble, flux.
- Couleurs : noir / gris pour la marque ; bleu électrique (`--blue:#2f7bff`, `--blue2:#4fc3ff`) pour les flux.
- Peu de scroll, fiches d'information lisibles (opaques, pas de fondu faible).
- Responsive testé de 320 px (petit téléphone) à 3440 px (ultra-large), tablettes portrait/paysage incluses. Taille de texte fluide (`html{font-size:clamp(15px,…,22px)}`) : tout ce qui est en rem grandit avec l’écran.
- Mise en page large (`.wrap` max 90rem) : accueil en 2 colonnes (titre + encadré « En bref »), méthode avec titre fixe à gauche et étapes à droite ; tout repasse sur 1 colonne sous 1000 px.
- Thème noir conservé (essais clair et anthracite refusés). Fond : nœuds qui dérivent lentement + courant électrique discret (1 à la fois, opacité réduite). Page Contact seule : rangée d’immeubles au trait avec réseau intégré (colonnes montantes, branchements, antennes) sur dégradé noir → anthracite, sans nœuds, fonction `city()`/`drawCity()`. Pas de bandes pleine largeur qui masquent le fond.

## Périmètre des services (validé le 11/11/2026, d’après le document réseau de Lorenzo)
- **Bâti** (Tony) : réhabilitation, second œuvre, faux planchers, cloisons, local technique, efficacité énergétique (Décret Tertiaire).
- **Wi-Fi** (Lorenzo) : conseil sur le choix des bornes ; étude de couverture (« survey ») sur plan, ou sur site avec une borne
  de test pour les clients exigeants ; outil Ekahau.
- **LAN** (Lorenzo) : architecture réseau (nombre de switchs, routeurs… à partir de l’étude Wi-Fi), installation des baies et
  équipements (routeur, switchs, pare-feu), tirage des câbles avec l’équipe bâtiment, configuration ; option : forfait maintenance.
- Message côté réseau sur le site : « un réseau qui tient la charge » (couverture étudiée puis vérifiée, réseau dimensionné,
  câblage évolutif). Pare-feu et Wi-Fi invités séparé du réseau de l’entreprise sont cités (configuration des équipements).
  Accueil : bloc « Deux exigences, une réponse » = Décret Tertiaire + réseau fiable ; plus aucune promesse NIS 2 / « cyber-résilient ».
- **Hors périmètre, à ne pas proposer sur le site** : contrôle d’accès / badges, caméras, sécurisation de l’éclairage, du
  chauffage et des objets connectés, tests d’intrusion, accès distant / VPN, protection électromagnétique, conformité NIS 2.

## Mise en ligne et dépôt
- Dépôt GitHub public : https://github.com/tonydmngs-stack/NeuroBat (branche `main`, recréé le 11/11/2026 avec tout l’historique). `.gitignore` bloque les documents
  personnels (`docs-source/`, `prive/`, fichiers Office), identifiants et fichiers système : ne jamais publier de données perso.
- **Site en ligne (GitHub Pages, réactivé le 11/11/2026)** : https://tonydmngs-stack.github.io/NeuroBat/
  (majuscules comprises : l’ancien lien en `neurobat` ne marche plus). Source : `main`, dossier racine.
  L’activation de Pages se fait dans Settings → Pages ; Claude ne peut pas la faire depuis une session cloud.
  `.nojekyll` en place (site servi tel quel). Chaque push sur `main` redéploie le site en ~1 min.
- Nom de domaine `neurobat.fr` : à acheter seulement au lancement de l’entreprise (décision de Tony), puis le brancher sur Pages.

## À faire
1. ~~Mettre en ligne~~ → fait (GitHub Pages actif).
2. ~~Adresse e-mail~~ → fait : `neurobat.contact@gmail.com` (Gmail gratuit, créé le 11/11/2026), utilisée dans la page
   Contact ; le formulaire y envoie les messages via Web3Forms. Au lancement : passer à `contact@neurobat.fr`.
3. ~~Chiffres~~ → vérifiés le 11/11/2026. Sur le site, seul le Décret Tertiaire est cité : texte précisé (≥ 1 000 m² tertiaires,
   -40 % 2030 / -50 % 2040 / -60 % 2050 vs année de référence ; un plateau plus petit est concerné si le bâtiment dépasse le seuil).
   Les chiffres de l’étude de marché ne sont PAS sur le site et ne doivent pas y être ajoutés tels quels :
   « 48 % des cyberattaques sur PME/ETI » (presse ; l’ANSSI donne ~37 % des victimes de rançongiciels → à revérifier dans le
   Panorama ANSSI), « 4 M m² obsolètes (IEIF) » (non retrouvé ; ordres de grandeur trouvés : 5,6 à 6,1 M m² de bureaux vacants
   en IDF), « -50 % de carbone (ADEME) » (pas de chiffre ADEME unique ; « >50 % des émissions liées aux matériaux évitées »).
4. Si le site grossit : séparer CSS/JS, ajouter des images (photos de chantier), (proposé, non validé). Formulaire : fait (Web3Forms).

## Le jour du lancement (déploiement hors GitHub / passage à `neurobat.fr`) — check-list
- **Web3Forms : mettre à jour l’adresse du site** dans les réglages du compte Web3Forms (compte lié à
  `neurobat.contact@gmail.com`). Aujourd’hui l’URL déclarée est https://tonydmngs-stack.github.io/NeuroBat/ ;
  sans cette mise à jour, le formulaire de contact du nouveau site risque de ne plus envoyer les messages.
- Après le changement, envoyer un message de test depuis la page Contact du nouveau site et vérifier sa réception.
- Passer l’adresse de contact à `contact@neurobat.fr` (page Contact + Web3Forms).

## Conventions
- Réponses et textes du site en français.
- Garder le site fonctionnel en ouvrant simplement `index.html` dans un navigateur (pas d'étape de build).

# 📚 Ma Bibliothèque

Une application web pour **cataloguer ses livres en scannant leur code-barres**. Elle tient dans un seul fichier (`index.html`), fonctionne sur téléphone comme sur ordinateur, et garde toutes vos données **sur votre appareil** : pas de compte, pas de serveur.

## Ce que fait l'application

- **Scan d'ISBN** : visez le code-barres avec la caméra, ou photographiez-le, ou tapez le numéro. Les livres s'ajoutent à la suite, sans rien toucher.
- **Fiche automatique** : titre, auteur, éditeur, année, pages, couverture et résumé sont récupérés en ligne (Google Livres, Open Library, catalogue de la BnF).
- **Classement par genre** : roman, policier, SF et fantasy, BD, histoire, économie, cuisine, etc. Chaque livre reçoit une cote de rangement (ex. `ROM CAM`).
- **Trois façons de ranger** : par genre, par auteur (A-Z) ou par état de lecture (à lire, en cours, lu).
- **Couvertures en carrousel** : chaque couverture se retourne pour afficher les caractéristiques du livre. Une vue liste est aussi disponible.
- **Valeur de la bibliothèque** : prix neuf total et revente possible, avec relevé des prix d'occasion de la Bourse aux livres. Vous pouvez aussi saisir une offre Momox ou un montant à la main.
- **Suivi de lecture** : statut, note sur 5 étoiles et avis personnel pour chaque livre.
- **Analyse et « persona » de lecteur** : thématiques dominantes, habitudes, curseurs (fiction/savoirs, classiques/nouveautés…), et un portrait du lecteur pour toute la bibliothèque ou pour une sélection de livres.
- **Livres connexes** : suggestions de lectures proches de vos thèmes ou d'un livre précis, ajoutables en « à lire » d'un geste.
- **Résumés** : tirés de Wikipédia ou de l'éditeur, ou rédigés par Claude si vous renseignez votre propre clé API (facultatif).
- **Export et sauvegarde** : Excel (.xlsx), CSV, et sauvegarde JSON à restaurer après un changement d'appareil.

## Utilisation

1. Ouvrez la page de l'application (voir ci-dessous) dans le navigateur de votre téléphone.
2. Touchez **Scanner** et autorisez la caméra.
3. Visez le code-barres d'un livre : la fiche se remplit toute seule.

> La caméra en direct exige une adresse en **https**. Sur un autre appareil, vous pouvez toujours photographier le code-barres ou saisir l'ISBN.

### Publier avec GitHub Pages

Dans **Settings → Pages**, choisissez la branche `main` et le dossier racine. L'application sera alors accessible à l'adresse `https://benmignard-bit.github.io/BIBLIOTHEQUE/`. Sur iPhone, vous pouvez l'ajouter à l'écran d'accueil depuis Safari pour l'utiliser comme une app.

## Vos données

Les livres sont enregistrés dans le stockage local du navigateur, sur votre appareil uniquement. Pensez à créer une sauvegarde de temps en temps depuis l'écran **Exporter**.

Les clés API facultatives (Google Livres, Claude) restent elles aussi sur l'appareil. Une clé Claude n'est utilisée que pour générer des résumés, et son usage est facturé sur votre compte API.

## Sources en ligne

Google Livres · Open Library · catalogue de la BnF · La Bourse aux livres · Wikipédia · bibliothèques [ZXing](https://github.com/zxing-js/library) (lecture des codes-barres) et [SheetJS](https://sheetjs.com/) (export Excel).

## Technique

Un seul fichier HTML, sans build ni dépendance à installer : HTML, CSS et JavaScript. Les bibliothèques de scan et d'export se chargent à la demande depuis un CDN.

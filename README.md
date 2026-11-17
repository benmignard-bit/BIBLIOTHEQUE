# 📚 Ma Bibliothèque / My Library

🇬🇧 [English](#-english) · 🇫🇷 [Français](#-français)

---

## 🇬🇧 English

A web app to **catalogue your books by scanning their barcodes**. It lives in a single file (`index.html`), works on phones and computers, and keeps all your data **on your own device**: no account, no server.

### What it does

- **ISBN scanning**: point the camera at a book's barcode, take a photo of it, or type the number. Books are added one after another, hands-free.
- **Automatic book sheet**: title, author, publisher, year, page count, cover and summary are fetched online (Google Books, Open Library, BnF catalogue).
- **Genre shelving**: novel, crime, sci-fi and fantasy, comics, history, economics, cooking and more. Each book gets a shelf code (e.g. `ROM CAM`).
- **Three ways to sort**: by genre, by author (A-Z) or by reading status (to read, reading, read).
- **Cover carousel**: each cover flips over to show the book's details. A list view is also available.
- **Library value**: total new price and possible resale value, with used prices pulled from La Bourse aux livres. You can also enter a Momox offer or an amount by hand.
- **Reading tracker**: status, 5-star rating and a personal review for each book.
- **Analysis and reader "persona"**: dominant themes, habits, sliders (fiction/non-fiction, classics/new releases...) and a reader portrait for the whole library or a selection of books.
- **Related books**: reading suggestions close to your themes or to a given book, added to "to read" in one tap.
- **Summaries**: taken from Wikipedia or the publisher, or written by Claude if you provide your own API key (optional).
- **Export and backup**: Excel (.xlsx), CSV, and a JSON backup you can restore on a new device.

### How to use it

1. Open the app page (see below) in your phone's browser.
2. Tap **Scanner** and allow camera access.
3. Aim at a book's barcode: the sheet fills in by itself.

> The live camera requires an **https** address. On any device you can still photograph the barcode or type the ISBN.

### Publish with GitHub Pages

In **Settings → Pages**, pick the `main` branch and the root folder. The app will then be available at `https://benmignard-bit.github.io/BIBLIOTHEQUE/`. On iPhone, you can add it to your home screen from Safari to use it like an app.

### Your data

Books are saved in your browser's local storage, on your device only. Remember to create a backup from the **Exporter** (Export) screen from time to time.

The optional API keys (Google Books, Claude) also stay on your device. A Claude key is only used to generate summaries, and usage is billed to your own API account.

### Online sources

Google Books · Open Library · BnF catalogue · La Bourse aux livres · Wikipedia · [ZXing](https://github.com/zxing-js/library) (barcode reading) and [SheetJS](https://sheetjs.com/) (Excel export).

### Tech

A single HTML file, no build step and nothing to install: HTML, CSS and JavaScript. The scanning and export libraries load on demand from a CDN. The interface is in French.

---

## 🇫🇷 Français

Une application web pour **cataloguer ses livres en scannant leur code-barres**. Elle tient dans un seul fichier (`index.html`), fonctionne sur téléphone comme sur ordinateur, et garde toutes vos données **sur votre appareil** : pas de compte, pas de serveur.

### Ce que fait l'application

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

### Utilisation

1. Ouvrez la page de l'application (voir ci-dessous) dans le navigateur de votre téléphone.
2. Touchez **Scanner** et autorisez la caméra.
3. Visez le code-barres d'un livre : la fiche se remplit toute seule.

> La caméra en direct exige une adresse en **https**. Sur un autre appareil, vous pouvez toujours photographier le code-barres ou saisir l'ISBN.

### Publier avec GitHub Pages

Dans **Settings → Pages**, choisissez la branche `main` et le dossier racine. L'application sera alors accessible à l'adresse `https://benmignard-bit.github.io/BIBLIOTHEQUE/`. Sur iPhone, vous pouvez l'ajouter à l'écran d'accueil depuis Safari pour l'utiliser comme une app.

### Vos données

Les livres sont enregistrés dans le stockage local du navigateur, sur votre appareil uniquement. Pensez à créer une sauvegarde de temps en temps depuis l'écran **Exporter**.

Les clés API facultatives (Google Livres, Claude) restent elles aussi sur l'appareil. Une clé Claude n'est utilisée que pour générer des résumés, et son usage est facturé sur votre compte API.

### Sources en ligne

Google Livres · Open Library · catalogue de la BnF · La Bourse aux livres · Wikipédia · [ZXing](https://github.com/zxing-js/library) (lecture des codes-barres) et [SheetJS](https://sheetjs.com/) (export Excel).

### Technique

Un seul fichier HTML, sans build ni dépendance à installer : HTML, CSS et JavaScript. Les bibliothèques de scan et d'export se chargent à la demande depuis un CDN. L'interface est en français.

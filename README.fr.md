<p align="center">
  <a href="README.md">🇩🇪 Deutsch</a> · <a href="README.en.md">🇬🇧 English</a> · 🇫🇷 Français · <a href="README.es.md">🇪🇸 Español</a>
</p>

<p align="center">
  <img src="screenshots/hero.png" alt="IMG Performer" width="100%">
</p>

<h1 align="center">IMG Performer</h1>

<p align="center">
  <strong>Conversion WebP/AVIF et étiquetage des images IA selon l'EU AI Act pour WordPress – directement sur votre propre serveur.</strong><br>
  Sans cloud, sans compte, sans quota mensuel.
</p>

<p align="center">
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/v/enfants-img-performer?label=WordPress.org&color=2271b1" alt="Version WordPress.org"></a>
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/installs/enfants-img-performer?label=installations%20actives&color=2271b1" alt="Installations actives"></a>
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/tested/enfants-img-performer?label=test%C3%A9%20jusqu%27%C3%A0&color=2271b1" alt="Testé jusqu'à"></a>
  <img src="https://img.shields.io/badge/PHP-7.4%2B-777bb4" alt="PHP 7.4+">
  <img src="https://img.shields.io/badge/Gratuit-WebP%20%2B%20%C3%A9tiquetage%20IA-brightgreen" alt="Version gratuite">
  <img src="https://img.shields.io/badge/RGPD-traitement%20local-blue" alt="RGPD">
</p>

<p align="center">
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><strong>Télécharger</strong></a> ·
  <a href="https://img-performer.enfants.de/fr/">Site web</a> ·
  <a href="https://img-performer.enfants.de/fr/#pricing">Tarifs</a> ·
  <a href="https://wordpress.org/plugins/enfants-img-performer/#developers">Journal des modifications</a> ·
  <a href="https://wordpress.org/support/plugin/enfants-img-performer/">Support</a>
</p>

---

## Pourquoi un autre plugin d'images ?

La plupart des optimiseurs envoient vos fichiers à un service tiers et vous limitent par mois. **IMG Performer convertit en local** avec la bibliothèque PHP GD. Pour la conversion et l'étiquetage des images générées par IA, vos images ne quittent pas votre serveur.

Depuis le **2 août 2026**, l'article 50 du règlement européen sur l'IA (EU AI Act) s'applique. WordPress supprime les informations de provenance intégrées lorsqu'il génère les miniatures. L'étiquetage des images IA nécessite donc une solution dédiée, que le plugin applique dès la mise en ligne.

## Fonctions

### Conversion

- Convertit automatiquement les images JPEG et PNG en **WebP**, sans limite et gratuitement
- Convertit toutes les tailles d'image enregistrées (miniature, moyenne, grande, personnalisées)
- Réécrit les attributs `src`, `srcset`, `href` (lightbox) et lazy-load dans le frontend
- Supprime les fichiers WebP lorsque l'original est supprimé
- Qualité réglable de 1 à 100, journal d'activité pour chaque conversion
- Compteur d'économies de CO₂ optionnel (statistique anonyme uniquement sur opt-in)

### Étiquetage des images IA selon l'EU AI Act (art. 50)

- Détecte la provenance IA des nouvelles images (métadonnées intégrées comme les manifestes C2PA, lorsqu'elles existent)
- Écrit son propre étiquetage, indépendant de l'hébergeur, dans l'original et dans chaque taille générée
- Affiche un **badge « Généré par IA »** visible dans le frontend, désactivable
- Correction de la classification automatique en un clic dans la médiathèque
- Colonnes de statut pour l'étiquetage IA et le texte alternatif, plus un filtre pour les images non vérifiées
- Génère pour les images mises en avant étiquetées une image `og:image` (1200×630) portant l'étiquette

### PRO

- **Conversion AVIF**, en général plus légère que le WebP
- **Convertisseur en masse** pour toute la médiathèque
- **Générateur de textes alternatifs par IA** (WCAG 2.1 AA) avec votre propre clé API : Mistral, Claude, OpenAI ou tout point de terminaison compatible OpenAI, y compris auto-hébergé
- Mention facultative dans le texte alternatif des images classées comme générées par IA

## Captures d'écran

<table>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-2.png" alt="Réglages"><br><sub>Réglages et compteur de CO₂</sub></td>
    <td width="50%"><img src="screenshots/screenshot-4.png" alt="Réglages de l'étiquetage IA"><br><sub>Réglages de l'étiquetage IA</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-6.png" alt="Médiathèque"><br><sub>Médiathèque avec colonnes de statut et filtre</sub></td>
    <td width="50%"><img src="screenshots/screenshot-8.png" alt="Badge dans le frontend"><br><sub>Badge visible dans le frontend</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-9.png" alt="Comparaison de tailles"><br><sub>PNG d'origine 2,1 Mo → WebP 87 Ko → AVIF 110 Ko (PRO)</sub></td>
    <td width="50%"><img src="screenshots/screenshot-10.png" alt="Comparaison de tailles"><br><sub>JPEG 329 Ko → WebP 119 Ko → AVIF 142 Ko (PRO)</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-13.png" alt="Fonctions PRO"><br><sub>PRO : AVIF, traitement en masse et textes alternatifs IA</sub></td>
    <td width="50%"><img src="screenshots/screenshot-17.png" alt="Texte alternatif IA"><br><sub>PRO : texte alternatif, légende et description générés</sub></td>
  </tr>
</table>

## Installation

1. Dans WordPress, ouvrez **Extensions → Ajouter** et recherchez **IMG Performer**, ou [téléchargez-le sur WordPress.org](https://fr.wordpress.org/plugins/enfants-img-performer/).
2. Activez l'extension.
3. Dans **Réglages → IMG Performer**, définissez la qualité.

**Prérequis :** WordPress 6.0+, PHP 7.4+, GD avec prise en charge de WebP (`imagewebp`). L'AVIF (PRO) nécessite PHP 8.1+ avec prise en charge AVIF dans GD, ou Imagick avec AVIF. Sans cela, le WebP est servi.

## Gratuit ou PRO

| | Gratuit | PRO |
|---|:---:|:---:|
| Conversion WebP, sans limite | ✅ | ✅ |
| Étiquetage IA selon l'EU AI Act et badge | ✅ | ✅ |
| `og:image` avec étiquette IA | ✅ | ✅ |
| Conversion AVIF | | ✅ |
| Convertisseur en masse | | ✅ |
| Générateur de textes alternatifs IA (clé API personnelle) | | ✅ |

## Confidentialité (RGPD)

La conversion et l'étiquetage des images IA s'exécutent entièrement sur votre serveur. La version gratuite n'a besoin d'aucune clé API et n'envoie ni données d'image ni données personnelles à des services externes. La seule connexion externe facultative est la statistique de CO₂ sur opt-in. Elle transmet uniquement le total d'octets économisés et un identifiant de site aléatoire et anonyme, sans domaine ni adresse IP.

Le texte alternatif IA de la version PRO fonctionne différemment : l'image est envoyée au fournisseur IA dont vous saisissez la clé API. Un contrat de sous-traitance (DPA) avec ce fournisseur est nécessaire. Nous recommandons Mistral (entreprise européenne, serveurs européens).

## Code source et licence

L'extension gratuite est open source sous **GPL-2.0 ou ultérieure** et distribuée via [WordPress.org](https://fr.wordpress.org/plugins/enfants-img-performer/). Le code source n'est pas publié dans ce dépôt, qui ne contient que le README, des captures d'écran et des liens. PRO est une extension distincte et commerciale.

## Liens et support

- Site web : [img-performer.enfants.de](https://img-performer.enfants.de/fr/)
- Forum de support : [wordpress.org/support/plugin/enfants-img-performer](https://wordpress.org/support/plugin/enfants-img-performer/)
- Développé par [enfants terribles](https://enfants.de), Hambourg

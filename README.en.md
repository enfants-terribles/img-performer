<p align="center">
  <img src="screenshots/hero.png" alt="Enfants IMG Performer" width="100%">
</p>

<h1 align="center">Enfants IMG Performer</h1>

<p align="center">
  <strong>WebP/AVIF conversion and EU AI Act image labeling for WordPress – processed on your own server.</strong><br>
  No cloud, no account, no monthly quota.
</p>

<p align="center">
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/v/enfants-img-performer?label=WordPress.org&color=2271b1" alt="WordPress.org version"></a>
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/installs/enfants-img-performer?label=active%20installs&color=2271b1" alt="Active installs"></a>
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/tested/enfants-img-performer?label=tested%20up%20to&color=2271b1" alt="Tested up to"></a>
  <img src="https://img.shields.io/badge/PHP-7.4%2B-777bb4" alt="PHP 7.4+">
  <img src="https://img.shields.io/badge/Free%20plan-WebP%20%2B%20AI%20labeling-brightgreen" alt="Free plan">
</p>

<p align="center">
  <a href="README.md">🇩🇪 Deutsch</a> · 🇬🇧 English
</p>

<p align="center">
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><strong>Download</strong></a> ·
  <a href="https://img-performer.enfants.de/">Website</a> ·
  <a href="https://img-performer.enfants.de/#pricing">Pricing</a> ·
  <a href="https://wordpress.org/plugins/enfants-img-performer/#developers">Changelog</a> ·
  <a href="https://wordpress.org/support/plugin/enfants-img-performer/">Support</a>
</p>

---

## Why another image plugin?

Many image optimizers upload your files to a third-party service and meter you by month. **Enfants IMG Performer converts locally** with PHP's GD library. Your images never leave your server for conversion or AI-image labeling.

Since **2 August 2026**, Article 50 of the EU AI Act applies. WordPress strips embedded provenance metadata when it generates thumbnails, so labeling AI images needs its own handling. The plugin does that on upload.

## Features

### Conversion

- Converts JPEG and PNG uploads to **WebP** automatically, unlimited and free
- Converts every registered image size (thumbnail, medium, large, custom)
- Rewrites `src`, `srcset`, `href` (lightbox) and lazy-load attributes in the frontend
- Removes the WebP files when the original is deleted
- Quality setting from 1 to 100, activity log for every conversion
- Optional CO₂ savings counter (anonymous statistics are opt-in)

### EU AI Act Art. 50 labeling

- Detects AI provenance in new uploads (embedded metadata such as C2PA manifests, where present)
- Writes its own hosting-independent label into the original and every generated size, no Imagick required
- Shows a visible **"AI-generated" badge** in the frontend, toggleable
- Correct the automatic classification in one click in the Media Library
- "AI Labeling" and alt-text status columns plus a "Needs review" filter
- Generates a 1200×630 `og:image` with the label for AI-labeled featured images

### PRO

- **AVIF conversion**, usually smaller than WebP
- **Bulk converter** for your whole media library
- **AI alt text generator** (WCAG 2.1 AA) with your own API key: Mistral, Claude, OpenAI or any OpenAI-compatible endpoint, including self-hosted
- Optional disclosure note in the alt text of AI-classified images

## Screenshots

<table>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-2.png" alt="Settings"><br><sub>Settings and live CO₂ counter</sub></td>
    <td width="50%"><img src="screenshots/screenshot-4.png" alt="AI labeling settings"><br><sub>AI labeling settings</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-6.png" alt="Media Library"><br><sub>Media Library with "Needs review" filter</sub></td>
    <td width="50%"><img src="screenshots/screenshot-8.png" alt="Frontend badge"><br><sub>Visible badge in the frontend</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-9.png" alt="Size comparison"><br><sub>Original PNG 2.1 MB → WebP 87 KB → AVIF 110 KB (PRO)</sub></td>
    <td width="50%"><img src="screenshots/screenshot-10.png" alt="Size comparison"><br><sub>JPEG 329 KB → WebP 119 KB → AVIF 142 KB (PRO)</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-13.png" alt="PRO features"><br><sub>PRO: AVIF, bulk and AI alt text</sub></td>
    <td width="50%"><img src="screenshots/screenshot-17.png" alt="AI alt text"><br><sub>PRO: generated alt text, caption and description</sub></td>
  </tr>
</table>

## Install

1. In WordPress, go to **Plugins → Add New** and search for **Enfants IMG Performer**, or [download it from WordPress.org](https://wordpress.org/plugins/enfants-img-performer/).
2. Activate the plugin.
3. Open **Settings → IMG Performer** and set the quality.

**Requirements:** WordPress 6.0+, PHP 7.4+, GD with WebP support (`imagewebp`). AVIF (PRO) needs PHP 8.1+ with AVIF support in GD, or Imagick with AVIF. Without it, WebP is delivered.

## Free vs. PRO

| | Free | PRO |
|---|:---:|:---:|
| WebP conversion, unlimited | ✅ | ✅ |
| EU AI Act labeling and badge | ✅ | ✅ |
| `og:image` with AI label | ✅ | ✅ |
| AVIF conversion | | ✅ |
| Bulk converter | | ✅ |
| AI alt text generator (own API key) | | ✅ |

## Privacy

Conversion and AI-image labeling run entirely on your server. The free plugin needs no API key and sends no image data or personal data to external services. The only optional external connection is the opt-in CO₂ statistic, which sends only the total bytes saved and a random, anonymous site ID – no domain, no IP address.

The AI alt text feature in PRO works differently: the image goes to the AI provider whose API key you enter. A data processing agreement with that provider is required. We recommend Mistral (EU company, EU servers).

## Source and license

The free plugin is open source under **GPL-2.0-or-later** and is distributed through [WordPress.org](https://wordpress.org/plugins/enfants-img-performer/). The source is not published in this repository, which only holds the README, screenshots and links. PRO is a separate, commercial plugin.

## Links and support

- Website: [img-performer.enfants.de](https://img-performer.enfants.de/)
- Support forum: [wordpress.org/support/plugin/enfants-img-performer](https://wordpress.org/support/plugin/enfants-img-performer/)
- Made by [enfants terribles](https://enfants.de), Hamburg

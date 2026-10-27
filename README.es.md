<p align="center">
  <a href="README.md">🇩🇪 Deutsch</a> · <a href="README.en.md">🇬🇧 English</a> · <a href="README.fr.md">🇫🇷 Français</a> · 🇪🇸 Español
</p>

<p align="center">
  <img src="screenshots/hero.png" alt="IMG Performer" width="100%">
</p>

<h1 align="center">IMG Performer</h1>

<p align="center">
  <strong>Conversión a WebP/AVIF y etiquetado de imágenes de IA según el EU AI Act para WordPress, directamente en tu propio servidor.</strong><br>
  Sin nube, sin cuenta, sin cuota mensual.
</p>

<p align="center">
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/v/enfants-img-performer?label=WordPress.org&color=2271b1" alt="Versión en WordPress.org"></a>
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/installs/enfants-img-performer?label=instalaciones%20activas&color=2271b1" alt="Instalaciones activas"></a>
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><img src="https://img.shields.io/wordpress/plugin/tested/enfants-img-performer?label=probado%20hasta&color=2271b1" alt="Probado hasta"></a>
  <img src="https://img.shields.io/badge/PHP-7.4%2B-777bb4" alt="PHP 7.4+">
  <img src="https://img.shields.io/badge/Gratis-WebP%20%2B%20etiquetado%20IA-brightgreen" alt="Versión gratuita">
  <img src="https://img.shields.io/badge/RGPD-procesamiento%20local-blue" alt="RGPD">
</p>

<p align="center">
  <a href="https://wordpress.org/plugins/enfants-img-performer/"><strong>Descargar</strong></a> ·
  <a href="https://img-performer.enfants.de/es/">Sitio web</a> ·
  <a href="https://img-performer.enfants.de/es/#pricing">Precios</a> ·
  <a href="https://wordpress.org/plugins/enfants-img-performer/#developers">Registro de cambios</a> ·
  <a href="https://wordpress.org/support/plugin/enfants-img-performer/">Soporte</a>
</p>

---

## ¿Por qué otro plugin de imágenes?

La mayoría de los optimizadores envían tus archivos a un servicio de terceros y te limitan por mes. **IMG Performer convierte en local** con la biblioteca PHP GD. Para la conversión y el etiquetado de imágenes generadas por IA, tus imágenes no salen de tu servidor.

Desde el **2 de agosto de 2026** se aplica el artículo 50 del Reglamento de IA de la UE (EU AI Act). WordPress elimina la información de procedencia incrustada al generar las miniaturas, así que etiquetar imágenes de IA requiere una solución propia. El plugin la aplica al subir la imagen.

## Funciones

### Conversión

- Convierte automáticamente las imágenes JPEG y PNG a **WebP**, sin límite y gratis
- Convierte todos los tamaños de imagen registrados (miniatura, mediano, grande, personalizados)
- Reescribe los atributos `src`, `srcset`, `href` (lightbox) y de carga diferida en el frontend
- Elimina los archivos WebP cuando se elimina el original
- Calidad ajustable de 1 a 100, registro de actividad de cada conversión
- Contador opcional de ahorro de CO₂ (estadística anónima solo con opt-in)

### Etiquetado de imágenes de IA según el EU AI Act (art. 50)

- Detecta la procedencia de IA en las imágenes nuevas (metadatos incrustados como los manifiestos C2PA, cuando existen)
- Escribe su propio etiquetado, independiente del hosting, en el original y en cada tamaño generado
- Muestra una **insignia «Generado por IA»** visible en el frontend, desactivable
- Corrección de la clasificación automática con un clic en la biblioteca de medios
- Columnas de estado para el etiquetado de IA y el texto alternativo, más un filtro para imágenes sin revisar
- Genera para las imágenes destacadas etiquetadas un `og:image` (1200×630) con la etiqueta

### PRO

- **Conversión a AVIF**, normalmente más ligera que WebP
- **Convertidor masivo** para toda la biblioteca de medios
- **Generador de textos alternativos con IA** (WCAG 2.1 AA) con tu propia clave API: Mistral, Claude, OpenAI o cualquier endpoint compatible con OpenAI, también autoalojado
- Nota opcional en el texto alternativo de las imágenes clasificadas como generadas por IA

## Capturas de pantalla

<table>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-2.png" alt="Ajustes"><br><sub>Ajustes y contador de CO₂</sub></td>
    <td width="50%"><img src="screenshots/screenshot-4.png" alt="Ajustes del etiquetado de IA"><br><sub>Ajustes del etiquetado de IA</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-6.png" alt="Biblioteca de medios"><br><sub>Biblioteca de medios con columnas de estado y filtro</sub></td>
    <td width="50%"><img src="screenshots/screenshot-8.png" alt="Insignia en el frontend"><br><sub>Insignia visible en el frontend</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-9.png" alt="Comparación de tamaños"><br><sub>PNG original 2,1 MB → WebP 87 KB → AVIF 110 KB (PRO)</sub></td>
    <td width="50%"><img src="screenshots/screenshot-10.png" alt="Comparación de tamaños"><br><sub>JPEG 329 KB → WebP 119 KB → AVIF 142 KB (PRO)</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="screenshots/screenshot-13.png" alt="Funciones PRO"><br><sub>PRO: AVIF, procesamiento masivo y textos alternativos con IA</sub></td>
    <td width="50%"><img src="screenshots/screenshot-17.png" alt="Texto alternativo con IA"><br><sub>PRO: texto alternativo, leyenda y descripción generados</sub></td>
  </tr>
</table>

## Instalación

1. En WordPress, ve a **Plugins → Añadir nuevo** y busca **IMG Performer**, o [descárgalo en WordPress.org](https://es.wordpress.org/plugins/enfants-img-performer/).
2. Activa el plugin.
3. En **Ajustes → IMG Performer**, define la calidad.

**Requisitos:** WordPress 6.0+, PHP 7.4+, GD con compatibilidad con WebP (`imagewebp`). AVIF (PRO) requiere PHP 8.1+ con soporte AVIF en GD, o Imagick con AVIF. Sin ello, se sirve WebP.

## Gratis o PRO

| | Gratis | PRO |
|---|:---:|:---:|
| Conversión a WebP, sin límite | ✅ | ✅ |
| Etiquetado de IA según el EU AI Act e insignia | ✅ | ✅ |
| `og:image` con etiqueta de IA | ✅ | ✅ |
| Conversión a AVIF | | ✅ |
| Convertidor masivo | | ✅ |
| Generador de textos alternativos con IA (clave API propia) | | ✅ |

## Privacidad (RGPD)

La conversión y el etiquetado de imágenes de IA se ejecutan por completo en tu servidor. La versión gratuita no necesita clave API y no envía datos de imagen ni datos personales a servicios externos. La única conexión externa opcional es la estadística de CO₂ con opt-in. Solo transmite el total de bytes ahorrados y un identificador de sitio aleatorio y anónimo, sin dominio ni dirección IP.

El texto alternativo con IA de PRO funciona de otra forma: la imagen se envía al proveedor de IA cuya clave API introduces. Necesitas un contrato de encargado del tratamiento (DPA) con ese proveedor. Recomendamos Mistral (empresa europea, servidores en la UE).

## Código fuente y licencia

El plugin gratuito es de código abierto bajo **GPL-2.0 o posterior** y se distribuye a través de [WordPress.org](https://es.wordpress.org/plugins/enfants-img-performer/). El código fuente no se publica en este repositorio, que solo contiene el README, capturas de pantalla y enlaces. PRO es un plugin independiente y comercial.

## Enlaces y soporte

- Sitio web: [img-performer.enfants.de](https://img-performer.enfants.de/es/)
- Foro de soporte: [wordpress.org/support/plugin/enfants-img-performer](https://wordpress.org/support/plugin/enfants-img-performer/)
- Desarrollado por [enfants terribles](https://enfants.de), Hamburgo

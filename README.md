 Motor de guion & prompt para video IA

App web para pasar de un **brief** a un **guion escena por escena** y a un **prompt optimizado**
listo para pegar en tu motor de video IA (Sora, Veo 3, Runway, Kling, Pika, Luma, Hailuo, Oreate).

- Videos de **30 s a 5 min**.
- Formatos **IG** (Reels 9:16, Feed 1:1 / 4:5) y **LinkedIn** (16:9, 1:1).
- Tema **oscuro y minimalista**, con la identidad de ALTO MONTE.
- Funciona **100% en el navegador**: sin cuentas, sin servidor, sin claves API.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | La aplicación completa (todo el CSS y JS va incluido). |
| `PROMPT-MAESTRO-ALTOMONTE.md` | El prompt de marca reutilizable, editable a mano. |
| `README.md` | Este archivo. |

## Usarla en local

Abre `index.html` con doble clic en cualquier navegador. Eso es todo.

## Desplegar (elige una)

Como es un sitio estático, se publica sin configuración:

**Netlify (arrastrar y soltar):**
1. Entra a https://app.netlify.com/drop
2. Arrastra la carpeta con `index.html`. Listo, te da una URL pública.

**Vercel:**
1. Sube estos archivos a un repositorio de GitHub.
2. En https://vercel.com → *Add New Project* → importa el repo → *Deploy*.
   No hace falta framework ni build; detecta el sitio estático.

**GitHub Pages:**
1. Sube los archivos a un repo.
2. *Settings → Pages → Deploy from branch* → `main` / `root`.

## Cómo se usa

1. Escribe el **concepto** del video.
2. Ajusta **tipo, duración, formato, motor, estilo e idioma**.
3. Activa/desactiva **locución, música y texto en pantalla**.
4. Pulsa **Generar**. Obtienes dos pestañas:
   - **Guion por escenas:** desglose con encuadre, cámara, luz, locución y texto.
   - **Prompt IA:** el prompt formateado para el motor elegido, con nota de consistencia.
5. **Copia o descarga** cada uno y pégalo en tu motor de video.

## Notas

- El prompt se genera en **inglés** porque Sora, Veo, Runway y Kling rinden mejor así;
  el guion y la locución respetan el idioma que elijas.
- Cambia el **motor** para reformatear el prompt (cada uno usa una estructura distinta).
- Para publicar en varios formatos, genera de nuevo cambiando el **formato**.
- La paleta, la marca y el tagline son editables desde el propio panel.

# ALTO MONTE · Sistema de video corporativo con IA

Del brief al video, todo con material generado por IA.

```
App (brief) → guion.json → subir en la app → 3 preguntas → generación
                                                    ↓
                                        manifiesto → Colab → MP4 final
```

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | La app. Blanco y negro, lista para desplegar. |
| `proxy-worker.js` | Proxy para que el navegador pueda llamar la API de video. |
| `render_video_altomonte.ipynb` | Ensamblado final en Colab: escenas + voz + música → MP4. |
| `PROMPT-MAESTRO-ALTOMONTE.md` | Prompt de marca reutilizable. |

## La app

**Pestaña Guion.** Escribe el concepto y genera el desglose escena por escena.
El prompt **no se muestra en pantalla**: queda en un panel colapsable bajo «Revisar»,
con dos descargas — el prompt en texto y el archivo `.json` que alimenta la generación.

**Pestaña Generar.** Arrastra el `.json`. Al soltarlo aparecen **tres preguntas** y,
al confirmar, la generación arranca sola:

1. **¿Qué generamos?** Imágenes con movimiento (sin costo) · Video en escenas clave · Video en todas
2. **¿Cuántas escenas?** Solo las tres primeras (prueba) · Todas
3. **¿Consistencia visual?** Semilla fija · Semilla variada

Las tres preguntas existen para que una corrida completa nunca se dispare por accidente:
28 escenas en video real cuestan dinero, tres imágenes de prueba no cuestan nada.

## Diseño

Negro puro, tipografía del sistema, retículas de una sola línea y mucho aire.
El **verde aparece solo en estados** — la barra de progreso y los interruptores activos —
nunca como decoración. Así el color significa «esto está pasando» en vez de ser un adorno,
y el blanco y negro se mantiene limpio.

## Conexión con la API de terceros

Las imágenes se generan sin clave. Para clips de video, en **Ajustes de conexión** defines:

- **Endpoint** y **clave** de tu proveedor
- **Encabezado** y **prefijo** (por defecto `Authorization` / `Bearer `)
- **Cuerpo de la petición**, con `{{prompt}}`, `{{aspect}}` y `{{seconds}}`

La respuesta se explora sola buscando la dirección del clip. Si el proveedor devuelve
un trabajo pendiente, la app consulta hasta que esté listo. La clave vive solo en la
pestaña abierta: no se guarda en ningún lado.

### El proxy no es opcional en la práctica

Casi todos los proveedores rechazan las peticiones hechas desde un navegador (CORS).
Si ves ese error, despliega `proxy-worker.js`:

1. dash.cloudflare.com → Workers & Pages → Create → Worker
2. Pega el archivo y publica
3. En la app, campo Proxy: `https://tu-worker.workers.dev/?url=`

El proxy solo reenvía a los dominios de su lista `ALLOW`. Agrega el de tu proveedor
y cambia `ORIGIN` por tu dominio cuando publiques.

## Por qué el ensamblado final sigue en Colab

El navegador genera bien las escenas una por una, pero unir 28 clips con locución y
música es mucho más estable en el notebook, que ya está probado y produce el MP4
con voz femenina colombiana y música original.

## Desplegar

Sitio estático, sin build:

- **Netlify:** arrastra la carpeta a https://app.netlify.com/drop
- **Vercel:** sube a GitHub → Add New Project → importa → Deploy
- **GitHub Pages:** Settings → Pages → Deploy from branch → `main` / `root`

## Pendiente

Cuando tengas el logo en PNG y la tipografía de ALTO MONTE, se reemplazan la fuente
del notebook y el cierre del video con la marca real.

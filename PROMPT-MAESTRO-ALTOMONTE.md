# PROMPT MAESTRO — ALTO MONTE

Bloque de marca reutilizable. Pégalo como contexto/estilo en cualquier motor de video IA
(Sora, Veo 3, Runway, Kling, Pika, Luma, Hailuo, Oreate) y luego añade tu escena.
La app genera esto automáticamente, pero aquí lo tienes editable a mano.

---

## 1. Identidad

- **Marca:** ALTO MONTE
- **Sector:** Energía renovable / limpia
- **Tagline:** «Energía que nace de las alturas.»
- **Llamado a la acción:** «Hagámoslo posible.»
- **Personalidad:** confiable, moderna, sobria, con raíz en la naturaleza y la montaña.
- **Idea central:** la energía baja desde las alturas (montaña, agua, viento, sol) hasta las personas.

## 2. Sistema visual

- **Paleta:** verde energía `#3FE0A0` + ámbar amanecer `#F4B44C` sobre base oscura `#080B0A`.
- **Color grade:** alto contraste, sombras profundas, luz volumétrica, destellos dorados sobre terreno de montaña.
- **Motivos recurrentes:** cordilleras al amanecer, aerogeneradores, paneles solares, represas
  hidroeléctricas, torres de alta tensión, salas de control modernas, comunidades iluminadas al anochecer,
  líneas de contorno topográfico como recurso gráfico.
- **Cámara:** movimientos elegantes y con propósito (dolly-in lento, grúa ascendente, órbita suave, drone push-in).
- **Acabado:** 4K, profundidad de campo reducida, look comercial de cine.

## 3. Tono narrativo

Épico pero cálido. La montaña como origen de una fuerza limpia que llega a la gente.
Evitar: estética sucia/industrial contaminante, sobresaturación, tipografías de relleno, clichés genéricos.

## 4. Bloque de estilo (copiar/pegar en inglés — mejor rendimiento)

```
Cinematic commercial film for ALTO MONTE, a renewable energy company.
Brand color grade of energy green #3FE0A0 and sunrise amber #F4B44C, deep contrast,
volumetric light, golden-hour highlights on mountain terrain, shallow depth of field,
4K, filmic, professional. Aspect ratio [9:16 / 1:1 / 16:9].
```

## 5. Plantilla por escena

```
Scene [n] ([segundos]s): [movimiento de cámara] — [descripción visual del motivo energético].
Lighting: [luz]. [BLOQUE DE ESTILO].
Audio: [música cinematográfica sutil]; voiceover: "[línea]".
```

## 6. Arco recomendado para un lanzamiento

1. **Apertura** — gancho visual que detiene el scroll (amanecer sobre la cumbre).
2. **Contexto** — por qué importa la energía limpia.
3. **Revelación de marca** — aparece ALTO MONTE como respuesta.
4. **Diferencial** — qué la hace única (renovable, inteligente, en tiempo real).
5. **Demostración** — la energía en acción, de la montaña al hogar.
6. **Impacto** — beneficio para las comunidades.
7. **Cierre / CTA** — logo sobre plano aéreo de la cordillera + «Hagámoslo posible.»

Para 3 minutos el arco se amplía a 11 beats distintos (apertura, contexto, problema, origen,
marca, valores, cultura, diferencial, demostración, impacto, cierre) para que ninguna línea
de locución se repita. Algunas escenas quedan sin narración a propósito: son respiros de música.

## 6b. Locución

Voz femenina con acento colombiano. En Veo, indícalo dentro del prompt de audio:
`voiceover (Colombian Spanish, female): "..."`. En el notebook se usa `es-CO-SalomeNeural`.

## 7. Negative prompt (para Kling / Pika / Hailuo / Luma)

```
no on-screen text artifacts, no distorted faces, no warped logos, no extra limbs,
no watermark, no oversaturation, no flicker, no low resolution
```

## 8. Consistencia entre clips

- Repite el **bloque de estilo** en cada generación.
- Fija un **seed** constante.
- Si el motor lo permite, sube un **frame de referencia** del primer clip.
- Genera **clip por clip** y móntalos en secuencia en tu editor.

## 9. Motor recomendado

**Veo 3.1** es el primario: genera audio nativo sincronizado, lo que ahorra un paso completo
de post-producción en video corporativo. Luma y Runway son alternos válidos.

**Sora quedó fuera del sistema:** OpenAI discontinuó sus apps el 26 de abril de 2026 y la API
cierra el 24 de septiembre de 2026.

# ONCORED - Red de Cuidado Oncológico - COL (Animación de Logo 3D)

Animación vectorial interactiva del logotipo **ONCORED - Red de Cuidado Oncológico - COL**, construida en un único archivo `index.html` con HTML5, CSS3 3D, SVG y síntesis de audio sutil con Web Audio API.

## Características
- **Animación de atrás hacia adelante (3D):** El círculo central y los cuatro cuadrantes emergen desde profundidad en el eje Z y encajan secuencialmente.
- **Íconos internos protagonistas:** Cada ícono interno entra por separado en tamaño grande en primer plano y se adapta con suavidad a su posición y escala final.
- **Cierre tipográfico:** Entrada secuencial de **«ONCORED»** y **«Red de Cuidado Oncológico - COL»**, seguida de una flotación suave continua.
- **Audio sutil integrado (Web Audio API):** Efectos suaves y armónicos sin archivos externos, con botón de **Sonido ON/OFF**, **Repetir**, selector de fondo (**Blanco**, **Chroma Verde**, **Oscuro**) y opción para ocultar controles.

## Publicación en GitHub Pages
1. Sube `index.html` (y opcionalmente la imagen de referencia del logo) a la rama `main` del repositorio.
2. Ve a **Settings → Pages**.
3. En **Branch**, selecciona **`main`** y haz clic en **Save**.
4. Espera 1–2 minutos para acceder al enlace público generado por GitHub Pages.

## Prompt maestro utilizado

> **ROLE:** Eres un desarrollador experto en Frontend, diseño vectorial SVG, animaciones 3D con CSS/GSAP y síntesis de audio sutil con Web Audio API en HTML5 puro.
>
> **TASK:** Crea un único archivo `index.html` autónomo, limpio y sin dependencias externas obligatorias, que recree en SVG vectorial y anime pieza por pieza el logotipo **ONCORED - Red de Cuidado Oncológico - COL** (basado en la imagen adjunta), incluyendo efectos de sonido sutiles generados por código al entrar cada pieza y encajar cada ícono.
>
> **CONTEXT:** El proyecto se alojará gratis en GitHub Pages y también se utilizará para grabaciones/presentaciones del logotipo. Cada elemento debe tener su propio grupo (`<g>`) con `id` independiente, respetando la paleta de colores y distribución original:
> - `#base-sup-izq`: Cuadrante superior izquierdo `#0B4D4B` con borde gris `#9E9E9E`.
> - `#base-sup-der`: Cuadrante superior derecho `#3B8580` con borde gris `#9E9E9E`.
> - `#base-inf-der`: Cuadrante inferior derecho `#07605C` con borde gris `#9E9E9E`.
> - `#base-inf-izq`: Cuadrante inferior izquierdo `#5EBAB3` con borde gris `#9E9E9E`.
> - `#base-centro`: Círculo central con anillo gris `#9E9E9E`, borde blanco y relleno `#92DBD2`.
> - `#icono-centro`: Símbolo blanco estilizado de cangrejo en el centro.
> - `#icono-sup-izq`: Símbolo blanco lineal de psicología/flor en el cuadrante superior izquierdo.
> - `#icono-sup-der`: Símbolo blanco de nutrición (brote con hojas y espiral) en el cuadrante superior derecho.
> - `#icono-inf-der`: Símbolo blanco de lámpara de enfermería en el cuadrante inferior derecho.
> - `#icono-inf-izq`: Símbolo blanco de estetoscopio con hojas en el cuadrante inferior izquierdo.
> - `#texto-oncored`: Texto principal `"ONCORED"` en color `#0B4D4B`.
> - `#texto-subtitulo`: Texto secundario `"Red de Cuidado Oncológico - COL"` en color gris `#6E7373`.
>
> **REASONING & CHOREOGRAPHY:**
> 1. **Escenario 3D:** Usa `perspective: 1400px` y `transform-style: preserve-3d` para que las piezas viajen en profundidad (eje Z) desde atrás hacia adelante.
> 2. **Fase 1 — Bases y cuadrantes (de atrás hacia adelante):** Cada pieza base arranca desde el fondo (`translateZ` negativo, escala pequeña `0.2`–`0.25`, opacidad `0` y desenfoque suave) y sale volando hacia adelante con ligera inclinación 3D (`rotateX`/`rotateY`) hasta encajar con un rebote sutil.
> 3. **Fase 2 — Íconos internos protagonistas (grandes y luego adaptados):** Cada ícono interno entra por separado después de su base, aparece en primer plano con tamaño grande (`scale` ~`2.3`–`2.5` y sombra/brillo suave) y luego se reduce suavemente hasta adaptarse a su tamaño y posición exactos dentro del logo.
> 4. **Fase 3 — Textos:** Entra `"ONCORED"` desde el fondo y luego `"Red de Cuidado Oncológico - COL"` asentándose debajo.
> 5. **Sonido sutil (Web Audio API):** Implementa un sintetizador suave y discreto (ganancia baja, ondas sinusoidales/triangulares cortas con *fade-out* limpio, sin estridencias) que reproduzca:
>    - Un *whoosh* o pulso grave muy suave cuando salen las piezas base y los textos.
>    - Un toque armónico cristalino y sutil cuando cada ícono grande se adapta y encaja en su lugar.
>    - Incluye un botón de **Sonido ON/OFF** en el panel de controles (respetando las políticas del navegador al pulsar "Repetir" o activar audio).
>
> **OUTPUT FORMAT:** Entrega el código completo de `index.html` listo para guardar y ejecutar, junto con un panel discreto de controles (Repetir, Sonido ON/OFF, selector de fondo Blanco / Chroma Verde / Oscuro y botón Ocultar controles).
>
> **CONDITIONS:**
> - No uses archivos de audio MP3/WAV externos que puedan fallar al cargar; usa Web Audio API integrada.
> - Mantén los colores originales del logo intactos y los bordes limpios.
> - Si el usuario no especifica cambios adicionales, entrega una solución funcional y bien comentada en una sola pieza de código.

---
name: Uva
description: Muestrario cálido de diseños de uñas, con fotografía protagonista y controles sólidos.
colors:
  coral: "#E2725B"
  lilac: "#9B8BD4"
  soft: "#E4DDF3"
  closing: "#F1B5A5"
  bg: "#FAF4EC"
  ink: "#2C2128"
  paper: "#FFFFFF"
typography:
  display:
    fontFamily: "Fraunces, serif"
    fontSize: "78px"
    fontWeight: 500
    lineHeight: 1.04
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "Fraunces, serif"
    fontSize: "50px"
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: "-0.03em"
  title:
    fontFamily: "Fraunces, serif"
    fontSize: "27px"
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: "-0.03em"
  body:
    fontFamily: "Manrope, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.65
  action:
    fontFamily: "Manrope, sans-serif"
    fontSize: "14px"
    fontWeight: 700
    lineHeight: 1.45
  price:
    fontFamily: "Manrope, sans-serif"
    fontSize: "26px"
    fontWeight: 500
    lineHeight: 1.25
rounded:
  card: "16px"
  photo: "12px"
  pill: "999px"
spacing:
  inset: "40px"
  inset-mobile: "22px"
  gallery-gap: "24px"
  section: "96px"
  section-mobile: "68px"
components:
  button-primary:
    backgroundColor: "{colors.coral}"
    textColor: "{colors.ink}"
    typography: "{typography.action}"
    rounded: "{rounded.pill}"
    padding: "14px 23px"
    height: "52px"
  button-primary-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bg}"
  button-secondary:
    backgroundColor: "{colors.soft}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "14px 23px"
  button-secondary-hover:
    backgroundColor: "{colors.lilac}"
  filter:
    backgroundColor: "{colors.soft}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "11px 19px"
    height: "44px"
  filter-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bg}"
  service-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "30px"
---

# Design System: Uva

## Overview

**Creative North Star: "Muestrario de diseños"**

Un mundo cálido y directo: fotografías grandes de manos, titulares con oficio e
itálicas puntuales, y controles sólidos que se leen con facilidad. El color
acompaña la fotografía; los bloques suaves organizan la lectura sin añadir
ornamentos.

Este documento concilia el sistema creado antes del código con los valores
observados en `index.html` y las capturas finales de escritorio y móvil. Los
tokens del frontmatter son normativos; el sidecar amplía estados, movimiento y
ejemplos sin sustituirlos.

**Key Characteristics:**

- Fotografía de manos como material principal.
- Serif expresiva y lectura sans serif tranquila.
- Contraste tinta sobre fondos cálidos.
- Píldoras de acción y superficies de poca profundidad.

## Colors

La paleta combina crema y tinta con coral de acción y lila de apoyo.

### Primary

- **Coral cálido** (`coral`): botones principales y acceso flotante, siempre con texto tinta.
- **Coral suave** (`closing`): superficie amplia de cierre.

### Secondary

- **Lila** (`lilac`): respuesta de filtros y acciones secundarias al hover.
- **Lila suave** (`soft`): fondo de servicios y controles secundarios.

### Neutral

- **Crema** (`bg`): lienzo principal y texto sobre tinta.
- **Tinta ciruela** (`ink`): lectura, selección, foco y footer.
- **Papel blanco** (`paper`): fichas de servicios sobre lila suave.

**The Ink Contrast Rule.** El botón coral lleva texto tinta; su hover invierte
a fondo tinta y texto crema.

## Typography

**Display Font:** Fraunces, con fallback serif.
**Body Font:** Manrope, con fallback sans serif.

Fraunces aporta curvas e itálicas deliberadas. Manrope mantiene la información
práctica compacta y legible, sin convertirla en rotulación de mayúsculas espaciadas.

### Hierarchy

- **Display:** H1 pasa de su token de escritorio a (65px) hasta (1100px), (55px) hasta (900px) y (52px) hasta (600px); conserva dos líneas y una itálica.
- **Headline:** H2 usa el token general; en móvil baja a (36px / 1.16). El cierre tiene su ajuste propio (54px / 38px).
- **Title:** el token es la base. Servicios usan (29px), luego (27px); las tarjetas de galería y los pasos ajustan entre (25–27px) según ancho.
- **Body:** el token de lectura limita párrafos a (65ch); la introducción usa (17px) en escritorio. Notas y metadatos usan (13–14px).
- **Action:** el token de botón baja a (13px) en móvil. Los filtros usan peso (600).
- **Price:** cifras tabulares; el precio baja a (25px) en móvil.
- **Marca:** Fraunces 600 itálica (44px / 42px) en header; (54px / 56px) en footer.

**The Two Voices Rule.** Usar Fraunces para títulos y marca, y Manrope para
lectura, precios y controles. Mantener las itálicas como énfasis puntual.

## Layout

El marco centra el contenido con un máximo de (1220px). Las entradas laterales
del token de escritorio pasan por (28px) hasta (900px) y toman el token móvil
hasta (600px). El header mide (80px / 76px); las anclas dejan (104px) de respiro.

La apertura combina texto y fotografía con columnas casi iguales. Hasta (600px)
se apila y conserva la acción antes de la foto. Las secciones usan el ritmo del
frontmatter, con excepciones propias de apertura, FAQ y cierre.

La galería es un estante de desplazamiento horizontal nativo, con imágenes
(4:5), tres tarjetas visibles en escritorio, dos hasta (900px) y una más un
anticipo hasta (600px). El espacio entre fotos pasa a (20px) en móvil. Los cinco
filtros se envuelven completos; el desplazamiento pertenece al estante, no a la página.

Los servicios forman dos columnas y pasan a una en móvil: cuatro fichas, retiro
en una fila aparte y extras en texto. Proceso y FAQ comparten una columna de
introducción y otra de contenido, que se apilan hasta (900px). El proceso lleva
cuatro pasos; la FAQ, seis disclosures. El footer usa tres, dos y una columna
según ancho y reserva espacio inferior (6rem) para el acceso flotante.

## Elevation & Depth

Sin sombras decorativas. La profundidad aparece por cambios de superficie,
fotografía recortada y espacio. El header conserva el fondo crema, y el acceso
flotante se separa con un borde crema (3px).

Las respuestas habituales duran (0.2s). La entrada coordinada del hero mueve
levemente texto y acción y escala la foto; no gobierna la lectura ni la galería.
Con movimiento reducido se desactivan transiciones y la entrada. Sin JavaScript,
el contenido permanece visible.

## Shapes

Píldoras completas para acciones y filtros; esquinas suaves para fichas y fotos.
La fotografía principal usa un recorte propio (20px), las imágenes del estante
usan el token `photo` y las fichas el token `card`. Flechas y acceso flotante
son círculos. No añadir marcos o sombras a las tarjetas de galería.

## Components

### Buttons

Acciones sólidas, con una sola línea, icono y texto centrados. Los tokens de
componente describen tamaño y color; en móvil el mínimo baja a (49px) y el
padding a (14px 20px). Hover eleva levemente (-2px), active regresa a su posición.
El secundario usa lila suave; en el cierre usa crema. El foco es tinta (3px),
separado (5px).

WhatsApp usa el SVG relleno estándar de Bootstrap Icons, `currentColor` y sin
stroke: (20 × 20px) en botones y (27 × 27px), con base flex (27px), en el flotante.
La licencia MIT se conserva en `THIRD-PARTY-LICENSES.txt`.

### Navigation

Marca itálica y cuatro anclas en Manrope (14px / 600), con subrayado al hover.
Hasta (900px) se abre mediante botón de (44px); informa su estado, cierra con
Escape y devuelve el foco. Sin JavaScript, las anclas siguen visibles.

### Chips

Filtros de (44px) de altura mínima y bordes de píldora. La selección usa tinta
con texto crema y `aria-pressed`; hover usa lila. Los cinco controles se
envuelven y un estado vivo informa cuántos diseños quedan.

### Cards / Containers

Las fichas blancas llevan el token `service-card`; el padding baja a (26px).
Título, explicación y precio mantienen una jerarquía clara, con duración al lado
o debajo según el ancho. La galería usa foto, nombre y técnica sin caja añadida.
Muestra cinco diseños y ofrece flechas, teclado y gesto táctil, sin avance automático.

### Steps

Numeración serif de dos dígitos (38px / 32px), título y explicación. En móvil
los números quedan a la izquierda y los cuatro pasos forman una columna.

### Disclosures

FAQ nativa con `details/summary`, texto de pregunta (16px / 600) y un signo más
SVG fino que gira al abrir. El contenido se revela bajo la pregunta, sin modal
ni iconos de texto.

## Do's and Don'ts

### Do:

- **Do** usar tinta para que los botones coral conserven contraste.
- **Do** mantener visibles los cinco filtros envueltos y el desplazamiento manual de la galería.
- **Do** conservar el foco visible, la lectura sin JavaScript y la alternativa de movimiento reducido.
- **Do** usar fotografías ilustrativas de manos con procedencia registrada.

### Don't:

- **Don't** añadir sombras decorativas o marcos a las fotos del estante.
- **Don't** sustituir los SVG por emojis, glifos tipográficos o paquetes de iconos en tiempo de ejecución.
- **Don't** trasladar el rótulo contextual del hero a nuevas superficies como patrón del sistema.

## Fotografías y procedencia

Fotografías ilustrativas de [Pexels](https://www.pexels.com/license/), guardadas
como WebP locales en `assets/`. No son imágenes propias de Uva ni evidencia de
trabajos de un negocio real. Se descargaron las seis fuentes de la tabla; no
hubo sustituciones por fallos. Se descartaron 6852174 por una marca en ropa y
34121866 por un rostro.

| Archivo | Uso | Fuente |
|---|---|---|
| hero-coral.webp | Hero, manos coral | Lazar Gugleta — https://www.pexels.com/photo/hands-of-a-woman-with-orange-nail-polish-11393877/ |
| diseno-francesita.webp | Francesitas | Roman Titov — https://www.pexels.com/photo/hand-with-french-tip-nails-13038494/ |
| diseno-ondas.webp | Nail art de color | cottonbro studio — https://www.pexels.com/photo/close-up-shot-of-hands-with-colorful-nail-polish-5871824/ |
| diseno-mono.webp | Nail art rosa con aplique | Salim Da — https://www.pexels.com/photo/close-up-of-elegant-manicured-nails-with-floral-design-34885842/ |
| diseno-rojo.webp | Lisos y tonos | Oleskandra Biliak — https://www.pexels.com/photo/close-up-of-a-hand-of-a-woman-with-red-nails-17389258/ |
| diseno-dorado.webp | Efectos, detalles dorados | Анастасія — https://www.pexels.com/photo/elegant-nail-art-with-gold-details-in-natural-light-31744665/ |

## Contenido de muestra

Marca, personas, precios, horarios y contacto son ficticios. Las sesiones de
60/90/120/75/30 minutos y la seña del 30% son datos de muestra del brief, no
operación de una empresa real. La duración orientativa de 2–3 semanas no promete
el mismo resultado a todas las personas. La página tiene tres accesos WhatsApp
placeholder, sin formulario ni pagos conectados. Estas muestras no son tokens
ni reglas visuales reutilizables.

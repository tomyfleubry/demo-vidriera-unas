---
name: Uva
description: Catálogo alegre de diseños y carta de precios sumable
colors:
  bg: "#FAF4EC"
  ink: "#2C2128"
  coral: "#E2725B"
  lilac: "#9B8BD4"
  soft: "#E4DDF3"
typography:
  display:
    fontFamily: "Young Serif, serif"
    fontSize: "72px"
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: "-.03em"
  headline:
    fontFamily: "Young Serif, serif"
    fontSize: "48px"
    fontWeight: 400
    lineHeight: 1.16
    letterSpacing: "-.025em"
  title:
    fontFamily: "Young Serif, serif"
    fontSize: "25px"
    fontWeight: 400
    lineHeight: 1.16
    letterSpacing: "-.025em"
  body:
    fontFamily: "Manrope, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.65
  action:
    fontFamily: "Manrope, sans-serif"
    fontSize: "15px"
    fontWeight: 700
    lineHeight: 1.45
  label:
    fontFamily: "Manrope, sans-serif"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: 1.45
  price:
    fontFamily: "Manrope, sans-serif"
    fontSize: "24px"
    fontWeight: 600
    lineHeight: 1.25
rounded:
  field: "6px"
  gallery: "12px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter: "40px"
  gutter-tablet: "28px"
  gutter-mobile: "22px"
  section: "96px"
  section-mobile: "68px"
  price-row: "14px"
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
    typography: "{typography.action}"
    rounded: "{rounded.pill}"
    padding: "14px 23px"
    height: "52px"
  button-secondary-hover:
    backgroundColor: "{colors.lilac}"
    textColor: "{colors.ink}"
  button-work:
    backgroundColor: "{colors.coral}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "13px 20px"
    height: "48px"
  filter:
    backgroundColor: "{colors.soft}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "11px 19px"
    height: "44px"
  filter-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.bg}"
  quantity-input:
    backgroundColor: "{colors.bg}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "8px 10px"
    width: "76px"
    height: "44px"
---

# Design System: Uva

Dirección elegida íntegramente por Tomas y documentada ANTES de modificar el
HTML. Esta versión concilia esa decisión previa con el sistema implementado;
no presenta la identidad como una elección posterior al código. La copia previa
se conserva en la evidencia privada `uva-catalogo/DESIGN-primero.md`. Los tokens
del frontmatter son normativos; el sidecar amplía estados y ejemplos.

## Overview

**Creative North Star: "Catálogo alegre"**

Una portada con una fotografía de manicura coral y una carta abierta de precios.
Young Serif recta aporta oficio y personalidad; Manrope mantiene claras las
descripciones, los importes y las consultas. Crema y tinta sostienen la lectura,
con coral para las acciones y lila para acompañar el recorrido.

La clienta reconoce un diseño, consulta por ese diseño y puede sumar una
referencia de precio. Una sola foto ocupa la portada junto al panel lila. El
resto de la página usa fondos planos, filas abiertas y espacios reconocibles. La
identidad es propia de Uva y conserva el tono alegre con oficio elegido por Tomas.

**Key Characteristics:**

- Foto protagonista junto al titular sobre lila, con una entrada breve.
- Catálogo en grilla vertical con filtros y consulta propia por diseño.
- Carta de precios con puntitos guía y suma orientativa local.
- Franja lila de proceso, preguntas crema y cierre tinta.

## Colors

El crema es el lienzo; tinta sostiene la lectura; coral invita a reservar y lila
marca el recorrido. Se conservan los cuatro colores fijados en el brief.

### Primary

- **Coral cálido** (`coral`): acciones, consulta por diseño, flotante y palabra
  «diseño». Los controles coral llevan texto tinta.

### Secondary

- **Lila** (`lilac`): palabra «manos» y hover de filtros y acciones secundarias.
- **Lila suave** (`soft`): tono bajo existente para filtros, secundarias,
  filtros de galería y franja de proceso.

### Neutral

- **Crema** (`bg`): lienzo general y lectura sobre superficies tinta.
- **Tinta ciruela** (`ink`): texto, precios, selección, cierre y footer.

| Bloque | Fondo | Texto / acentos |
|---|---|---|
| Header y hero | Crema | Tinta; «diseño» coral y «manos» lila |
| Catálogo | Crema | Tinta; filtros lila suave, elegido tinta; CTA coral |
| Carta de servicios y extras | Crema | Tinta, puntitos tinta; controles de selección tinta |
| Proceso | Lila a tono bajo, soft existente | Tinta y números Young Serif |
| Preguntas | Crema | Tinta |
| Cierre y footer | Tinta | Crema; botón coral con texto tinta |
| Flotante | Coral | Icono tinta y borde crema |

No hay tarjetas blancas añadidas a servicios, proceso o calculadora; las fichas
del catálogo tampoco agregan un fondo blanco detrás del texto.

**The Ink Contrast Rule.** Coral lleva texto tinta. Las dos palabras coloreadas
del titular conservan su relleno y un contorno tinta fino (0,5 px), con el relleno
pintado por encima del trazo. No oscurecer la paleta fijada.

## Typography

**Display Font:** Young Serif, fallback serif; peso real 400 y estilo recto.
**Body Font:** Manrope, fallback sans-serif; pesos cargados 400, 500, 600 y 700.

**Character:** la serif distingue títulos, marca y resultado del sumador; la sans
ordena lectura y controles. No se simulan cursivas ni pesos de Young Serif.

### Hierarchy

- **Display:** H1 en dos líneas, 72 / 60 / 48 / 46 / 42 px según los cortes
  1100 / 900 / 600 / 400 px; interlínea 1,1 y 1,12 en móvil.
- **Headline:** H2 general 48 / 34 px, interlínea 1,16 / 1,18. Proceso 34 px,
  reducido a 30 px desde tablet.
- **Title:** diseños 25 / 24 px; servicios 24 px, 18 px en móvil y 17 px hasta
  400 px. Pasos 21 px, con ajustes 20 / 22 / 21 px.
- **Body:** base 16 px, interlínea 1,65 y máximo de párrafo 65ch. Lead 17 / 16 /
  15 px; descripciones de carta 15 / 14 px.
- **Label:** navegación y filtros 14 px; filtros móviles 13 px. Acciones
  generales 15 / 14 px, consultas por diseño 14 px.
- **Price:** importes base 24 px, 20 px en móvil y 19 px hasta 400 px, con cifras
  tabulares; extras móviles a 20 px. Resultado Young Serif 40 / 32 px; estado
  vacío 23 / 20 px.
- **Wordmark:** header 42 / 38 px; footer 84 / 76 px; interlínea 1.

**The Upright Serif Rule.** Young Serif permanece recta y en peso 400. Manrope
resuelve los énfasis funcionales y las cifras de la carta; el mínimo de notas,
tiempos y «desde» es 13 px.

## Layout

Orden de secciones: portada, diseños, carta de precios, proceso, preguntas,
reservar y footer. Marco máximo 1220 px, márgenes 40/28/22 px según ancho.
Header sticky 80/76 px; anclas con margen 104 px; footer con 6rem de reserva
inferior. Secciones generales con 96/68 px verticales; proceso 52/42 px.

La portada reúne el texto sobre lila y una foto de manos con manicura coral.
Desde 650 px hacia abajo, el texto y la foto se apilan. El titular usa coral
oscuro `#B94E3D` y lila oscuro `#765AA9` para mejorar el contraste.
El horario queda bajo los botones y la ubicación acompaña el titular.

El catálogo conserva cinco filtros (Todos, Francesitas, Nail art, Lisos y tonos,
Efectos) y muestra fotografías 4:3 en una grilla de tres, dos o una columna según
el ancho. Cada foto tiene debajo su nombre, descripción y botón propio. El acceso
«Ver precios y calcular» lleva desde el catálogo a la carta.

Carta: cinco filas sin tarjetas, máximo 980 px, padding vertical de fila 14 px,
nombre a izquierda y precio a derecha unidos por puntos. Descripción y duración
actuales se conservan debajo de cada fila. Apartado «Extras por uña», con dos
líneas separadas y cantidades. La suma vive
en la misma carta: un servicio base, retiro opcional y cantidades producen una
referencia orientativa. Extras sin servicio se identifican como subtotal.
Se conserva la nota de confirmación del total; no es una cotización
cerrada, pago, reserva automática ni cambio de reglas comerciales.

El proceso agrupa las cuatro etapas actuales en tres: foto de referencia,
confirmación y seña, diseño y cuidados. Conserva los cuatro títulos, los cuatro
párrafos y el 30% de seña; no elimina esa condición ni inventa otra. Franja ligera, números y
texto en línea; desde 900 px adapta a filas sin cajas pesadas. FAQ nativo,
mismo texto; pasa de dos columnas a una desde 900 px. El cierre se apila desde
1100 px; el footer pasa de tres columnas a dos y luego una.

## Elevation & Depth

El espacio y los fondos planos separan los bloques.

La foto se descubre de abajo hacia arriba en 880 ms y el titular entra en dos
tiempos. El filtro revela las fotos en 280 ms y el nuevo importe recibe un realce
lila de 410 ms. Lenis conserva el desplazamiento suave. Con movimiento reducido,
la portada, las fotos y los importes se actualizan de forma estática. Sin
JavaScript quedan visibles los diseños, los precios y los enlaces de WhatsApp.

## Shapes

La portada tiene esquinas de 18 px y las fotos del catálogo de 12 px.
Las acciones principales y los filtros usan cápsulas. La carta usa líneas abiertas.
El punteado tiene función de guía entre servicio y precio, solicitado por Tomas.

## Components

### Botones y filtros

Acciones sólidas: coral/tinta como principal y lila suave/tinta como secundaria.
Altura mínima general 52 px, 50 px en móvil; padding 14×23 px, 14×20 px en móvil.
La consulta del catálogo parte de 48 px y 13×20 px. Hover principal invierte a
tinta/crema; secundaria pasa a lila. Ambos suben 2 px y regresan al pulsar. En
el cierre tinta el hover usa crema/tinta. Foco visible de 3 px y separación 5 px.

Filtros de mínimo 44 px, padding 11×19 px y 17 px horizontales en móvil. Reposo
lila suave/tinta, seleccionado tinta/crema, hover lila/tinta. `aria-pressed`
refleja selección y el estado comunica el número visible. Las fichas apilan
foto, título, descripción y botón de consulta con borde y radio de 8 px.

### Catálogo por diseño

Cinco diseños existentes: Francesita nude, Ondas de color, Moño en rosa, Rojo de
siempre y Líneas de luz. Un enlace estático y funcional por diseño, aun sin JS:
«Quiero este diseño». Mensaje exacto: «Hola! Vi el diseño [NOMBRE] en la página y
quiero pedir un turno con ese diseño.» Nombre tomado literalmente del H3.
Destino siempre https://wa.me/5491100000000 .

### Carta y suma

Esmaltado semipermanente desde $22.000; Kapping / soft gel desde $28.000;
Esculpidas en gel desde $38.000; Service / relleno desde $26.000; retiro de otro
estudio $6.000. Extras: diseños a mano alzada desde $1.500 por uña; piedritas,
dijes y efectos (cromo, aurora, ojo de gato) desde $800 por uña. Los importes son
enteros y se suman sin redondeos monetarios. Cuatro radios mutuamente excluyentes
eligen el servicio base; retiro usa un checkbox independiente. Los controles
nativos de selección miden 20 px, con acento tinta y área de fila mínima 44 px.

Campos de cantidad de 76 px de ancho y mínimo 44 px de alto, padding 8×10 px,
borde tinta de 1 px y fondo crema. Aceptan enteros 0–10; vacío equivale a cero.
Los inválidos muestran «Usá cantidades enteras entre 0 y 10.» y «Revisá las
cantidades» como resultado, con `aria-invalid`; no publican una suma parcial.

Con radio seleccionado: «Total orientativo desde». Solo retiro: «Total
orientativo». Extras sin servicio base: «Subtotal de extras», o «Subtotal de
extras y retiro» cuando corresponde, junto con «Elegí un servicio para completar
el total.» Nunca se presenta ese subtotal como total de turno. «Limpiar
selección» restablece radios, checkbox y cantidades. El vacío invita a elegir
servicio. Se conserva la nota de confirmación de tiempo y total por foto.

Solo UI local y transitoria; sin datos personales, proveedor de pagos,
persistencia, reserva automática ni cobros. Sin JS la carta completa sigue
siendo legible; la mención ficticia a la seña no habilita pagos.

### Navegación, FAQ y WhatsApp

Navegación Manrope 600, enlaces subrayados al hover y marca Young Serif recta.
Menú móvil desde 900 px, botón 44×44 px, estado expandido y Escape que devuelve
el foco al botón. Sin JS las anclas quedan visibles y envueltas. FAQ nativo
details/summary, seis preguntas con más SVG de 20 px que gira 45° al abrir.
Tres href originales de WhatsApp intactos (hero, cierre, flotante), más cinco
del catálogo. Icono SVG de
WhatsApp estándar actual, cuadrado y sin compresión, no se redibuja.

## Do's and Don'ts

### Do:

- **Do** mantener la portada y la grilla dentro del ancho de pantalla a 430 px.
- **Do** preservar títulos de diseños, precios, textos de FAQ y tres href originales.
- **Do** dejar el CTA por diseño visible bajo su imagen y disponible sin JS.
- **Do** distinguir subtotal de extras y total con servicio, conservando «desde».
- **Do** mantener notas, tiempos y «desde» en un mínimo de 13 px.
- **Do** conservar foco visible, controles nativos y movimiento reducido.

### Don't:

- **Don't** trasladar el molde de Bruma ni alterar Mora.
- **Don't** agregar precios, servicios, cobros, testimonios ni afirmaciones reales.
- **Don't** añadir tarjetas blancas para vestir la carta o el proceso.
- **Don't** convertir extras sin servicio en un total de turno.
- **Don't** presentar filtros o sumador como funcionales si JavaScript no está activo.
- **Don't** añadir fotos nuevas, cursivas sintéticas o una tipografía alternativa.

## Fotografías y procedencia

Las fotografías reutilizadas están en assets/ y son material ilustrativo de
Pexels. [Licencia](https://www.pexels.com/license/).

| Archivo | Ubicación decidida | Fuente |
|---|---|---|
| hero-coral.webp | Foto de portada, manos coral | Lazar Gugleta — https://www.pexels.com/photo/hands-of-a-woman-with-orange-nail-polish-11393877/ |
| diseno-ondas.webp | Catálogo, «Ondas de color» | cottonbro studio — https://www.pexels.com/photo/close-up-shot-of-hands-with-colorful-nail-polish-5871824/ |
| diseno-francesita.webp | Catálogo, «Francesita nude» | Roman Titov — https://www.pexels.com/photo/hand-with-french-tip-nails-13038494/ |
| diseno-mono.webp | Catálogo, «Moño en rosa» | Salim Da — https://www.pexels.com/photo/close-up-of-elegant-manicured-nails-with-floral-design-34885842/ |
| diseno-rojo.webp | Catálogo, «Rojo de siempre» | Oleskandra Biliak — https://www.pexels.com/photo/close-up-of-a-hand-of-a-woman-with-red-nails-17389258/ |
| diseno-dorado.webp | Catálogo, «Líneas de luz» | Анастасія — https://www.pexels.com/photo/elegant-nail-art-with-gold-details-in-natural-light-31744665/ |

Los descartes históricos 6852174 (marca en ropa) y 34121866 (rostro) siguen fuera.
Créditos accesibles desde el footer con esta misma ancla.

## Contenido de muestra

Marca, personas, precios, contacto, horarios, seña del 30% y condiciones son
ficticios y se conservan. Footer exacto: «Vidriera de demostración de Nexvia IA ·
Marca, personas y datos ficticios.» Noindex/nofollow se mantiene.

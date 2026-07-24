
# Landing 1 — Laboratorio de Creatividad para Astrólog@s

Landing de captación para **Gaby Tomás** (astróloga, docente de teatro y psicodramatista), primera etapa del funnel de venta de su programa de astrología, creatividad y teatro. Esta landing capta inscriptos al Laboratorio de Creatividad gratuito (2 encuentros online), los deriva a un grupo de WhatsApp, y teasea el programa pago de 7 clases al que se accede después.

> ✅ **Estado actual: copy real cargado y optimizaciones de UI/UX completadas.** La estructura, el diseño visual y la lógica interactiva (carrusel infinito y footer responsive) están completamente integrados. Quedan puntos puntuales pendientes de confirmación — ver [Pendiente](#pendiente).

## Estructura del sitio

1. **Navbar** — logo, link "¿Quién soy?" y accesos a redes sociales (Instagram, Facebook, WhatsApp).
2. **Hero** — "Laboratorio de Creatividad para Astrólog@s", 2 encuentros gratuitos online, meta de fecha/duración/cupos, CTA de inscripción.
3. **Dolor** — 5 preguntas de identificación dirigidas a astrólog@s (inseguridad, falta de recursos, rigidez técnica).
4. **Transformación** — promesa central + 4 beneficios concretos post-encuentros.
5. **Qué incluye** — bullets del contenido del Laboratorio (ejercicios, dinámicas, PDF, grabaciones).
6. **Para quién es / no es** — dos columnas de calificación del lead.
7. **Testimonios** — carrusel horizontal infinito e bidireccional mediante duplicación cuádruple en DOM y medición geométrica dinámica (`getBoundingClientRect`), soporta *swipe* suave con clase `.no-snap` para transiciones sin salto visual.
8. **Formulario de inscripción** — nombre, email, WhatsApp, y botón de unión al grupo de WhatsApp.
9. **Sobre mí** — foto, bio y credenciales de Gaby Tomás.
10. **Cierre** — frase de cierre + CTAs de inscripción y WhatsApp.
11. **Próximos talleres** — teaser del programa pago "Recursos para potenciar la Sesión Astrológica" (7 clases, arranca 26/8, $245.000 con descuento).
12. **Contactanos** — formulario simple de consultas.
13. **Footer** — redes y datos de contacto reestructurados en mobile (`max-width: 640px`) con alineación central explícita, reseteo de `flex-basis` (`flex: 0 0 auto`) y espaciados/paddings compactos mediante unidades relativas (`rem`).

## Estructura de archivos

```

├── index.html        # Estructura principal + script de carrusel infinito bidireccional
├── styles.css        # Estilos globales, paleta de colores, reglas CSS del carrusel y footer responsive
└── src/
├── hero-bg.jpg   # Fondo del hero
├── course-card1.jpg
└── course-card2.jpg

```

## Stack y Tecnologías

- **HTML5 + CSS3 + JavaScript (Vanilla):** Sin dependencias, frameworks ni pasos de compilación (*build step*).
- **Flexbox & CSS Grid Layout:** Diseño responsive con breakpoint en `640px`.
- **CSS Paged & Relative Units:** Uso riguroso de `rem` y `clamp()` para escalabilidad tipográfica y de layout.
- **Paleta de diseño:** *Night-sky* (`#14122b`) con acentos dorados (`#d9a95f`), lila (`#b8a9d9`) y tipografía *serif* en encabezados.
- **Deploy target:** Pensado para integración/deploy directo en **systeme.io** (formularios, Mercado Pago, automatizaciones de WhatsApp).

## Registro de Cambios Recientes (Sesión Actual)

### Carrusel Infinito de Testimonios (`index.html` & `styles.css`)

- **Loop Infinito Bidireccional:** Se reestructuró la clonación de nodos a 2 conjuntos previos y 2 posteriores para permitir scroll continuo tanto hacia la izquierda como hacia la derecha desde el renderizado inicial.
- **Cálculo Geométrico Dinámico:** Transición de cálculos de ancho estáticos a medición vía `getBoundingClientRect().left`, garantizando la sincronización del reset sin importar alineación (`center` o `start`) o paddings activos.
- **Reset de Snap Invisible:** Implementación de la clase CSS `.no-snap` (`scroll-snap-type: none !important; scroll-behavior: auto !important;`) aplicada temporalmente por JS durante el reposicionamiento del scroll.

### Footer Responsive y Alineación Mobile (`styles.css`)

- **Alineación Central:** Se agregaron reglas `@media (max-width: 640px)` para forzar la alineación al centro (`text-align: center`, `align-items: center`) de textos, títulos e íconos de redes sociales.
- **Colapso de Espacio Vertical:** Anulación del crecimiento flex de las columnas (`flex: 0 0 auto !important;`) y sobreescritura de paddings internos del `footer` (`padding: 1.5rem 1rem 1rem !important;`), eliminando espacios en blanco innecesarios.
- **Relatividad de Espaciados:** Normalización de todos los márgenes y *gaps* del footer a unidades `rem` (`gap: 1rem`, `margin-bottom: 0.25rem` / `0.125rem`).

---

## Repositorio y deploy

- El repo está pensado para pasar a **privado**, con Julián y Gonzalo como colaboradores.
- **Importante:** con GitHub Free, Pages solo funciona sobre repos públicos. Para tener repo privado + demo pública en Pages hace falta **GitHub Pro** (repo personal) o **GitHub Team** (repo de organización) — o, como alternativa sin costo extra, mover el deploy de la demo a Netlify/Vercel conectado al repo privado.
- Definición pendiente: con cuál de las dos opciones se sigue.

## Pendiente

- Confirmar si **"Gaby Tomás"** es el nombre de marca definitivo (se reemplazó "Gabriela" en base a la bio recibida, a confirmar con Gonzalo).
- Fechas exactas de agosto de los 2 encuentros gratuitos (el brief solo indica "[día] y [día] de agosto").
- Confirmar si los 4 testimonios cargados corresponden a este Laboratorio gratuito o a una edición anterior del programa pago.
- Link real del grupo de WhatsApp.
- Email y teléfono de contacto reales.
- Foto real de Gaby Tomás.
- Enlaces reales de redes sociales.
- Copy de la sección "Contactanos" (sigue en placeholder).
- Landing 2 (conversión/venta del programa pago) — se construye en semana 4-5, después de los encuentros gratuitos, según el plan de ejecución.

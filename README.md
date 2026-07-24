# Landing 1 — Laboratorio de Creatividad para Astrólog@s

Landing de captación para **Gaby Tomás** (astróloga, docente de teatro y psicodramatista), primera etapa del funnel de venta de su programa de astrología, creatividad y teatro. Esta landing capta inscriptos al Laboratorio de Creatividad gratuito (2 encuentros online), los deriva a un grupo de WhatsApp, y teasea el programa pago de 7 clases al que se accede después.

> ✅ **Estado actual: copy real cargado.** La estructura, el diseño visual y el copy de la mayoría de las secciones ya están resueltos a partir del material que compartió el equipo. Quedan puntos puntuales pendientes de confirmación — ver [Pendiente](#pendiente).

## Estructura del sitio

1. **Navbar** — logo, link "¿Quién soy?" y accesos a redes sociales (Instagram, Facebook, WhatsApp)
2. **Hero** — "Laboratorio de Creatividad para Astrólog@s", 2 encuentros gratuitos online, meta de fecha/duración/cupos, CTA de inscripción
3. **Dolor** — 5 preguntas de identificación dirigidas a astrólog@s (inseguridad, falta de recursos, rigidez técnica)
4. **Transformación** — promesa central + 4 beneficios concretos post-encuentros
5. **Qué incluye** — bullets del contenido del Laboratorio (ejercicios, dinámicas, PDF, grabaciones)
6. **Para quién es / no es** — dos columnas de calificación del lead
7. **Testimonios** — carousel horizontal de 4 testimonios reales (Viviana B., Paula M., Lorena B., Natalia P.), 3 tarjetas visibles por vista con scroll-snap y scrollbar temática
8. **Formulario de inscripción** — nombre, email, WhatsApp, y botón de unión al grupo de WhatsApp
9. **Sobre mí** — foto, bio y credenciales de Gaby Tomás
10. **Cierre** — frase de cierre + CTAs de inscripción y WhatsApp
11. **Próximos talleres** — teaser del programa pago "Recursos para potenciar la Sesión Astrológica" (7 clases, arranca 26/8, $245.000 con descuento)
12. **Contactanos** — formulario simple de consultas
13. **Footer** — redes y datos de contacto

## Estructura de archivos

```
├── index.html
├── styles.css
└── src/
    ├── hero-bg.jpg          # fondo del hero
    ├── course-card1.jpg     # sin uso actualmente (el hero ya no usa tarjetas por encuentro)
    └── course-card2.jpg     # sin uso actualmente (el hero ya no usa tarjetas por encuentro)
```

## Stack

- HTML5 + CSS3 estático, sin frameworks ni build step
- Paleta night-sky con acentos dorados y lila, tipografía serif para headers
- Pensado para deploy directo en **systeme.io** (formularios, Mercado Pago, automatizaciones de WhatsApp)

## Repositorio y deploy

- El repo está pensado para pasar a **privado**, con Julián y Gonzalo como colaboradores.
- **Importante:** con GitHub Free, Pages solo funciona sobre repos públicos. Para tener repo privado + demo pública en Pages hace falta **GitHub Pro** (repo personal) o **GitHub Team** (repo de organización) — o, como alternativa sin costo extra, mover el deploy de la demo a Netlify/Vercel conectado al repo privado.
- Definición pendiente: con cuál de las dos opciones se sigue.

## Pendiente

- Confirmar si **"Gaby Tomás"** es el nombre de marca definitivo (se reemplazó "Gabriela" en base a la bio recibida, a confirmar con Gonzalo)
- Fechas exactas de agosto de los 2 encuentros gratuitos (el brief solo indica "[día] y [día] de agosto")
- Confirmar si los 4 testimonios cargados corresponden a este Laboratorio gratuito o a una edición anterior del programa pago
- Link real del grupo de WhatsApp
- Email y teléfono de contacto reales
- Foto real de Gaby Tomás
- Enlaces reales de redes sociales
- Copy de la sección "Contactanos" (sigue en placeholder)
- Landing 2 (conversión/venta del programa pago) — se construye en semana 4-5, después de los encuentros gratuitos, según el plan de ejecución

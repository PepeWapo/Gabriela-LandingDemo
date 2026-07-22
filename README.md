# Landing Gabriela — Astrología, Creatividad y Teatro

Landing page para **Gabriela**, psicóloga que lanza un programa que combina astrología, creatividad y teatro. El sitio funciona como funnel único: capta inscriptos a dos encuentros gratuitos, los deriva a un grupo de WhatsApp, y presenta el programa pago de recursos psicológicos para astrólogos.

> ⚠️ **Estado actual: esqueleto / placeholder.** Toda la estructura y el diseño visual están definidos; el copy real está pendiente del brief de discovery con Gabriela (tono de marca, precio, fechas de los encuentros).

## Estructura del sitio

1. **Navbar** — logo y accesos a redes sociales (Instagram, Facebook, WhatsApp)
2. **Hero** — presenta los 2 encuentros gratuitos de creatividad/teatro, con CTA de inscripción y botón secundario hacia "Sobre mí"
3. **Testimonios** — grid de experiencias de participantes
4. **Formulario de inscripción** — nombre, email, WhatsApp, selección de encuentro, y botón de unión al grupo de WhatsApp
5. **Sobre mí** — foto, bio y credenciales de Gabriela
6. **Próximos talleres** — presentación del programa pago de recursos psicológicos para astrólogos
7. **Contactanos** — formulario simple de consultas
8. **Footer** — redes y datos de contacto

## Estructura de archivos

```
├── index.html
├── styles.css
└── src/
    ├── hero-bg.jpg          # fondo del hero
    ├── course-card1.jpg     # fondo tarjeta encuentro 01
    └── course-card2.jpg     # fondo tarjeta encuentro 02
```

## Stack

- HTML5 + CSS3 estático, sin frameworks ni build step
- Paleta night-sky con acentos dorados y lila, tipografía serif para headers
- Pensado para deploy directo en **systeme.io** (formularios, Mercado Pago, automatizaciones de WhatsApp)

## Pendiente

- Copy final de todas las secciones (a partir del brief de discovery)
- Fechas, precio y modalidad del programa pago
- Testimonios reales de los encuentros gratuitos
- Foto y bio definitiva de Gabriela
- Enlaces reales de redes sociales
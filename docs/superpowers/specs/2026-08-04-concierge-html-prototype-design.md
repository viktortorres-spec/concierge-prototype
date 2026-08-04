# Prototipo HTML — App Concierge by CC

**Fecha:** 2026-08-04 · **Fuente:** Figma "App Concierge by CC" (survey visual en viewer, sin dev mode)

## Objetivo

Prototipo HTML navegable en formato móvil del flujo principal de la app de concierges/comisionistas de Grupo Anderson's (reservas en restaurantes + comisiones + pagos vía Mercado Pago). Audiencia: cliente/stakeholder — debe verse pulido.

## Enfoque (aprobado: opción A)

- **Un solo archivo** `index.html`: CSS y JS embebidos, cero build, cero dependencias locales.
- Cada pantalla es una `<section class="screen">`; JS vanilla alterna la activa con transición slide.
- Marco de teléfono 390×844 centrado en desktop; fullscreen en viewport móvil.
- Imágenes: Picsum (seeds estables) para heros/fotos — nivel 2 por audiencia cliente.
- Design tokens del Figma: navy `#1E2837`, naranja `#C77E3E`, verde estados `#2FA860`, rojo `#D64541`, fondo `#F4F4F6`, cards blancas redondeadas, status bar iOS "9:41".

## Pantallas (flujo principal)

1. Splash (navy, logo, barra progreso, auto-avanza)
2. Login (selector hotel, usuario, contraseña, Entrar)
3. Home (hero, comisiones hoy/mes, botón Nueva Reserva, MIS RESERVAS, bottom nav)
4. Mis Reservas (chips filtro, cards por restaurante con estados, card expandible con detalle)
5. Nueva Reserva — Selecciona ciudad
6. Nueva Reserva — Selecciona unidad (restaurante)
7. Nueva Reserva — Reservación (personas, calendario, horario)
8. Confirmación de reserva (check verde)
9. Mis Comisiones (header navy acumulado, chips, lista)
10. Notificaciones (chips, lista de eventos)
11. Perfil (datos usuario, tipo concierge, cuenta Mercado Pago, identificación)
12. Menú hamburguesa (overlay dark)

## Navegación

- Bottom nav 5 iconos (home, reservas, comisiones, notificaciones, perfil) visible solo en pantallas principales; estado activo naranja.
- Flujo Nueva Reserva: ciudad → unidad → reservación → confirmación → home.
- Menú hamburguesa como overlay desde Home.
- Interacciones demo: chips cambian estado visual, cards expanden/colapsan, splash auto-avanza.

## Fuera de alcance

Registro, recuperación de contraseña, feed de noticias, QR/menú footer, modales de edición de perfil, lógica real (validación, datos dinámicos).

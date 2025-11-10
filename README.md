# Marie Salón & Spa

Sitio web estático para el salón y spa "Marie Salón & Spa" ubicado en Trujillo, Perú. Es una landing page optimizada para conversión con un flujo claro: Hero → Servicios → Sobre Nosotros → Feed → Ubicación → Contacto/CTA.

## Demo Local

- Abrir directamente `index.html` en el navegador, o
- Usar un servidor estático:
  - `npm init -y`
  - `npx serve -s . -l 5173`
  - Vista previa: `http://localhost:5173/`

## Tecnologías Utilizadas

- HTML5 (estructura y contenido)
- Tailwind CSS (CDN) para estilos utilitarios
- Google Fonts (`Inter`, `Playfair Display`)
- Node + `serve` (solo para desarrollo local / vista previa)

## Características Principales

- Header fijo con navegación y CTA de reserva.
- Hero con imagen de fondo, overlay y llamado a la acción vía WhatsApp.
- Sección de servicios en tarjetas (grid responsive).
- Sección "Sobre Nosotros" para reforzar la propuesta de valor.
- Simulación de feed de Instagram con enlace real a `@mariesalon25`.
- Sección de ubicación con Google Maps embebido.
- Sección de contacto con CTA final y formulario básico (estático).

## Estructura del Proyecto

```
MARIE SALON/
├── assets/
│   └── img/
│       └── banner1.jpeg
├── index.html        ← Página principal (contenido real)
├── index_bckup_1.html
└── package.json      ← Usado si levantas servidor local
```

## Datos Reales Editables

- Título del sitio: en `<head>` de `index.html`
  - `title`: "Marie Salón & Spa - Renueva tu Look y Bienestar en Trujillo"
  - `meta[name="description"]`: descripción SEO editable
- Hero (dentro de `#hero` en `index.html`)
  - `h1`: "Renueva tu look, reconecta contigo."
  - `h2`: "Tu salón & spa en Trujillo dedicado a tu bienestar."
  - Botón WhatsApp (`a[href]`): `https://wa.me/51987654321?text=Hola!...`
- Instagram
  - Handle: `@mariesalon25` — enlace a `https://www.instagram.com/mariesalon25/`
- Ubicación y Contacto
  - Dirección: `Av. Larco 123, Urb. La Merced, Trujillo`
  - Horarios: `Lun–Vie 9:00–20:00`, `Sáb 10:00–18:00`
  - Teléfono: `+51 987 654 321`
  - Google Maps `iframe[src]`: reemplazar con el embed real del local

Para editar cualquiera de estos datos, abre `d:\MARIE SALON\index.html` y modifica los elementos correspondientes.

## Cómo Ejecutar en Local

- Opción 1: Abrir `index.html` haciendo doble clic.
- Opción 2: Servidor local
  - `npm init -y`
  - `npx serve -s . -l 5173`
  - Navegar a `http://localhost:5173/`

## Preparar y Subir al Repositorio (branch `main`)

- Repositorio: `https://github.com/Crismandev/marie-salon`
- Pasos (PowerShell / CMD):

```
cd "d:\MARIE SALON"

:: Inicializa Git y usa main como rama principal
git init
git branch -M main

:: Añade archivos y realiza el primer commit
git add .
git commit -m "Initial commit: Marie Salon & Spa landing"

:: Apunta al repositorio remoto y sube a main
git remote add origin https://github.com/Crismandev/marie-salon.git
git push -u origin main
```

- Si el repo remoto ya tiene historial y necesitas unirlo:

```
git pull origin main --allow-unrelated-histories
:: resuelve conflictos si los hay, luego
git push -u origin main
```

## Personalización de Estilos

- Tailwind está cargado vía CDN. Puedes ajustar colores y fuentes en el bloque `tailwind.config` dentro de `index.html`.
- Paleta actual:
  - `aura-pink-light`: `rgb(249, 236, 235)`
  - `aura-pink-accent`: `rgb(222, 161, 154)`
  - `aura-beige`: `rgb(245, 241, 237)`
  - `aura-text`: `rgb(30, 41, 59)`

## Próximas Mejoras (Sugerencias)

- Integrar un widget real de Instagram (Elfsight, Lightwidget, etc.).
- Añadir script para menú móvil (toggle del menú).
- Conectar el formulario de contacto a un backend o servicio (Formspree, Netlify Forms, etc.).
- Optimizar imágenes y agregar `srcset`.

## Contacto

- Instagram: `https://www.instagram.com/mariesalon25/`
- WhatsApp reservas: `https://wa.me/51987654321/`
- Teléfono: `+51 987 654 321`
- Dirección: `Av. Larco 123, Urb. La Merced, Trujillo, Perú`

---

Cualquier cambio visual en `index.html` puede validarse levantando el servidor local y abriendo `http://localhost:5173/`.
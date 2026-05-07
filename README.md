# 💰 Finanzas Personales

Dashboard personal para gestionar ingresos, gastos y deudas. Funciona como PWA — instalable en celular y laptop sin app store.

## Características

- Registro de ingresos y gastos (fijos y variables)
- Calendario mensual con puntos de color por evento
- Alertas de pagos próximos (7 días)
- Resumen por categoría con barra de progreso
- Registro de deudas con historial de abonos
- Instalable como app (PWA) en Android, iOS, Windows y macOS
- Funciona sin internet después de la primera carga
- Datos guardados localmente en el dispositivo (localStorage)

## Estructura de archivos

```
finanzas-app/
├── index.html       ← App principal
├── manifest.json    ← Configuración PWA
├── sw.js            ← Service Worker (offline)
└── icons/           ← Íconos de la app
    ├── icon-72x72.png
    ├── icon-96x96.png
    ├── icon-128x128.png
    ├── icon-144x144.png
    ├── icon-152x152.png
    ├── icon-192x192.png
    ├── icon-384x384.png
    └── icon-512x512.png
```

## Deploy en Vercel (recomendado)

### Paso 1 — Subir a GitHub

1. Crear cuenta en [github.com](https://github.com) si no tienes
2. Clic en **New repository** → nombre: `finanzas-app` → **Create repository**
3. Subir todos los archivos de esta carpeta (arrastra y suelta en la interfaz web, o usa Git)

### Paso 2 — Publicar en Vercel

1. Ir a [vercel.com](https://vercel.com) → **Sign up with GitHub**
2. Clic en **Add New Project** → selecciona el repositorio `finanzas-app`
3. Dejar todo por defecto → clic **Deploy**
4. En ~30 segundos tendrás un link tipo `finanzas-app.vercel.app`

### Paso 3 — Instalar como app

**Android (Chrome):**
- Abre el link en Chrome
- Toca el banner "📲 Instalar app" que aparece abajo
- O: menú (⋮) → "Añadir a pantalla de inicio"

**iPhone/iPad (Safari):**
- Abre el link en Safari (debe ser Safari, no Chrome en iOS)
- Toca el ícono de compartir (□↑)
- Selecciona "Añadir a pantalla de inicio"

**Windows/macOS (Chrome o Edge):**
- Abre el link
- En la barra de dirección aparece un ícono de instalación (⊕)
- Clic → "Instalar"

## Notas

- Los datos se guardan en el navegador del dispositivo (localStorage). Cada dispositivo tiene sus propios datos.
- Para compartir datos entre dispositivos, en el futuro se puede agregar sincronización con Google Drive o Supabase.

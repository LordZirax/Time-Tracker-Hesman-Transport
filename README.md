# Mis Horas — PWA Time Tracker

## Instalación en Android (3 minutos)

### Opción A: GitHub Pages (GRATIS, recomendado)

1. **Crea cuenta en GitHub** si no tienes: https://github.com/signup

2. **Crea un repositorio nuevo:**
   - Ve a https://github.com/new
   - Nombre: `mis-horas`
   - Selecciona **Public**
   - Click **Create repository**

3. **Sube los archivos:**
   - En el repo nuevo, click **"uploading an existing file"**
   - Arrastra TODOS los archivos de esta carpeta: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`
   - Click **Commit changes**

4. **Activa GitHub Pages:**
   - Ve a **Settings** → **Pages** (menú lateral izquierdo)
   - Source: **Deploy from a branch**
   - Branch: **main** / **(root)**
   - Click **Save**
   - En 1-2 minutos tu app estará en: `https://TU-USUARIO.github.io/mis-horas/`

5. **Instala en Android:**
   - Abre la URL en Chrome
   - Chrome mostrará un banner "Agregar a pantalla de inicio" o:
   - Toca el menú ⋮ → **"Instalar app"** o **"Agregar a pantalla de inicio"**
   - Listo! Aparece como app con ícono propio

### Opción B: Netlify (también gratis)

1. Ve a https://app.netlify.com/drop
2. Arrastra la carpeta completa
3. Te da una URL automática
4. Abre en Chrome → Instalar como app

---

## Funciones
- Un botón para entrada/salida
- Campo de servicio/empresa con chips rápidos
- Notas explicativas por turno
- Redondeo automático cada 15 minutos (0.25h)
- Turnos que cruzan medianoche
- Entradas retroactivas
- Exportación CSV por rango de fechas
- Funciona 100% offline una vez instalada
- Datos guardados en localStorage del teléfono

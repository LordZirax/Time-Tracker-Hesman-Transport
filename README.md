# Ziad Personal Driver Time Tracker — v10

App web (PWA) para registrar horas de trabajo, pausas y hojas de ruta. Instalable en Android/PC, funciona offline, trilingüe (ES / EN / FR).

---

## Instalación en Android

1. Abre en Chrome: `https://lordzirax.github.io/Time-Tracker-Hesman-Transport/`
2. Menú ⋮ → **Instalar app** (o "Agregar a pantalla de inicio")
3. Aparece como app con su propio ícono, funciona sin internet

## Abrir en PC

- Online: misma URL en cualquier navegador
- Offline: descarga el ZIP, extrae y abre `index.html`

> Los datos NO se sincronizan entre dispositivos. Cada uno guarda los suyos en local. Para pasar datos: exporta el respaldo JSON y restáuralo en el otro equipo.

---

## Funciones

### Registro de tiempo
- Un botón grande para ENTRADA / SALIDA
- Redondeo automático a 15 min (22→15, 23→30)
- Timer en vivo mientras trabajas

### Pausas
- Botón ⏸ PAUSA en vivo (congela el tiempo trabajado)
- En hojas de ruta y en entradas retroactivas (varias pausas)
- Se descuentan del total; redondeo 15 min individual

### Servicios y pago
- Registra servicios en ⚙ Ajustes → MIS SERVICIOS
  - Por hora: $X/h + bonus opcional por hora
  - Tarifa fija: $Y por jornada
- El monto bruto se calcula sobre horas netas
- Se muestra por entrada, por período y en reportes

### Hojas de ruta
- Una por día, con cliente, conductor, vehículo, KM
- Paradas con llegada/salida, ubicación, palettes, factura, observaciones
- Pausas con detalle
- Export PDF (limpio) y CSV en el idioma de la app

### Historial plegable
- Pestañas: Today / Week / Biweekly / Monthly
- Secciones plegables por rango, con total de horas y $
- El período más reciente se abre solo

### Exportar para RH
- 👁 Ver resultados (tabla en la app)
- 📄 PDF de reporte por rango de fechas
- 📊 CSV con horas, pausas, montos y notas

### Respaldo
- Descarga/restaura JSON con todos los datos, servicios y ajustes
- Consejo: respaldar cada viernes

---

## Idiomas
Español / English / Français. Auto-detecta el idioma del teléfono; cambiable en ⚙ Ajustes.

## Archivos
- `index.html` — la app completa
- `manifest.json` — config PWA
- `sw.js` — service worker (offline + cache)
- `icon-192.png`, `icon-512.png` — íconos

## Actualizar
Reemplaza los archivos en el repo. El service worker (v9) refresca el cache solo. Si ves la versión vieja: borra solo "caché/imágenes", nunca "datos del sitio" (ahí están tus registros).

## Privacidad
Todos los datos viven en el almacenamiento local del dispositivo. Nada se envía a ningún servidor.

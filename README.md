# 📚 Centro de Apps Docente

Dashboard personal para organizar todas tus aplicaciones web educativas.

**Desarrolladas por José R. White**

## 📦 Archivos incluidos

- `app-launcher.html` - Aplicación principal
- `manifest.json` - Configuración PWA
- `sw.js` - Service Worker (funciona offline)
- `icon-192.png` - Icono pequeño ✅ YA INCLUIDO
- `icon-512.png` - Icono grande ✅ YA INCLUIDO

## 🎯 Pasos para instalar

### 1. Subir a GitHub Pages

**Opción A: Crear un nuevo repositorio**

```bash
# En tu carpeta con todos los archivos:
git init
git add .
git commit -m "Initial commit: App Launcher PWA"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/app-launcher.git
git push -u origin main
```

Luego en GitHub:
- Ve a Settings → Pages
- En "Source" selecciona: `main` branch
- Click en "Save"
- Tu URL será: `https://TU-USUARIO.github.io/app-launcher/app-launcher.html`

**Opción B: Usar repositorio existente**

```bash
# Crea una carpeta "launcher" en tu repo
mkdir launcher
# Copia todos los archivos ahí
# Commit y push
git add launcher/
git commit -m "Add app launcher"
git push
```

Tu URL será: `https://TU-USUARIO.github.io/TU-REPO/launcher/app-launcher.html`

### 2. Instalar como PWA

**En Chrome (Escritorio):**
1. Abre la URL de GitHub Pages
2. En la barra de direcciones, verás un ícono de instalación (➕ o ⬇️)
3. Click en "Instalar" o menú ⋮ → "Instalar aplicación"

**En Chrome (Android):**
1. Abre la URL en Chrome
2. Menú ⋮ → "Añadir a pantalla de inicio"
3. Confirma el nombre y listo

**En Safari (iOS):**
1. Abre la URL en Safari
2. Tap en el botón Compartir (cuadrado con flecha)
3. "Añadir a pantalla de inicio"

## ✨ Cómo usar

1. **Agregar apps**: Click en el botón "+" 
2. **Nombre**: El nombre de tu app
3. **URL**: La dirección completa (https://...)
4. **Icono**: Selecciona un emoji
5. **Abrir**: Click en cualquier app para abrirla
6. **Eliminar**: Hover sobre una app y click en la "×"

## 🔧 Personalización

Edita `app-launcher.html` para cambiar:
- **Colores**: Busca `#f59e0b` y `#d97706` (gradiente amarillo/naranja)
- **Título**: Cambia "Centro de Apps Docente" en el `<h1>`
- **Emojis disponibles**: Edita el array `emojis` en el JavaScript

## 💾 Datos

Tus apps se guardan en **localStorage** del navegador. Son persistentes incluso si cierras la PWA.

## 🌐 Funciona offline

Gracias al Service Worker, la app funciona sin conexión a internet una vez instalada.

## 🤔 Problemas comunes

**"No aparece el botón de instalación":**
- Verifica que estés usando HTTPS (GitHub Pages lo usa automáticamente)
- Abre DevTools → Application → Manifest para ver errores
- Asegúrate de que los archivos icon-192.png e icon-512.png estén en la misma carpeta

## 📱 Compatible con

- ✅ Chrome (Android/Desktop)
- ✅ Edge
- ✅ Safari (iOS/macOS)
- ✅ Firefox (instalación manual)
- ✅ Samsung Internet

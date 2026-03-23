# 🛡️ FlexNet Agents — Guía de Instalación y Configuración

Guía interactiva completa para la instalación y configuración de los FlexNet Agents de Flexera en Windows, Linux, macOS y Contenedores.

Basada en la documentación pública oficial de Flexera (docs.flexera.com).

---

## 🚀 Publicación rápida

### Opción A: Vercel (recomendado, más fácil)

1. **Sube este proyecto a GitHub:**
   ```bash
   cd flexnet-guide-project
   git init
   git add .
   git commit -m "Initial commit - FlexNet Agent Guide"
   git branch -M main
   git remote add origin https://github.com/TU-USUARIO/flexnet-agent-guide.git
   git push -u origin main
   ```

2. **Despliega en Vercel:**
   - Ve a [vercel.com](https://vercel.com) y haz login con GitHub
   - Click en **"Add New Project"**
   - Selecciona el repositorio `flexnet-agent-guide`
   - Vercel detecta automáticamente que es un proyecto Vite
   - Click en **"Deploy"**
   - ¡Listo! Tu guía estará en `https://flexnet-agent-guide.vercel.app`

### Opción B: GitHub Pages

1. **Sube a GitHub** (igual que arriba)

2. **Instala dependencias y construye:**
   ```bash
   npm install
   npm run build
   ```

3. **Activa GitHub Pages:**
   - Ve a Settings → Pages en tu repositorio
   - Source: **GitHub Actions**
   - El workflow `.github/workflows/deploy.yml` incluido se encarga del resto

### Opción C: Netlify

1. **Sube a GitHub** (igual que arriba)
2. Ve a [netlify.com](https://netlify.com) → **"Add new site"** → **"Import from Git"**
3. Selecciona el repositorio
4. Build command: `npm run build`
5. Publish directory: `dist`
6. Click **"Deploy"**

---

## 💻 Desarrollo local

```bash
# Instalar dependencias
npm install

# Iniciar servidor de desarrollo
npm run dev

# Construir para producción
npm run build

# Previsualizar build de producción
npm run preview
```

---

## 📁 Estructura del proyecto

```
flexnet-guide-project/
├── index.html              # Punto de entrada HTML
├── package.json            # Dependencias y scripts
├── vite.config.js          # Configuración de Vite
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions para GitHub Pages
├── src/
│   ├── main.jsx            # Punto de entrada React
│   ├── App.jsx             # Componente principal (toda la guía)
│   └── index.css           # Estilos globales
└── README.md               # Este archivo
```

---

## 📦 HTML Autocontenido

También se incluye `flexnet-guide.html` como archivo único autocontenido que puedes:
- Abrir directamente en cualquier navegador (doble clic)
- Subir a SharePoint, intranet, o cualquier servidor web
- Enviar por email como adjunto
- Alojar en un bucket S3/GCS como sitio estático

---

## ⚠️ Disclaimer

Esta guía está basada en documentación pública de Flexera disponible en docs.flexera.com y community.flexera.com. **No es documentación oficial de Flexera.** Consulta siempre la documentación oficial correspondiente a tu versión antes de realizar instalaciones en producción.

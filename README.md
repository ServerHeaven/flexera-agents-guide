# FlexNet Agents — Guía de Instalación y Configuración / Installation and Configuration Guide

🌐 **Web / Live site:** https://serverheaven.github.io/flexera-agents-guide/
(`?lang=es` · `?lang=en`)

[Español](#español) · [English](#english)

---

## Español

Guía de referencia sobre la instalación y configuración de los agentes de Flexera para **Windows, Linux, macOS y contenedores**. Está disponible en español e inglés, con un selector **ES | EN** en la cabecera.

> Guía basada en documentación pública de Flexera. **No es documentación oficial**: las versiones y comportamientos pueden cambiar, así que consulta siempre la documentación de tu versión en [docs.flexera.com](https://docs.flexera.com/).

### Contenido

| Sección | Qué cubre |
|---|---|
| Visión general | Tipos de agente, métodos de recolección de inventario, requisitos, disco y consumo, arquitectura de comunicación |
| Windows | FlexNet Agent (Eng. Apps) e Inventory Agent: wizard, instalación silenciosa, `mgssetup.ini`, MSI, logs |
| Linux | Instalación `.bin`/RPM/DEB, bootstrap `mgsft_rollout_response`, servicios, `mgsconfig` |
| macOS | Paquete `.pkg`, Gatekeeper, despliegue con JAMF |
| Contenedores | Agente de Kubernetes (completo y ligero), Helm, Docker/Podman |
| Configuración | Puertos, proxy, `flxconfig`, auto-actualización |
| Problemas | FAQ de resolución de problemas y ubicación de logs |
| Recursos | Índice de documentación oficial y changelog del agente |

Cada sección incluye enlaces a la documentación oficial de Flexera.


### Estructura y mantenimiento

- Todo el sitio está en [`index.html`](index.html): una aplicación React (con Babel en el navegador) y los estilos en línea.
- **Idiomas:** los textos se escriben con la función `t('español', 'english')`. Al añadir contenido, incluye siempre ambas versiones.
- El idioma se elige por este orden: parámetro `?lang=`, preferencia guardada en el navegador (`localStorage`) e idioma del navegador.
- Los enlaces a la documentación de Flexera están centralizados en el objeto `DOC` del propio `index.html`.
- El sitio se publica con GitHub Pages.

---

## English

Reference guide for installing and configuring Flexera agents on **Windows, Linux, macOS and containers**. It is available in Spanish and English, with an **ES | EN** switch in the header.

> This guide is based on Flexera's public documentation. **It is not official documentation**: versions and behavior may change, so always consult the documentation for your specific version at [docs.flexera.com](https://docs.flexera.com/).

### Contents

| Section | What it covers |
|---|---|
| Overview | Agent types, inventory collection methods, requirements, disk and resource usage, communication architecture |
| Windows | FlexNet Agent (Eng. Apps) and Inventory Agent: wizard, silent install, `mgssetup.ini`, MSI, logs |
| Linux | `.bin`/RPM/DEB installation, `mgsft_rollout_response` bootstrap, services, `mgsconfig` |
| macOS | `.pkg` package, Gatekeeper, JAMF deployment |
| Containers | Kubernetes agent (full and lightweight), Helm, Docker/Podman |
| Configuration | Ports, proxy, `flxconfig`, auto-update |
| Troubleshooting | Troubleshooting FAQ and log locations |
| Resources | Official documentation index and agent change log |

Every section links to the official Flexera documentation.

### Structure and maintenance

- The whole site lives in [`index.html`](index.html): a React app (with in-browser Babel) and inline styles.
- **Languages:** text is written with the `t('español', 'english')` helper. When adding content, always provide both versions.
- Language is chosen in this order: the `?lang=` parameter, the preference saved in the browser (`localStorage`), then the browser language.
- Links to Flexera documentation are centralized in the `DOC` object inside `index.html`.
- The site is published with GitHub Pages.

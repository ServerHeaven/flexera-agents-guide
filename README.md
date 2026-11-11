# Flexera One — Agentes de inventario / Inventory agents

🌐 **Web / Live site:** https://serverheaven.github.io/flexera-agents-guide/
(`?lang=es` · `?lang=en`)

[Español](#español) · [English](#english)

---

## Español

Guía de referencia sobre la **instalación, configuración y actualización de los agentes de Flexera One** (IT Asset Management e IT Visibility) y de sus componentes de recolección, con **matrices de compatibilidad**. Cubre el FlexNet Inventory Agent para **Windows, Linux/UNIX y macOS**, los agentes de **Kubernetes** (completo y ligero), el **Inventory Beacon** y la recolección sin agente (zero-footprint, scanner y conectores). Las diferencias de FlexNet Manager Suite on-premises se indican como notas. Está disponible en español e inglés, con un selector **ES | EN** en la cabecera.

> Versión de referencia: **Flexera One ITAM 2026 R2** (agente y beacon 27.0.0), según la documentación leída el 11/11/2026. Guía basada en documentación pública de Flexera. **No es documentación oficial**: las versiones y comportamientos pueden cambiar, así que consulta siempre la documentación de tu versión en [docs.flexera.com](https://docs.flexera.com/). Lo que no se ha podido confirmar en la documentación pública aparece marcado como «verificar en tu tenant/versión» (o con «?» en las matrices).

### Contenido

| Sección | Qué cubre |
|---|---|
| Visión general | Qué agente o componente usar y cuándo: adopción, despliegue de terceros, zero-footprint, scanner, Beacon, Kubernetes; rutas de la consola de Flexera One; arquitectura de comunicación |
| Matrices | **1** SO y versión por agente · **2** funcionalidades por agente/plataforma · **3** versión de agente frente a beacon/plataforma · **4** métodos de despliegue por plataforma |
| Windows | Inventory Agent: MSI + `mgssetup.ini`, instalación silenciosa, desinstalación, servicios, logs; apéndice FlexNet Agent (Eng. Apps) |
| Linux | RPM/DEB/AIX/Solaris, bootstrap `mgsft_rollout_response`, HTTPS y mTLS, modo *least privilege*, rutas personalizadas, desinstalación y versión |
| macOS | Paquete `.pkg`, versiones soportadas (13–27), Gatekeeper, Apple silicon, JAMF/Intune |
| Contenedores | Agentes de Kubernetes (completo KRM y ligero LWK), Helm, versiones y plataformas, Docker/Podman/containerd |
| Beacon y sin agente | Inventory Beacon (descarga, instalación, requisitos), zero-footprint, FlexNet Inventory Scanner, conectores y adaptadores |
| Actualización | Actualización automática por política, terceros y manual; reglas de ciclo de vida y compatibilidad |
| Configuración | Puertos, proxy, `flxconfig`, bootstrap HTTPS |
| Problemas | FAQ de resolución de problemas y ubicación de logs |
| Recursos | Índice de documentación oficial y changelog del agente (hasta 27.0.0) |

Cada sección incluye enlaces a la documentación oficial de Flexera.


### Estructura y mantenimiento

- Todo el sitio está en [`index.html`](index.html): una aplicación React (con Babel en el navegador) y los estilos en línea.
- **Idiomas:** los textos se escriben con la función `t('español', 'english')`. Al añadir contenido, incluye siempre ambas versiones.
- El idioma se elige por este orden: parámetro `?lang=`, preferencia guardada en el navegador (`localStorage`) e idioma del navegador.
- Los enlaces a la documentación de Flexera están centralizados en el objeto `DOC` del propio `index.html`.
- El sitio se publica con GitHub Pages.

---

## English

Reference guide for **installing, configuring and upgrading Flexera One agents** (IT Asset Management and IT Visibility) and their collection components, with **compatibility matrices**. It covers the FlexNet Inventory Agent for **Windows, Linux/UNIX and macOS**, the **Kubernetes** agents (full and lightweight), the **Inventory Beacon** and agentless collection (zero-footprint, scanner and connectors). Differences for on-premises FlexNet Manager Suite are shown as notes. It is available in Spanish and English, with an **ES | EN** switch in the header.

> Reference release: **Flexera One ITAM 2026 R2** (agent and beacon 27.0.0), based on the documentation read on 11 Nov 2026. This guide is based on Flexera's public documentation. **It is not official documentation**: versions and behavior may change, so always consult the documentation for your specific version at [docs.flexera.com](https://docs.flexera.com/). Anything that could not be confirmed in the public documentation is marked "verify in your tenant/version" (or "?" in the matrices).

### Contents

| Section | What it covers |
|---|---|
| Overview | Which agent or component to use and when: adoption, third-party deployment, zero-footprint, scanner, Beacon, Kubernetes; Flexera One console paths; communication architecture |
| Matrices | **1** OS and version per agent · **2** features per agent/platform · **3** agent version vs beacon/platform · **4** deployment methods per platform |
| Windows | Inventory Agent: MSI + `mgssetup.ini`, silent install, uninstall, services, logs; appendix on the FlexNet Agent (Eng. Apps) |
| Linux | RPM/DEB/AIX/Solaris, `mgsft_rollout_response` bootstrap, HTTPS and mTLS, least-privilege mode, custom paths, uninstall and version |
| macOS | `.pkg` package, supported versions (13–27), Gatekeeper, Apple silicon, JAMF/Intune |
| Containers | Kubernetes agents (full KRM and lightweight LWK), Helm, versions and platforms, Docker/Podman/containerd |
| Beacon and agentless | Inventory Beacon (download, install, requirements), zero-footprint, FlexNet Inventory Scanner, connectors and adapters |
| Upgrades | Automatic upgrade by policy, third-party and manual; lifecycle and compatibility rules |
| Configuration | Ports, proxy, `flxconfig`, HTTPS bootstrap |
| Troubleshooting | Troubleshooting FAQ and log locations |
| Resources | Official documentation index and agent change log (up to 27.0.0) |

Every section links to the official Flexera documentation.

### Structure and maintenance

- The whole site lives in [`index.html`](index.html): a React app (with in-browser Babel) and inline styles.
- **Languages:** text is written with the `t('español', 'english')` helper. When adding content, always provide both versions.
- Language is chosen in this order: the `?lang=` parameter, the preference saved in the browser (`localStorage`), then the browser language.
- Links to Flexera documentation are centralized in the `DOC` object inside `index.html`.
- The site is published with GitHub Pages.

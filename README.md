# 🚀 Mi MCP Server

<div align="center">

![MCP Server](https://img.shields.io/badge/MCP-Server-blue?style=for-the-badge)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)
![Node.js](https://img.shields.io/badge/Node.js-18+-green?style=for-the-badge&logo=node.js)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

**Un servidor del Model Context Protocol (MCP) construido con TypeScript que se conecta con cualquier cliente MCP como Claude, VS Code, Cursor y más**

[![Claude Desktop](https://img.shields.io/badge/Claude-Desktop-7C3AED?style=flat-square&logo=anthropic&logoColor=white)](https://claude.ai)
[![VS Code](https://img.shields.io/badge/VS-Code-007ACC?style=flat-square&logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com)
[![Cursor](https://img.shields.io/badge/Cursor-Editor-000000?style=flat-square&logo=cursor&logoColor=white)](https://cursor.sh)

</div>

---

## 📋 Tabla de Contenidos

- [✨ Características](#-características)
- [🛠️ Herramientas Disponibles](#️-herramientas-disponibles)
- [📦 Requisitos Previos](#-requisitos-previos)
- [🚀 Instalación](#-instalación)
- [🔧 Configuración para Clientes](#-configuración-para-clientes)
  - [VS Code](#visual-studio-code)
  - [Cursor](#cursor)
  - [Claude Desktop](#claude-desktop)
- [🧪 Uso y Pruebas](#-uso-y-pruebas)
- [📁 Estructura del Proyecto](#-estructura-del-proyecto)
- [🤝 Contribución](#-contribución)
- [📄 Licencia](#-licencia)

---

## ✨ Características

- ✅ **Herramientas (Tools)**: Funciones que la IA puede ejecutar
- ✅ **Recursos (Resources)**: Datos estructurados que la IA puede leer
- ✅ **Prompts**: Plantillas de instrucciones reutilizables
- ✅ **Compatible con múltiples clientes**: VS Code, Claude Desktop, Cursor y más
- ✅ **TypeScript**: Código tipado y moderno
- ✅ **Fácil de extender**: Añade tus propias herramientas en minutos

---

## 🛠️ Herramientas Disponibles

| Herramienta | Descripción | Ejemplo |
|-------------|-------------|---------|
| `echo` | Devuelve el mensaje que recibe | `echo("Hola mundo")` → "Echo: Hola mundo" |
| `sum` | Suma dos números | `sum(5, 3)` → "5 + 3 = 8" |
| `get_current_time` | Muestra la hora actual | `get_current_time()` → "Hora: 14:30:45" |
| `greeting` (Resource) | Saludo personalizado | `greeting://Juan` → "Hello, Juan!" |
| `summarize` (Prompt) | Plantilla para resumir texto | Pide resumir cualquier texto |

---

## 📦 Requisitos Previos

- [Node.js](https://nodejs.org/) (v18.0.0 o superior)
- [pnpm](https://pnpm.io/) (v8.0.0 o superior) o npm
- [Git](https://git-scm.com/) (opcional, para clonar)

---

## 🚀 Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/mcp-server.git
cd mcp-server
```

### 2. Instalar Dependencias

```bash
pnpm install
```

### 3. Compilar el proyecto

```bash
pnpm run build
```

### 4. Ejecutar el servidor

```bash
pnpm start
```

### Configuración para Clientes

1. Crea el archivo .vscode/mcp.json con el siguiente contenido:
```json
{
  "servers": {
    "mi-servidor": {
      "command": "node",
      "args": ["dist/index.js"]
    }
  }
}
```
2. Abre VS Code en la carpeta del proyecto
3. Asegúrate de tener la extensión GitHub Copilot instalada
4. En Copilot Chat, ya puedes usar las herramientas del servidor

### Estructura del Proyecto

```
mcp-server/
├── .vscode/
│   └── mcp.json          # Configuración para VS Code
├── dist/                  # Código compilado
├── src/
│   └── index.ts          # Código fuente del servidor
├── scripts/
│   └── install-desktop.js # Script para Claude Desktop
├── package.json          # Dependencias y scripts
├── tsconfig.json         # Configuración TypeScript
└── README.md             # Este archivo
```

### Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo LICENSE para más detalles.

### Agradecimientos

- Model Context Protocol - El protocolo que hace esto posible

- Anthropic - Por Claude y el soporte a MCP

- Comunidad de desarrolladores MCP
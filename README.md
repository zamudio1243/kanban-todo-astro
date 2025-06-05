# Kanban Board - Astro

Una aplicación de tablero Kanban construida con Astro.

## 📋 Requisitos previos

Este proyecto requiere **Node.js 20**. Se recomienda usar nvm para manejar las versiones de Node.js.

### Configuración con nvm

1. **Instalar nvm** (si no lo tienes):

   ```sh
   # macOS/Linux
   curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
   # Reinicia tu terminal o ejecuta:
   source ~/.bashrc  # o ~/.zshrc
   ```

2. **Usar la versión correcta de Node.js**:

   ```sh
   # Instalar y usar Node.js 20 (se lee automáticamente desde .nvmrc)
   nvm use

   # Si no tienes Node.js 20 instalado:
   nvm install 20
   nvm use 20
   ```

3. **Configuración automática** (opcional):
   Añade esto a tu `~/.zshrc` o `~/.bashrc` para cambiar automáticamente:
   ```sh
   # Auto-switch node version when .nvmrc is present
   autoload -U add-zsh-hook
   load-nvmrc() {
     if [[ -f .nvmrc && -r .nvmrc ]]; then
       nvm use
     fi
   }
   add-zsh-hook chpwd load-nvmrc
   load-nvmrc
   ```

## 🚀 Instalación y desarrollo

1. **Clonar el repositorio**:

   ```sh
   git clone <url-del-repositorio>
   cd kanban-todo-astro
   ```

2. **Usar la versión correcta de Node.js**:

   ```sh
   nvm use  # Esto usará Node.js 20 automáticamente
   ```

3. **Instalar dependencias**:

   ```sh
   npm install
   ```

4. **Iniciar el servidor de desarrollo**:
   ```sh
   npm run dev
   ```

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

To learn more about the folder structure of an Astro project, refer to [our guide on project structure](https://docs.astro.build/en/basics/project-structure/).

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

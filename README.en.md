# Droid Resource Manager

[中文](README.md)

Droid Resource Manager is a desktop app for managing **Droids / Skills / MCP / Prompts / Rules**. Built with Electron, React, and Vite.

## Highlights
- Home dashboard with manual resource initialization
- Droids: create/copy, drag-move, tools & config updates
- Skills: create/edit/delete, manual AI summary
- MCP: servers and tools listing
- Prompts / Rules management
- Marketplace and settings (import/export)

## Screenshots

![Home](screenshots/home.png)

![Skills Manager](screenshots/skills.png)

## Quick Start
~~~bash
npm install
npm run dev
~~~

## Build & Packaging
~~~bash
npm run build
npm run dist
~~~

## Data Sources
- Global resources: ~/.factory (droids, skills, etc.)
- Project resources: <project>/.factory
- Use “Init Resources” on Home to refresh caches

## Layout
~~~
electron/        # Electron main process + IPC
src/             # React renderer
public/          # icons and static assets
screenshots/     # README images
release/         # packaged output (LFS)
~~~

## Release & Git LFS
Executables in release/ are tracked with LFS:
~~~bash
git lfs install
git lfs pull
~~~

## License
MIT

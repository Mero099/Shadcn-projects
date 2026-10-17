# Shadcnspace

A React landing page built with Vite. The repository root is an npm workspace, so install dependencies and run scripts from the `Space` folder.

## Getting started

Requirements: Node.js 20.19+ or 22.12+ and npm.

1. Open a terminal in the `Space` folder.
2. Run `npm install` once to install every workspace dependency.
3. Run `npm run dev` to start the local development server.

Useful commands from the workspace root:

- `npm run dev` — start Vite with hot reload.
- `npm run build` — create a production build.
- `npm run preview` — preview the production build locally.
- `npm run lint` — run Oxlint.

## Project map

```text
Space/
├── package.json                 # Workspace scripts and shared setup
└── shadcn/                      # React/Vite application
    ├── index.html               # Browser document and page title
    ├── public/                  # Static files served from the site root
    ├── imags/                   # Image assets used by the page
    └── src/
        ├── main.jsx             # React application bootstrap
        ├── index.css            # Global styles, theme tokens, and page defaults
        ├── App.jsx              # Top-level Navbar + Home composition
        └── Componant/           # UI components (legacy folder spelling)
            ├── Home/            # Landing-page content and styles
            └── Navbar/          # Header, theme switch, and styles
```

## Where to make changes

- Update the homepage statistics, technology badges, or community avatars in the named data lists near the top of `src/Componant/Home/Home.jsx`.
- Change homepage layout and component-specific visuals in `src/Componant/Home/Home.css`.
- Change the header or theme toggle in `src/Componant/Navbar/Navbar.jsx` and `src/Componant/Navbar/Navbar.css`.
- Change global colors and light/dark theme tokens in `src/index.css`.
- Add dependencies to the app with `npm install <package> --workspace shadcn` from the `Space` folder.

Keep image paths and their matching files in `imags/` together when adding or replacing homepage images.

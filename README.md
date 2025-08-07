# 🧪 Angular 20 SSR Lab: Comparativa de CSR, SSR Clásico y SSR con Hidratación Parcial

Este proyecto demuestra y compara los tres enfoques principales de renderizado en Angular 20:

- ✅ **CSR (Client-Side Rendering)**
- 🟧 **SSR clásico con Angular Universal**
- 🟦 **SSR con Hidratación Parcial (Partial Hydration)**

---

## 📁 Estructura del proyecto

```bash
poke-ssr-lab/
├── src/app/
│   ├── home/               # Página de bienvenida
│   ├── csr/                # Buscador usando CSR puro
│   ├── ssr-classic/        # Buscador con SSR clásico (Angular Universal)
│   ├── ssr-hydration/      # Buscador con SSR e hidratación parcial
│   └── layout/             # Layout base común
├── app.routes.ts           # Enrutamiento central
├── app.config.ts           # Configuración con `provideClientHydration`
├── main.ts                 # Bootstrap
├── server.ts               # SSR clásico (Angular Universal)
└── ...
```

---

## 🚀 Instalación

```bash
npm install
```

---

## 🧪 Ejecutar en modo desarrollo

- **CSR puro**:

```bash
ng serve
```

- **SSR clásico (Angular Universal)**:

```bash
npm run dev:ssr
```

> Esto utiliza `@angular/platform-server`.

---

## 🔍 Qué hace cada buscador

| Enfoque              | Ruta                 | Detalles |
|----------------------|----------------------|----------|
| **CSR**              | `/csr`               | Renderiza todo en el cliente. 100% SPA. |
| **SSR clásico**      | `/ssr-classic`       | Render inicial en servidor, pero necesita hidratar todo para ser interactivo. |
| **SSR + hidratación**| `/ssr-hydration`     | Render inicial desde el servidor + hidratación selectiva solo en el input de búsqueda. Más eficiente. |

---

## 📊 Objetivo del proyecto

- Comparar experiencia de usuario, tiempo de carga, TTI y peso de JS.
- Explorar la nueva capacidad de **hidratación parcial** de Angular 20.
- Servir como ejemplo educativo o base para proyectos más avanzados.

---

## 📎 Requisitos

- Node.js 18+
- Angular CLI 20+
- Compatible con PNPM / NPM

---

## 📚 Recursos útiles

- [Angular SSR Docs](https://angular.dev/guide/ssr)
- [Hydration Partial](https://angular.dev/guide/hydration)
- [PokéAPI](https://pokeapi.co/)

---

## 🧑‍💻 Autor

Proyecto creado por [Tu Nombre] como prueba técnica y didáctica con Angular 20.
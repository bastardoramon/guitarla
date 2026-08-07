# GuitarLA

**GuitarLA** es una tienda online de guitarras construida con Vue 3. Ofrece un catálogo de productos y un carrito de compras funcional, gestionado con estado reactivo y persistencia local, todo en el lado del cliente (sin backend).

## Características principales

- Catálogo de 12 guitarras con productos estáticos.
- Carrito de compras funcional:
  - Agregar productos al carrito.
  - Incrementar / disminuir cantidades (límite mínimo de 1 y máximo de 5).
  - Eliminar productos individualmente y vaciar el carrito.
- Cálculo automático del total a pagar.
- Persistencia del carrito en `localStorage`.
- Héctor con modelo destacado.

## Stack tecnológico

- **Vue 3** — Composition API con `<script setup>`.
- **TypeScript**.
- **Vite** — bundler y dev server.
- **Bootstrap 5** + Google Fonts (Outfit).

## Requisitos previos

- Node.js instalado en tu equipo.

## Cómo ejecutar

```bash
# Instalar dependencias
npm install

# Iniciar servidor de desarrollo
npm run dev

# Compilar para producción
npm run build

# Previsualizar el build
npm run preview
```

## Estructura del proyecto

```text
src/
├── App.vue              # Componente raíz: estados, lógica del carrito y persistencia
├── main.ts              # Punto de entrada de la aplicación
├── data/
│   └── guitarras.js     # Datos estáticos del catálogo (12 guitarras)
├── components/
│   ├── Header.vue        # Logo, hero con modelo destacado y carrito desplegable
│   ├── Guitarra.vue      # Tarjeta individual de cada guitarra
│   └── Footer.vue        # Pie de página
├── assets/              # Recursos de la aplicación
└── style.css            # Estilos globales
```

## Notas

Este proyecto es un **ejemplo básico de estudio** creado con fines de aprendizaje. No incluye backend, persistencia en bases de datos ni gestión de pagos; el carrito se guarda únicamente en el `localStorage` del navegador.
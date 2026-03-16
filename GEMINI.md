# FoodSmash - Project Context

## Project Overview
FoodSmash is a Nuxt 3/4 application designed to demonstrate the capabilities of the Gemini CLI. It allows users to discover and share unique food combinations.

### Core Technologies
- **Framework**: [Nuxt 3/4](https://nuxt.com/) (Vue 3)
- **Styling**: Vanilla CSS (located in `app/assets/css/main.css`)
- **Icons**: [Lucide Vue Next](https://lucide.dev/guide/packages/lucide-vue-next)
- **Testing**: [Vitest](https://vitest.dev/) with [@nuxt/test-utils](https://nuxt.com/docs/getting-started/testing)
- **Language**: TypeScript

## Getting Started

### Installation
```bash
npm install
```

### Development
Start the development server:
```bash
npm run dev
```
The application will be available at `http://localhost:3000`.

### Production Build
```bash
npm run build
```

### Testing
Run the test suite:
```bash
npm run test
```

## Project Structure
- `app/`: Contains the main application source code.
  - `pages/`: Application routes (e.g., `index.vue`, `create.vue`).
  - `layouts/`: Page layouts (e.g., `default.vue`).
  - `assets/css/`: Global stylesheets.
- `public/`: Static assets like favicons and robots.txt.
- `test/nuxt/`: Component and page tests using Vitest and Nuxt Test Utils.
- `nuxt.config.ts`: Nuxt configuration file.

## Development Conventions
- **Composition API**: Use `<script setup lang="ts">` for all Vue components.
- **Testing**: Every new feature or page should have a corresponding test in `test/nuxt/`. Use `mountSuspended` from `@nuxt/test-utils/runtime` for testing components in a Nuxt environment.
- **Styling**: Prefer updating `app/assets/css/main.css` for global styles and keeping components clean.
- **Icons**: Use `lucide-vue-next` for consistent iconography.

## Additional Coding preferences

- Do not use semmicolons for any Javascript/Typescript.
- Do not use Tailwind classes in component templates.
- Keep project dependencies minimal.
- Use relative importns and NOT a path alias.
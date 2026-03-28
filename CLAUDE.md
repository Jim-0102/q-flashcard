# q-flashcard

A multilingual math flashcard PWA built with Quasar (Vue 2).

## Dev Commands

```bash
yarn dev      # Start dev server
yarn build    # Build PWA (yarn build -m pwa --modern)
yarn lint     # ESLint (.js, .vue)
```

> `NODE_OPTIONS=--openssl-legacy-provider` is already set in scripts for Node 17+ compatibility.

## Tech Stack

- **Quasar v1** (Vue 2) — component framework and build tooling
- **vue-i18n v8** — i18n for en-us, zh-cn, zh-tw
- **PWA** — Workbox service worker via `quasar build -m pwa`
- **Cordova / Capacitor** — mobile targets (iOS/Android)

## Project Structure

```
src/
  pages/Index.vue      # Main flashcard/quiz page (core logic)
  layouts/MainLayout.vue
  boot/                # Quasar boot files (i18n init)
  i18n/                # en-us / zh-cn / zh-tw translations
  assets/              # Images and icons
  css/app.scss         # Global styles
```

## App Features

- **Flashcard mode** — flip cards to reveal answers
- **Quiz mode** — input answers, get immediate feedback
- **Challenge mode** — (see recent commits)
- **Operations** — addition, subtraction, multiplication, division, GCD
- Configurable operand ranges (max1, max2)

## Code Style

- ESLint with `plugin:vue/essential` + `standard`
- 2-space indent, LF line endings (see `.editorconfig`)
- No TypeScript — plain JavaScript (ES6+)

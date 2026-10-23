# Expo Mobile AI-Ready Kit

> Template mobile multiplataforma (iOS & Android) com **Expo SDK 52+**, **Expo Router**, **Clean Architecture**, **MVVM**, **Unistyles / Tamagui** e **Meta-Harness SDD** para desenvolvimento ágil com agentes de IA.

---

## Destaques da Arquitetura

- **Expo Router (File-Based Routing):** Navegação nativa via `app/` (tabs, stacks, modals).
- **Clean Architecture & MVVM:**
  - `src/features/[feature]/domain/`: Entidades e interfaces de repositório.
  - `src/features/[feature]/application/`: Casos de uso e DTOs (Zod).
  - `src/features/[feature]/infra/`: Repositórios HTTP (Axios/Ky) e SecureStore (tokens).
  - `src/features/[feature]/presentation/`: Telas e View-Models reativos.
- **Estilização de Alta Performance:** Unistyles ou Tamagui com design tokens compartilhados, modo escuro nativo e zero layout shift.
- **Preparado para Extensão:**
  - Push Notifications prontas com Expo Notifications + background tasks.
  - Armazenamento seguro de tokens com `expo-secure-store`.
  - Offline-first e cache com TanStack Query / WatermelonDB / MMKV.
  - Observabilidade e crash reporting integrados (Sentry React Native).

---

## O Meta-Harness (`.agent/` vs `.agents/`)

- `.agent/`: Meta-Harness interno do app com a Constituição Mobile (`system-prompt.md`) e regras em `rules/`.
- `.agents/`: Não conflita com CLIs externas de skills.

---

## Como usar como template

```bash
git clone https://github.com/wjuniorw/expo-mobile-ai-ready-kit.git meu-novo-app
cd meu-novo-app
pnpm install
pnpm run start
```

---

## Licença

MIT

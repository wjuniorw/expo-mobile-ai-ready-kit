# Meta-Harness: Automatic Agent Initialization (Expo Mobile)

When starting a session in this repository, you MUST process this file and register the following contexts without needing manual instruction from the developer:

## 1. Project Rules (Mobile Expo Constitution & Guidelines)
- Read **immediately** `.agent/system-prompt.md`. It contains the mobile architecture rules.
- Strictly follow mobile best practices:
  - Clean Architecture & DDD (`domain/`, `application/`, `infra/`, `presentation/`).
  - Feature-Sliced Design (FSD) and MVVM (`screens/`, `view-models/`, `components/`).
  - Expo Router (file-based navigation in `app/`).
  - Mobile Styling: Unistyles / Tamagui for cross-platform theme tokens and responsive layouts.
  - State Management: Zustand for shared/session state, view-models for screen state.
  - Push Notifications: Expo Notifications with proper token registration and background listeners.
  - Zero business logic inside React Native components.

## 2. Skill Registration & Conceptual Separation (.agent vs .agents)
- Scan and register in your context the skills available in `.agent/skills/`.
- **Important Conceptual Separation**:
  - `.agent/`: project-local architecture, SDD harness, and internal mobile domain skills.
  - `.agents/` / `.cursor/skills/`: external/third-party skills installed via community package managers.
- **TLC Spec-Driven Integration**:
  - Use `tlc-spec-driven` for structured feature implementation: `spec` -> `design` -> `tasks` -> `execute` -> `audit`.
  - Every mobile screen/component task MUST bind to the project's native skills.

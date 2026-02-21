
# Architecture Overview

## Monorepo Layout

offline-assistant/
  core/        → Rust shared logic
  apps/        → Desktop (Tauri), iOS, Android shells
  runtimes/    → llama.cpp builds
  policy/      → ethics configs
  packs/       → shared knowledge pack tooling
  docs/        → security + architecture documentation

## Core Components

### Inference Runtime
- llama.cpp GGUF models
- Desktop: 7–14B quant
- Mobile: 2–4B quant

### Conversation Engine
- Streaming chat
- Conversation memory
- Persona/system prompts

### Data Governor
- Capability-based mounts
- Explicit user permissions
- Full audit log

### Storage
- SQLCipher encrypted SQLite

### Ethics Module
- Rawlsian fairness scoring
- User-editable constitution

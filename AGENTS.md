# AGENTS.md — til (Today I Learned)

Guía para cualquier agente (Claude Code, Codex, Antigravity/Gemini, Copilot). Los puentes `CLAUDE.md`, `GEMINI.md` y `.github/copilot-instructions.md` apuntan a este archivo.

## Qué es

Colección de notas técnicas cortas (“today I learned”) sobre datos, Python y tooling. Repo público y minimalista: `notes/` contiene una nota por tema y el `README.md` es la presentación.

## Estructura

- `notes/` — notas en kebab-case (p. ej. `bash-strict-mode.md`, `git-worktree-add.md`, `bigquery-limit-does-not-cut-cost.md`).
- `README.md` — qué es el repo.

## Cómo trabajar acá

- Una nota = un aprendizaje concreto: contexto mínimo, ejemplo y por qué importa; archivos nuevos en `notes/` con nombre kebab-case.
- Título claro y prosa corta; sin relleno.
- Repo **público**: sin datos privados, credenciales ni material de clientes.
- Si el tema ya existe, mejor extender esa nota que duplicar.

## Estado

Colección estable; última actualización: 18/09/2026.

## Memoria de sesiones

- `memory/STATE.md` (foto del estado) y `memory/LOG.md` (historial *append-only*).
- Al cerrar una sesión con cambios: actualizar STATE, agregar la entrada en LOG y commitear; `scripts/scan_secrets.py` corre como hook pre-commit.

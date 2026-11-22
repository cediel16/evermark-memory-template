# Evermark memory repo

This repository is the memory of one person, kept by Evermark for their AI agents.
Every memory is a plain Markdown file in this repo, versioned by Git.

> Resumen en español: este repo guarda las memorias de una persona para sus agentes de IA.
> Cada memoria es un archivo Markdown dentro de una carpeta de proyecto. Lee `.evermark/index.md`
> para ver qué hay, y crea o cambia memorias siguiendo las reglas de abajo.

## How to read

1. Start with `.evermark/index.md`. It lists every project and the latest memories.
2. Open the project folder you need (for example `proyecto-ejemplo/`).
3. Read the files in `decisiones/`, `acciones/` and `notas/` as needed. Each file is self-contained.

## How to name files

- Put each memory in the folder of its project: `<project>/<kind>/<NNNN>-<short-slug>.md`.
- `<kind>` is one of: `decisiones` (decisions), `acciones` (actions taken or to take), `notas` (notes).
- `<NNNN>` is a four-digit number, increasing inside each folder: `0001`, `0002`, and so on.
- The slug is lowercase, uses hyphens and has no accents: `0003-cambio-de-proveedor.md`.

## Frontmatter

Every memory starts with this block:

```yaml
---
title: Short human title
type: decision | action | note
date: YYYY-MM-DD
---
```

- `title` is a short sentence.
- `type` must match the folder: `decisiones/` uses `decision`, `acciones/` uses `action`, `notas/` uses `note`.
- `date` is the day the memory was written.

## How to write

- One idea per file. If a memory grows into two topics, split it.
- Write the body in the language the person uses. Keep the frontmatter keys in English.
- Never edit the number or the slug of an existing memory. To correct one, add a new memory that says what changed, and link to the old file.
- Do not store secrets, passwords, tokens or personal data that the person has not asked to keep.

## Index

After you add or change a memory, update `.evermark/index.md` with one line per new file.

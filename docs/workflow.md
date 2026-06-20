# Workflow

## Task 1 — перший запит до агента

**Запит:** «прочитай AGENTS.md і опиши проєкт»

**Інструмент:** Claude Code (модель Claude Opus)

**Відповідь агента (контекст зчитано з `app/AGENTS.md`):**

> Це greenfield-застосунок на **Next.js 16.2.9** (App Router, Turbopack) з
> **React 19.2.4**, **TypeScript 5** і **Tailwind CSS 4**. Запускається на Node 22+.
>
> Структура: код застосунку — у теці `app/`; робочі команди — `npm run dev`
> (локальний запуск), `npm run build`, `npm run start`, `npm run lint`. Тести ще
> не налаштовані.
>
> Конвенції проєкту: функціональні компоненти у PascalCase, стилі лише через
> Tailwind, назви файлів kebab-case, тексти інтерфейсу українською, маленькі
> чисті функції.
>
> Guardrails: не чіпати `node_modules/`, `.next/` та білди; не комітити секрети
> й `.env*`; перед змінами коду показувати план і виконувати лише після
> погодження.

✅ Контекст зчитався: агент коректно переказав стек, команди, конвенції та
guardrails із `app/AGENTS.md`.

**Встановлений Agent Skill:** `vercel-react-best-practices`
(у `.agents/skills/`) — найкращі практики React/Next.js під цей стек.

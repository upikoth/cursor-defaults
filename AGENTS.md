# Инструкции для AI (Cursor)

## Рабочий процесс

1. **Требования по цепочке** — см. `.cursor/rules/requirements.mdc`: функциональный корпус → НФТ при необходимости → **architecture** (`docs/architecture/`, `.cursor/rules/architecture.mdc`, первичное создание — навык **`architecture-init`**) → код после явного подтверждения порции и опоры на утверждённые **FR**, **NFR** (если релевантно) и **архитектуру**.
2. **Доработка поведения** — обновление **`FR-{AREA}-{NNN}`** в `functional/` и подтверждение человека; отдельной папки карточек нет (`requirements.mdc`).
3. **Реализация** — Go-сервисы, затем Vue-приложения по задаче; в каждом каталоге — `backend.mdc` и `frontend.mdc`.
4. **Тесты** — создавай вместе с кодом (`.cursor/rules/testing.mdc`).

## Ссылки на правила

| Область      | Файл                               |
| ------------ | ---------------------------------- |
| Требования   | `.cursor/rules/requirements.mdc`   |
| Архитектура  | `.cursor/rules/architecture.mdc`   |
| Backend      | `.cursor/rules/backend.mdc`        |
| Frontend     | `.cursor/rules/frontend.mdc`       |
| Тесты        | `.cursor/rules/testing.mdc`        |
| База данных  | `.cursor/rules/database.mdc`       |

Тот же текст подключается в каждой сессии через `.cursor/rules/agents.mdc` (`alwaysApply: true`).

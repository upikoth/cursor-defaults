# Инструкции для AI (Cursor)

## Рабочий процесс

1. **Требования по цепочке** — см. `.cursor/rules/requirements.mdc`: при новом продукте или новой доменной области сначала **функциональный корпус** (`docs/requirements/functional/template.md`); затем **НФТ** при необходимости; затем **architecture** по согласованию с человеком; код — только после явного подтверждения порции работ и **опоры на утверждённые FR** из `functional/`.
2. **Доработка поведения** — обновление **`FR-{AREA}-{NNN}`** в `functional/` и подтверждение человека; отдельной папки карточек нет (`requirements.mdc`).
3. **Реализация** — backend → frontend. Строго следуй правилам из `backend.mdc` и `frontend.mdc`.
4. **Тесты** — создавай вместе с кодом (`.cursor/rules/testing.mdc`).

## Ссылки на правила

| Область     | Файл                             |
| ----------- | -------------------------------- |
| Требования  | `.cursor/rules/requirements.mdc` |
| Backend     | `.cursor/rules/backend.mdc`      |
| Frontend    | `.cursor/rules/frontend.mdc`     |
| Тесты       | `.cursor/rules/testing.mdc`      |
| База данных | `.cursor/rules/database.mdc`     |

Тот же текст подключается в каждой сессии через `.cursor/rules/agents.mdc` (`alwaysApply: true`).

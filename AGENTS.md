# Инструкции для AI (Cursor)

## Рабочий процесс

1. **Требования по цепочке** — см. `.cursor/rules/requirements.mdc`: при новом продукте или новой доменной области сначала **функциональный корпус** (`docs/requirements/functional/template.md`); затем **НФТ** при необходимости (`docs/requirements/non-functional/template.md`); затем **architecture** по согласованию с человеком; код — только после явного подтверждения порции работ и **опоры на утверждённые FR** (и утверждённые **НФТ**, если порция затрагивает зафиксированные свойства качества) из соответствующих папок `requirements/`.
2. **Доработка поведения** — обновление **`FR-{AREA}-{NNN}`** в `functional/` и подтверждение человека; отдельной папки карточек нет (`requirements.mdc`).
3. **Реализация** — Go-сервисы, затем Vue-приложения по задаче; в каждом каталоге — `backend.mdc` и `frontend.mdc`.
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

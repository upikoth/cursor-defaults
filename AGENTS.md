# Инструкции для AI (Cursor)

## Рабочий процесс

1. **Новая фича** — всегда начинай с `.cursor/rules/requirements.mdc`: задай уточняющие вопросы, заполни шаблон в `docs/requirements/features/`, дождись подтверждения пользователя.
2. **Реализация** — backend → frontend. Строго следуй правилам из `backend.mdc` и `frontend.mdc`.
3. **Тесты** — создавай вместе с кодом (`.cursor/rules/testing.mdc`).

## Ссылки на правила

| Область     | Файл                             |
| ----------- | -------------------------------- |
| Требования  | `.cursor/rules/requirements.mdc` |
| Backend     | `.cursor/rules/backend.mdc`      |
| Frontend    | `.cursor/rules/frontend.mdc`     |
| Тесты       | `.cursor/rules/testing.mdc`      |
| База данных | `.cursor/rules/database.mdc`     |

Тот же текст подключается в каждой сессии через `.cursor/rules/agents.mdc` (`alwaysApply: true`).

# Карта design-harness

## Передача между этапами

| Путь | Назначение |
| --- | --- |
| [input/HANDOFF_FROM_RESEARCH.md](input/HANDOFF_FROM_RESEARCH.md) | Вход из исследования (Git 1 → Git 2). Цель, доказательства, сценарии и критерии приёмки. |
| [output/figma-tokens.json](output/figma-tokens.json) | Выход дизайн-аудита (Git 2 → Git 3). DTCG-выгрузка токенов, нужных реализации. |
| [output/SPECS_FOR_DEV.md](output/SPECS_FOR_DEV.md) | Выход дизайн-аудита (Git 2 → Git 3). Проверенные фреймы, поведение и критерии реализации. |

## Правила

| Файл | Зачем открывать |
| --- | --- |
| [AGENTS.md](AGENTS.md) | Маршрут работы и пять золотых принципов. |
| [rules/tokens-summary.md](rules/tokens-summary.md) | Имена семантических Variables для подбора привязок. |
| [rules/tokens-dtcg.json](rules/tokens-dtcg.json) | Полный источник значений. Точечная сверка через Figma MCP или компиляция токенов. |
| [rules/figma-styles.md](rules/figma-styles.md) | Коллекции, Text Styles, привязки и библиотечные зависимости. |
| [rules/ux-heuristics.md](rules/ux-heuristics.md) | Визуальные правила, 10 эвристик Нильсена, плотность, состояния и зоны тапа. |
| [rules/ux-patterns.md](rules/ux-patterns.md) | Помощник, панель показателей, обзор пульса, отчёт и навигация. |
| [rules/figma-discipline.md](rules/figma-discipline.md) | Auto Layout, именование, Variables, Text Styles и библиотека. |

## Навыки

| Файл | Зачем открывать |
| --- | --- |
| [.skills/figma-make-brief/SKILL.md](.skills/figma-make-brief/SKILL.md) | Подготовка брифа для Make и перепривязка результата в Figma Design. |
| [.skills/figma-mcp-build/SKILL.md](.skills/figma-mcp-build/SKILL.md) | Сборка фреймов через MCP с проверяемыми привязками. |
| [.skills/design-audit/SKILL.md](.skills/design-audit/SKILL.md) | Проверка макета и заполнение пары выходных файлов. |

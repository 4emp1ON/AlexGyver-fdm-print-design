# fdm-print-design — скилл для Claude Code

Скилл для [Claude Code](https://claude.com/claude-code): как проектировать детали под FDM 3D-печать так,
чтобы они печатались на любом нормальном принтере на стандартных настройках, без поддержек, и переживали
типичные дефекты печати.

Основа — конспект своими словами видео **AlexGyver «📐Проектирование моделей под 3D печать»**
(https://youtu.be/Tvy8dkh3nPI), дополненный приёмами, отработанными на практике: разрезные кольца
со звёздочкой, клипсы-защёлки, колпачки, поворотные узлы с потайным крепежом.

> Неофициальный проект, не связан с AlexGyver. Все идеи видео — его; ошибки конспекта — наши.

## Что внутри

| Файл | Содержание |
|---|---|
| `SKILL.md` | Порядок работы, принципы (ориентация, стенки и рёбра, скругления/фаски, отверстия-капли, податливые посадки, крепёж, стыки корпусов, печать без поддержек, безопасность) и чек-лист перед печатью |
| `references/build123d-recipes.md` | Рецепты на [build123d](https://github.com/gumyr/build123d): капля, разрезное кольцо, киль «ласточкин хвост», кольцо в клетке, скруглённые перемычки, потай, коническая крыша, проверки |

## Установка

```bash
git clone https://github.com/4emp1ON/AlexGyver-fdm-print-design.git ~/.claude/skills/fdm-print-design
```

Для проекта, а не для всего пользователя — клонируйте в `.claude/skills/fdm-print-design` внутри проекта.
Claude Code подхватит скилл автоматически, когда речь зайдёт о деталях для 3D-печати.

## English

A Claude Code skill with design-for-FDM rules (orientation vs. load, walls over infill, fillets/chamfers,
teardrop holes, compliant fits, fasteners, support-free geometry) and build123d recipes. Based on a summary
of AlexGyver's video on designing models for 3D printing, plus techniques refined in practice.
Content is in Russian. Install: `git clone https://github.com/4emp1ON/AlexGyver-fdm-print-design.git ~/.claude/skills/fdm-print-design`.

# Портфолио демо-сайтов — правила для облачной сессии Claude

Это опубликованная копия портфолио (GitHub Pages): https://yusuframasanov-coder.github.io/portfolio/
Сайты: `demos/yurist/` («Параграф»), `demos/prokat/` («Перевал»), `demos/fond/` («Рядом»), `demos/doverennost/` («Бланк»), главная — `index.html`.

## Правила
- Общение и тексты — только по-русски.
- Любая правка — в отдельной ветке + Pull Request. НЕ пушить в main: слияние в main = публикация сайта, его делает только Юсуф.
- Ничего не удалять без явного «да».
- Чистый HTML/CSS/JS, по одному файлу на сайт, без сборщиков. Шрифты — Google Fonts, значки — встроенные SVG.
- Без изображений людей (особенно женщин) и без музыки — нормы Ислама.
- Компании вымышлены; в подвале остаётся пометка «Демо-проект». Контакты — заглушки +7 900 000-00-00, домены `.example`.
- Формы: согласие на обработку ПДн (152-ФЗ), галочка не стоит по умолчанию.
- Внешний вид: один акцент, без градиентов, свечения и эмодзи, отступы кратны 4.
- Перед PR — агент qa-tester (адаптив 360/768/1280, ссылки, формы, опечатки).
- В описании PR: что изменено и в каких файлах.

Агенты: `.claude/agents/` — brief-analyst, copywriter, ui-designer, frontend-dev, seo-specialist, integrations, legal-compliance, qa-tester, deploy-ops (ничего без «да»), client-support.

## Облачная сессия: навыки и общие правила (с 22.11.2026)
- Навыки (в том числе автотестировщик `qa-autotest`) и общие правила хранятся в приватном репозитории GitHub `yusuframasanov-coder/claude-config`. Обычно скрипт настройки облачного окружения сам запускает его `install.sh`.
- Запасной путь — в начале облачной сессии (claude.ai/code), если нет файла `~/.claude/skills/qa-autotest/branch.sh`: подключить репозиторий `claude-config` (инструмент add_repo; если его нет — `git clone https://github.com/yusuframasanov-coder/claude-config ~/claude-config`), затем `bash <папка claude-config>/install.sh`. После этого общие правила лежат в `~/.claude/CLAUDE.md`, автотестировщик — в `~/.claude/skills/qa-autotest`; прочитать `~/.claude/CLAUDE.md`.
- Правка навыка или общих правил — только в репозитории `claude-config` (ветка → Pull Request), не в `~/.claude` напрямую.

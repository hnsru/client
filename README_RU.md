[English](README.md) | **Русский**

# HNSRU Client (x64)

Кастомный 64-битный клиент для Counter-Strike 1.6 (HNS / KZ / Surf) с интерфейсом Tactical Glass Visor, split-loop движком, Reflex-Lite и встроенным автообновлением.

- **Страница загрузок и список изменений:** https://hnsru.github.io/client/
- **История изменений:** [CHANGELOG_RU.md](CHANGELOG_RU.md)
- **Полный обзор возможностей и настроек:** [docs/ANNOUNCEMENT_RU.md](docs/ANNOUNCEMENT_RU.md)
- **Релизы:** https://github.com/hnsru/client/releases

## Установка

1. Скачайте актуальный [`hnsru.exe`](https://github.com/hnsru/client/releases/latest/download/hnsru.exe) со страницы Releases.
2. Поместите `hnsru.exe` в корневую папку с установленной Half-Life / Counter-Strike 1.6 (рядом с `hl.exe` и папкой `cstrike`).
3. Запустите `hnsru.exe` при запущенном Steam.

## Каналы автообновления

| Канал | Как включить | Поведение |
|---|---|---|
| **Release** (по умолчанию) | Обычный запуск `hnsru.exe` | Автопроверка при запуске и во время работы. На главном экране обновляется и перезапускается автоматически; во время игры показывает плашку `CLIENT OUTDATED` сверху по центру. |
| **Beta** | Параметр запуска `-beta` | Подключает тестовые сборки из beta-канала (флаг `-beta` сохраняется после автоперезапуска). |

В главном меню или в игре можно в любой момент открыть окно последнего патчноута консольной командой `hnsru_changelog`.

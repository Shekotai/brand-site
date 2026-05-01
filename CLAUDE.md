# Контекст проекта — ARMOR DETAILING

## Окружение пользователя (macOS)
- **Homebrew** установлен (`/opt/homebrew`)
- **GitHub CLI (`gh`)** установлен и авторизован под `Shekotai`
- **Git push работает** — авторизация настроена через `gh auth login`
- Терминал: zsh

## Репозиторий
- GitHub: https://github.com/Shekotai/brand-site
- Основная ветка: `main`
- Push напрямую в main работает: `git push origin <branch>:main`

## Деплой
- Хостинг: **Vercel** (подключён к GitHub)
- Деплой автоматический — после push в `main` Vercel пересобирает сайт за ~30 секунд
- Не нужно ничего настраивать вручную: коммит → push → готово

## Структура проекта
- `index.html` — основной файл сайта (single-page, всё внутри: HTML + CSS + JS)
- `armor-detailing-standalone.html` — standalone-версия
- `assets/` — медиа-файлы

## Дизайн-система
Используется **LCG Communities | Bold Architecture**.

Основные токены:
- Primary (акцент): `#E74C3C` (красный)
- Neutral: `#111111`
- Background: `#F4F4F4`
- Tertiary: `#EECA3F`
- Border-radius: `0px` — все углы квадратные
- Шрифты: Manrope (display), Inter (body), JetBrains Mono (mono)
- Кнопки: фон `#111111`, текст `#F4F4F4`, padding 16px, без радиуса

## Правила работы с пользователем
- Пользователь — **новичок** в коде/терминале → объяснять простыми пошаговыми инструкциями
- При просьбе «залить на сайт» / «задеплоить»:
  1. `git add <файл>`
  2. `git commit -m "..."`
  3. `git push origin <текущая-ветка>:main`
  4. Vercel сам подхватит деплой
- НЕ нужно настраивать GitHub Pages, токены, SSH — всё уже работает

# Портфолио

Одностраничная визитка: `index.html` + `styles.css`, без сборки, зависимостей и внешних CDN.

## Что заменить перед публикацией

| Место | Что заменить |
| :--- | :--- |
| `index.html`, блок `#contact` | `https://t.me/your_telegram` → ваш Telegram |
| `index.html`, блок `#contact` | `you@example.com` → ваша почта |
| `index.html`, `<footer>` | год и имя, если нужно |

Ссылки на репозитории уже указывают на `github.com/Hopfi3721/...`. Если репозиторий
ещё не опубликован — ссылка будет вести в 404, поэтому публикуйте кейсы первыми.

## Локальный просмотр

Просто открыть `index.html` в браузере.

## Публикация на GitHub Pages

Вариант 1 — отдельный репозиторий `Hopfi3721.github.io` (адрес будет `https://hopfi3721.github.io`):

```powershell
cd C:\Users\admin\SiteMaking\portfolio
git init -b main
git add .
git commit -m "portfolio: one-page site with three cases"
gh repo create Hopfi3721.github.io --public --source=. --push
```

Через минуту сайт доступен по адресу `https://hopfi3721.github.io`.
В `Settings → Pages` должен быть выбран источник `Deploy from a branch`, ветка `main`, папка `/ (root)`.

Вариант 2 — папка `docs/` в любом существующем репозитории, источник Pages → `/docs`.

## Проверка перед отправкой ссылки заказчику

- [ ] открывается на телефоне (ширина 375 px)
- [ ] все три ссылки на GitHub живые
- [ ] Telegram и почта заменены на настоящие
- [ ] в описании кейса нет обещаний, которых проект не выполняет

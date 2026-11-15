# Docs — документация проекта Parts Unlimited

Репозиторий для ЛР 1.2 (задачи 2 и 3): документация хранится как код в папке `docs/`
и публикуется на GitHub Pages конвейером `.github/workflows/pages.yml`.

| Azure DevOps | Здесь |
| --- | --- |
| «Publish code as wiki» | GitHub Pages + MkDocs, сборка при каждом push в `main` |
| Заголовок страницы из имени файла | MkDocs берёт заголовок из первого `#`-заголовка или из имени файла |
| Файл `.order` | Файл `.pages` (плагин `mkdocs-awesome-pages-plugin`) |
| Публикация другой ветки | Поменять ветку в `on.push.branches` workflow |

Локальный просмотр:

```bash
python -m pip install -r requirements.txt
mkdocs serve        # http://127.0.0.1:8000
```

Включение публикации: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

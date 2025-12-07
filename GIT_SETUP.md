# Инструкция по подключению к GitHub

## Если Git не установлен:
1. Скачайте и установите Git: https://git-scm.com/download/win
2. Перезапустите терминал после установки

## Команды для подключения к репозиторию:

```bash
# Перейдите в папку проекта
cd "c:\Users\I1\Desktop\frontend"

# Инициализируйте git (если еще не инициализирован)
git init

# Добавьте remote репозиторий
git remote add origin https://github.com/van2011/math-tutor-landing.git

# Проверьте подключение
git remote -v

# Добавьте все файлы
git add .

# Сделайте первый commit
git commit -m "Initial commit: landing page with form integration"

# Если в репозитории уже есть файлы, сначала получите их
git pull origin main --allow-unrelated-histories

# Отправьте изменения на GitHub
git push -u origin main
```

## Если возникнут конфликты:

Если в репозитории уже есть файлы (README.md, index.html), и они отличаются от ваших:

```bash
# Сначала получите файлы из репозитория
git pull origin main --allow-unrelated-histories

# Разрешите конфликты вручную (если они есть)
# Затем добавьте файлы снова
git add .

# Сделайте commit
git commit -m "Merge with remote repository"

# Отправьте изменения
git push -u origin main
```

## Для последующих обновлений:

```bash
git add .
git commit -m "Описание изменений"
git push
```


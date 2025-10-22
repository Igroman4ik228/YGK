# YGK

## Основные команды Git

---

### Настройка

```
git config --global user.name "My Name"          # Установить имя пользователя
git config --global user.email myEmail@example.com  # Установить email
git config --list                                # Просмотреть текущие настройки
git config --global color.ui true                # Включить цветной интерфейс
git config --global color.status auto            # Цветное отображение статуса
git config --global color.branch auto            # Цветное отображение веток
```

---

### Создание и состояние репозитория

```
git init                                         # Инициализация нового репозитория
git status                                       # Проверить текущее состояние файлов
```

---

### Подготовка и фиксация изменений

```
git add hello.txt                                # Добавить файл в индекс
git add -A                                       # Добавить все изменения (новые, изменённые, удалённые файлы)
git add .                                        # Добавить всё из текущей папки
git reset css/style.css                          # Убрать файл из индекса
git commit -m "Add some code"                    # Зафиксировать изменения с комментарием
```

---

### Просмотр истории и изменений

```
git log                                          # Просмотр истории коммитов
git show <hash_commit>                           # Просмотр деталей конкретного коммита
git commit --amend -m "Новый комментарий"        # Изменить последний коммит
git diff <hash1>..<hash2>                        # Сравнить два коммита
```

---

### Работа с удалённым репозиторием

```
git clone https://github.com/user/project        # Клонировать удалённый репозиторий
git clone https://github.com/user/project folder # Клонировать в другую папку
git remote add origin https://github.com/user/project.git  # Добавить удалённый репозиторий
git push origin master                           # Отправить изменения на сервер
git pull origin master                           # Получить изменения с сервера
```

---

### Ветвление

```
git branch amazing_new_feature                   # Создать новую ветку
git branch                                       # Просмотреть список веток
git checkout amazing_new_feature                 # Перейти в другую ветку
git merge amazing_new_feature                    # Слить ветку с текущей
git branch -d local_branch_name                  # Удалить локальную ветку
git checkout -b <branch> origin/<branch>         # Создать локальную ветку из удалённой
```

---

### Откат и восстановление

```
git checkout <commit_hash> <file>                # Восстановить файл из старого коммита
git revert HEAD                                  # Отменить последний коммит (создаётся новый)
git revert <commit_hash>                         # Отменить конкретный коммит
git mergetool                                    # Визуально решить конфликт при слиянии
```

---

Хочешь, я сделаю из этого удобную шпаргалку в формате PDF или Markdown?

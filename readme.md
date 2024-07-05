# 1. Инициализация проекта
```bash
cd ~				# переходим в родительский уровень папки  
mkdir -p dev/starting-git	# создаем папку  
cd dev/starting-git/		# переходим в папку для работы с git  
git init			# инициализация локальной git  
```


# 2. Добавляем readme.md
```bash
touch readme.md			# создаем файл  
nano readme.md			# вставляем этот текст в файл и сохраняем  
```


# 3. Добавляем файлы в репозиторий и коммит!
```bash
git add .			# добавляем все  
git add --all			# или так  
git add readme.md		# или конкретный файл  
git commit -m "Создание шпаргалки по GIT"	# Сохраняем все файлы в локальный репозиторий  
git status			# проверить состояние коммита
```


# 4. Просматриваем историю коммитов
```bash
git log
```


# 5. Начнем работать с GitHub, а так же генерируем SSH-ключ
Много буков, см. курсы на Яндекс.Практикум
1. [GitHib](https://practicum.yandex.ru/trainer/git-basics/lesson/f7e00d04-1da2-46b4-b13d-b0bf751caf88/)
2. [SSH](https://practicum.yandex.ru/trainer/git-basics/lesson/42435683-0922-4231-bfb4-d7d32d61f50a/)


# 6. Создаём удалённый репозиторий
1. Заходим в свой профиль  
[https://github.com/lvorobjeff](https://github.com/lvorobjeff) (где lvorobjeff - моя профиль)
2. Создаем удаленный репозиторий:  
[https://github.com/lvorobjeff?tab=repositories](https://github.com/lvorobjeff?tab=repositories) --> New
3. Привязаем удаленный к локальному (используем готовый скрипт после создания, берем где SSH):
```bash
git remote add origin git@github.com:lvorobjeff/starting-git.git
git branch -M main
git push -u origin main		# опубликовать все локальные коммиты
```
4. Убедиться, что репозитории связаны
```bash
git remote -v
```



 # Подсказка по GIT

## Создание репозитория
Cоздает новый репозиторий Git. С ее помощью можно преобразовать существующий проект без управления версиями в репозиторий Git или инициализировать новый пустой репозиторий. Большинство остальных команд Git невозможно использовать без инициализации репозитория, поэтому данная команда обычно выполняется первой в рамках нового проекта.
```
git init 
  ```
 Добавляет изменение из рабочего каталога в раздел проиндексированных файлов. Она сообщает Git, что вы хотите включить изменения в конкретном файле в следующий коммит. Однако на самом деле команда git add не оказывает существенного влияния на репозиторий: изменения регистрируются в нем только после выполнения команды git commit.

 ```sh
 git add 
 ```
  Фиксирует изменения в репозитории. Когда пользователь использует ее, создается «снимок» (коммит) текущего состояния проекта, включая все внесенные изменения. Каждое такое сохранение имеет уникальный идентификатор, который позволяет отслеживать историю изменений в проекте.
  ```sh
 gid commit -m "Massage text" 
 ```
 
 Для просмотра истории проекта, чтобы узнать, кто и что сделал, выяснить, откуда появились баги, и отменить изменения, вызвавшие проблемы: 
 ```sh
 git log  
 ```
Для отображение  коммитов в укороченном виде: 

```sh
 git log --oneline 
```
 Команда, которая позволяет разработчикам переключаться между ветками, перемещаться по коммитам, восстанавливать файлы из предыдущих состояний:

  ```sh
 git checkout <имя_ветки>
```

Отображение всех веток
``` sh
git branch

```
Создание новой ветки
```sh
git branch <имя_ветки>
```
Удаление ветки
```sh
git branch -d <имя_ветки>
```
Команда для просмотра всех созданных commit
```sh
git --graph
```

# Работа c удаленным репозиторием

Команда для вставки удаленного репозитория (с GitHab)
```sh
git clone <ссылка>
```

Команда для добавления на GitHab своего репозитория
```sh
git push
```

Команда для добаления с GitHab и слияния удаленного в локальный репозиторий
```sh
git pull
```

Кнопка для копирования чужого репозитория в свой на GitHab
```sh
FORK
```


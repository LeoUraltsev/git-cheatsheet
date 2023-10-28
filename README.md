# Шпаргалка по работе с GIT

## Инициализация репозитория

`git init` - Команда для инициализации репозитория.  
`git status` - Команда для проверки статуса или состояния репозитория

При ошибочной инициализации репозитория, можно её «разгитить». Для этого нужно удалить скрытую подпапку `.git`  

Важное про инициализацию:    
- Инициализация Git-репозитория требует добавления файлов.
- Текстовые файлы часто используются для хранения кода, но Git может быть полезен для других типов файлов.
- Команда `git status` показывает статус изменений в репозитории.
- `git add` запоминает текущее содержимое файла, но не сохраняет его в репозитории.
- Коммит (фиксация состояния файлов) сохраняет текущее состояние файла.
- Команда `git add --all` подготавливает к сохранению все файлы в репозитории.
- `git add .` позволяет добавить текущую папку со всеми файлами.

## Commit

**Коммит в Git** - это сохранение изменений в истории и возможность "откатиться" к предыдущим версиям.

`git commit` - команда для выполнения коммита. При добавлении коммита также нужно указать сообщение об изменениях.

Пример:

``` $ git commit -m "Initial commit" ```

Важно:
- После выполнения коммита текущая версия файлов сохраняется в репозитории с указанным сообщением.
- Коммиты хранятся в ветках. Начальная ветка создаётся автоматически и называется `main` или `master`.
- Команда `git commit` выводит информацию о коммите, включая коммит-идентификатор, количество измененных файлов и их тип.
- Разница между `git add` и `git commit`: `git add` - сохраняет файлы, а `git commit` сохраняет и сохраняет изменения.
- Рекомендуется описывать коммит информативно, чтобы было понятно, какие изменения были сделаны.

## Просмотр истории коммитов

Команда для просмотра истории коммитов - `git log`

`git log --oneline` - получить сокрашенный лог. (В сокращённом логе выводятся сокращённые хеши — их можно использовать точно так же, как и полные.)

## Push

За отправку изменений на удалённый репозиторий отвечает команда - `git push`.

Примеры команды:  
* При первом вызове:  
``` $ git push -u origin master ```
* При повторном вызове:   
``` $ git push ```

`origin` - это название по умолчанию для удалённого сервера.  
`master` или `main` - ветка в которую отправляются изменения.


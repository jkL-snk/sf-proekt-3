# Документация по работе с репозиторием кода

## где располагается репозиторий с кодом, как посмотреть существующий код

Репозиторий распологается на сервисе Github по адресу https://github.com/jkL-snk/sf-proekt-3 
Основная ветка master

## как устроен процесс внесения своих изменений в основную кодовую базу

Работа с кодом ведется на основе модели Github flow: https://guides.github.com/introduction/flow/

Для внесений изменений требуется создать отдельную ветку с наименованием соответствующим тикету в тикет-системе c добавлением краткой сути работы в ветке:

```
git checkout -b 'SF3-1234-fix-auth-bug'
```

Все изменения разбиваются на коммиты. После выполнения работ в ветке выполняется Pull Request. Также Pull request можно выполнять для получения помощи и консультаций используя меншены @mention для упоминания конкретных людей из команды.

```
git commit -m 'fixed auth bug'
```

## как настроить свою среду разработки

Для начала нужно скопировать себе лежащий в репозитории .gitconfig
Затем нужно ввести свои данные:

```
git config user.name ivan.ivanov
git config user.email ivanov@example.com
```

Для примера настройки среды разработки возьмем VSCode:

Нажать CTRL+SHIFT+G для перехода в режим управления кодом, в меню выбрать "удаленный", "добавить удаленные репозиторий", приложение откроет браузер, нужно будет авторизоватся в Github и указать репозиторий для работы.
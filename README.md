# CRM - Система управления контактными данными клиентов.

## Описание
CRM разработана в соответствии с полученным ТЗ. База данных клиентов хранится на сервере. Произведена настройка REST API.
Краткая схема работы: 
`Запрос на сервер(request)` --> `Получение массива клиентов, в соответствии с запросом(response)` --> `Отрисовка таблицы`

Табличная часть приложения генерируется на JS. Реализован поиск и сортировка; создание, редактирование и удаление клиентов из БД. Верстка выполнена в соответсвии с выданным макетом. Применен компонентный подход, некое подобие [Factory Method Pattern](https://refactoring.guru/ru/design-patterns/factory-method): создан аккумулирующий класс, все остальные компоненты наследуются от него, тем самым создавая возможность расширения\маштабирования приложения при необходимости. В рамках технического задания реализован всего один такой компонент - Таблица(Table).

Из сторонних библиотек использованы: [choices](https://github.com/Choices-js/Choices) - для стилизации Select'ов и [Tippy.js](https://atomiks.github.io/tippyjs/) - для использования Tooltip'ов.

Использован Webpack (babel, eslint)


<img src="https://github.com/SolodovnikViktor/CRM-coin/blob/main/preview/login.png" width=35% height=35%>
<img src="https://github.com/SolodovnikViktor/CRM-coin/blob/main/preview/accounts.png" width=35% height=35%>
<img src="https://github.com/SolodovnikViktor/CRM-coin/blob/main/preview/account.png" width=35% height=35%>
<img src="https://github.com/SolodovnikViktor/CRM-coin/blob/main/preview/banks.png" width=35% height=35%>
<img src="https://github.com/SolodovnikViktor/CRM-coin/blob/main/preview/currency.png" width=35% height=35%>
# CRM-coin

## Для запуска
* скачать репозиторий
* открыть IDE 
* Для установки пакетов открыть терминал в папке с проектом, выполнить:

With [NPM](https://www.npmjs.com/package/choices.js):

```zsh
npm install
```

With [Yarn](https://yarnpkg.com/):

```zsh
yarn add
```
* Для запуска сервера
```zsh
npm start
```





# HTTP methods

> Данная тема является обязательной к изучению. {style="warning"}

HTTP определяет множество **методов запроса**, которые указывают, какое желаемое действие выполнится для данного ресурса. 
Несмотря на то, что их названия могут быть существительными, эти методы запроса иногда называются _HTTP глаголами_. 
Каждый реализует свою семантику, но каждая группа команд разделяет общие свойства: так, методы могут быть безопасными, 
[идемпотентными](https://developer.mozilla.org/ru/docs/Glossary/Idempotent) или 
[кешируемыми](https://developer.mozilla.org/ru/docs/Glossary/Cacheable). 
Идентопотентные и кешируемые. Безопасные методы - это которые не изменя.т состояние сервера.

- Метод [`GET`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/GET) запрашивает представление ресурса. 
Запросы с использованием этого метода могут только извлекать данные.

- Метод [`HEAD`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/HEAD) запрашивает ресурс так же, как и метод GET, но без тела ответа.

- Метод [`POST`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/POST) используется для отправки сущностей к определённому ресурсу. 
Часто вызывает изменение состояния или какие-то побочные эффекты на сервере.

- Метод [`PUT`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/PUT) заменяет все текущие представления ресурса данными запроса.

- Метод [`DELETE`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/DELETE) удаляет указанный ресурс.

- Метод [`CONNECT`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/CONNECT) устанавливает "туннель" к серверу, определённому по ресурсу.

- Метод [`OPTIONS`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/OPTIONS) используется для описания параметров соединения с ресурсом.

- Метод [`TRACE`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/TRACE) выполняет вызов возвращаемого тестового сообщения с ресурса.

- Метод [`PATCH`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/PATCH) используется для частичного изменения ресурса.

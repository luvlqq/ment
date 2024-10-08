# HTTP headers

> Данная тема является обязательной к изучению. {style="warning"}

**HTTP** (Hypertext Transfer Protocol) заголовки представляют собой метаданные,
передаваемые в запросах и ответах между веб-клиентами и серверами.
Эти заголовки содержат информацию о запросе, ответе и о данных, которые передаются между клиентом и сервером.
Заголовки являются важной частью протокола HTTP и используются для различных целей, таких как управление кэшированием,
обработка сессий, безопасность и другие.

Вот несколько типичных HTTP-заголовков:

### 1. **Общие заголовки:**

- **Cache-Control:** Управляет кэшированием, указывая, как кешировать или как не кешировать ресурс.
- **Date:** Дата и время, когда запрос был отправлен или ответ был сгенерирован.
- **Connection:** Управляет соединением между клиентом и сервером. Например, значение "keep-alive" позволяет
  использовать одно соединение для нескольких запросов.
- **Content-Length:** Размер тела ответа в байтах.
- **Content-Type:** Тип данных в теле запроса или ответа, например, "text/html" или "application/json".

### 2. **Заголовки запроса:**

- **Host:** Доменное имя и порт сервера, к которому отправляется запрос.
- **User-Agent:** Информация о веб-браузере или другом клиенте, отправляющем запрос.
- **Accept:** Типы медиа-ресурсов, которые клиент может принять, например, "text/html" или "application/json".
- **Authorization:** Данные для аутентификации, такие как токен или имя пользователя/пароль.

### 3. **Заголовки ответа:**

- **Status Code:** Код состояния ответа, например, 200 OK или 404 Not Found.
- **Server:** Информация о сервере, который генерирует ответ.
- **Location:** Используется для перенаправления клиента на другой ресурс.
- **Set-Cookie:** Устанавливает куки на стороне клиента, что позволяет серверу отслеживать состояние сессии.

### 4. **Заголовки сущности:**

- **Strict-Transport-Security:** Устанавливает политику безопасности, требуя использование HTTPS для всех последующих
  запросов.
- **X-Content-Type-Options:** Предотвращает атаки типа MIME sniffing, указывая браузеру не изменять тип контента.
- **Content-Security-Policy:** Определяет, какие ресурсы могут быть загружены на страницу.
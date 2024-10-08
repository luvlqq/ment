# HTTP versions

> Данная тема является обязательной к изучению. {style="warning"}

Протокол **HTTP** (Hypertext Transfer Protocol) является основой передачи данных в Интернете. С течением времени он прошел через несколько версий, каждая из которых внесла улучшения и новые возможности. Вот краткий обзор различных версий HTTP:

### 1. **HTTP/0.9:**

- Первая версия HTTP, введенная Тимом Бернерсом-Ли в 1989 году.
- Поддерживала только метод `GET`, который позволял получать HTML документы с веб-сервера.

### 2. **HTTP/1.0:**

- Введена в 1996 году.
- Поддерживались методы `GET`, `POST` и другие.
- Поддержка различных типов документов и заголовков.
- Каждый запрос от клиента и ответ от сервера требовали отдельного соединения.

### 3. **HTTP/1.1:**

- Введена в 1997 году.
- Решила множество проблем HTTP/1.0, включая использование одного соединения для нескольких запросов (keep-alive), что улучшило производительность.
- Поддержка пайплайнинга (pipelining) позволяет отправлять несколько запросов без ожидания ответа от предыдущего.
- Введение различных методов кеширования для улучшения производительности и снижения нагрузки на серверы.

### 4. **HTTP/2:**

- Введена в 2015 году.
- Более эффективная передача данных, сжатие заголовков и данных.
- Мультиплексирование (Multiplexing) позволяет отправлять несколько запросов и ответов в одном TCP-соединении, снижая задержки.
- Поддержка приоритетов запросов, что позволяет оптимизировать загрузку ресурсов.

### 5. **HTTP/3:**

- Начата разработка в 2018 году, в основном из-за ограничений TCP в условиях высоких задержек и потерь данных.
- HTTP/3 использует протокол QUIC (Quick UDP Internet Connections) вместо TCP для установления соединения, что уменьшает задержки и повышает производительность.
- Поддерживает мультиплексирование, сжатие данных и передачу данных в виде потока.

1. **HTTP/0.9**: Очень простая структура. Только метод GET. Отсутствие заголовков. Отсутствие сеансов( "keep-alive").
2. **HTTP/1.0**: Поддержка различных методов (GET, POST, HEAD), заголовков запроса и ответа, а также статусы ответов сервера (коды состояния). Отсутствие сеансов( "keep-alive").
3. **HTTP/1.1**: Поддержка статуса "keep-alive", поддержка кеширования, разделение заголовков на разрешенные и пользовательские заголовки, а также поддержка диапазонов запросов и сжатия данных.
4. **HTTP/2.0**: Оптимизации для более быстрой передачи данных. Механизмы мультиплексирования( разделение передаваемой информации между двумя и более каналами ). Также вводится сжатие заголовков, приоритизация запросов и другие оптимизации.  
5. **HTTP/3.0**: Эта версия представляет протокол QUIC (Quick UDP Internet Connections), который базируется на протоколе UDP вместо TCP. Он предназначен для улучшения производительности, особенно в условиях низкой задержки и потерь пакетов. HTTP/3 включает улучшенное управление соединением и более надежную передачу данных.
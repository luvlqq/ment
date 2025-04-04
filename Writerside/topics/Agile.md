# Agile

**Методологии разработки программного обеспечения** - это структурированные подходы к созданию программного обеспечения.

Они определяют как мы планируем, создаем, тестируем и реализуем программный проект.

**SDLC** - software development life cycle. (это виды, которые ниже)

## Виды:

### WATERFALL

> Для ознакомления {style="note"}

Последовательная модель в которой каждый этап зависит от предыдущего. Она систематична и имеет определенные цели для
каждого этапа, но не обладает гибкостью для внесения изменений после завершения этапа.

### V-Model

> Для ознакомления {style="note"}

Линейный подход при котором каждому этапу соответствует этап тестирования. Он подчеркивает важность валидации и
верификации.

### Итерационная

> Для ознакомления {style="note"}

Эта модель предполагает построение схемы по частям. Каждая итерация добавляет функциональные возможности к предыдущим.
Требует четкого понимания архитекруты.

### AGILE

Подход к управлению проектом, который предполагает разбиение проекта на этапы и акцентирует внимание на непрерывном
сотрудничестве и совершенствовании. Команды следуют циклу планирования, выполнения и оценки.

Ценности agile:

- Люди
- Работающий продукт
- Сотрудничество с заказчиком
- Готовность к изменениям

_у agile так же существует 12 принципов (хз какие, это знать вообще не надо)_

### SCRUM

> Важно {style="warning"}

**Scrum** - это фреймворк, одна из разновидностей _agile_. Суть в том, что мы что-то делаем и показываем, что-то сделали
и показали и так по кругу, пока не будет готовый проект.

**Ценности scrum:**

- Приверженность
- Открытость
- Сфокусированность
- Уважение
- Смелость

**Принципы Scrum:**

- Работа короткими циклами - спринтами (спринт от 1 недели до 4 недель, в основном всегда 2). Все действия планируются в
  рамках одного спринта.
- Гибкость. После каждого спринта продукт тестируют.
- Участие заказчика и пользователей в работе над продуктом.
- Тесное взаимодействие команды.

Результатом спринта является инкремент.

_Виды звонков_:

- **Планинг** (планирование спринта, оценка задач)
- **Дейли** (ежедневные созвоны по итогам работы (так же могут быть и не ежедневные, а например через день))
- **Демо** (созвон с заказчиком)
- **Ретроспектива** (анализ прошлого спринта, ошибок и тд)

_Роли_:

- product owner (человек который придумал продукт. определяет что нужно, задает требования и приоритеты, советуются с
  ним бизнес аналитики)
- команда разработчиков (от 3 до 10 человек. Девы. бизнес аналитики и пм)
- Scrum мастер


- Техлид (персонаж, который знает все о проекте, знает всю архитектуру. знает все тех решения)
- Тимлид (руководитель команды разработки)

**Scrum мастер** - отвечает за эффективность команды, причем именно целой команды, а не ее отдельных участников.

Артефакты скрама:

- бэклоги (списки задач, которые нужно сделать).
- спринт бэклог (спискок задач которые уже выбраны для реализации)

_Рефаймент_ (refinement) - когда раз в месяц собираемся и обсуждаем что находится в бэклоге. Меняются приоритеты и ид.
Так
же может называться и _груминогм_

### **Kanban**

> Важно {style="warning"}

**wip** - ограничение на количество задач, которые могу быть в одной колонке. Что бы не валить другие колонки. Что бы
пример 10 тасок не летели подряд (как пример)

Статусы (в каждой команде определяются свои статусы, но эти будут в большинстве случаев):

- todo
- in progress
- in testing (optional)
- in design (optional)
- in code review (optional)
- done

Плюс в том, что это самоорганизация команды.

### SDLC

> Для ознакомления {style="note"}

В целом, SDLC это такой замкнутый цикл, в котором каждый этап влияет на действия в последующих и дает перспективные
указания на будущее.

- **Анализ требований** отвечает на вопрос «Какие проблемы требуют решений?»
- **Планирование** отвечает на вопрос «Что мы хотим сделать?»
- **Проектирование и дизайн** отвечает на вопрос «Как мы добьемся наших целей?»
- **Разработка ПО** регулирует процесс создания продукта.
- **Тестирование** регулирует обеспечение качественной работы продукта.
- **Deploy** регулирует использование финального продукта.
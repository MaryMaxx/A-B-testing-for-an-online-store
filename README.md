# Описание проекта
Вы — аналитик крупного интернет-магазина. Вместе с отделом маркетинга вы подготовили список гипотез для увеличения выручки.
Приоритизируйте гипотезы, запустите A/B-тест и проанализируйте результаты. 
**Цели и задачи:**
- применить фреймворк ICE для приоритизации гипотез, отсортировать их по убыванию приоритета;
- применить фреймворк RICE для приоритизации гипотез, отсортировать их по убыванию приоритета;
- указать, как изменилась приоритизация гипотез при применении RICE вместо ICE, объяснить, почему так произошло.
Основной задачей проекта также является оценка результатов А/В теста, который должен показать, приведет ли предложенная гипотеза к увеличению выручки интернет- магазина в группе В. Для анализа результатов А/В теста необходимы следующие шаги:
    
 - для оценки изменения результатов эксперимента на каждый день тестирования необходимо изучить графики таких кумулятивныхданных данных, как: выручки, среднего чека и конверсии; 
 - для выявления аномальных данных необходимо изучение точечного графика количества заказов по пользователям и по стоимости заказов, а также определение 95-ого и 99-ого перцентилей для определения границы аномадтных значений;
 - для того, чтобы сделать выводы о том, произоли ли изменения между тестируемыми группами необходимо провести оценку статистической значимости в среднем чеке и в среднем количестве заказов на посетителя между группами.
# Описание данных
**Структура — `/datasets/hypothesis.csv`**

- `Hypothesis`	— краткое описание гипотезы
- `Reach` — охват пользователей по 10-балльной шкале
- `Impact` —	влияние на пользователей по 10-балльной шкале
- `Confidence` —  уверенность в гипотезе по 10-балльной шкале
- `Efforts` — затраты ресурсов на проверку гипотезы по 10-балльной шкале

**Структура — `/datasets/orders.csv**

- `transactionId`	— идентификатор заказа
- `visitorId` — идентификатор пользователя, совершившего заказ
- `date` —	дата, когда был совершён заказ
- `revenue` —   выручка заказа
- `group` — группа A/B-теста, в которую попал заказ

**Структура — `/datasets/visitors.csv**

- `date`	— дата
- `group` — группа A/B-теста
- `visitors` —	количество пользователей в указанную дату в указанной группе A/B-теста

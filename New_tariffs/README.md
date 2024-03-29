# Описание проекта

**Задача**  
Нужно перевести клиентов с архивных тарифов на новые, для этого нужно посторить модель которая будет предлагать тарифы. Для тренировки есть база клиентов которые уже перешли с архивных тарифов на "Ултра" и "Смарт".

**Описание данных**  
Каждый объект в наборе данных — это информация о поведении одного пользователя за месяц. Известно:

- сalls — количество звонков,
- minutes — суммарная длительность звонков в минутах,
- messages — количество sms-сообщений,
- mb_used — израсходованный интернет-трафик в Мб,
- is_ultra — каким тарифом пользовался в течение месяца («Ультра» — 1, «Смарт» — 0).

# Используемые библиотеки

- pandas
- sklearn

# Что было сделано

1. Оценка качества собранных данных
2. Разбиение на выборки
3. Обучение моделей
4. Проверка моделей
5. Выводы

# Вывод

Построив три модели с разными гиперпараметрами получили что случайный лес показал лучшие результаты на тестовой выборке 82%. Остальные модели оказались хуже. Так же модель не угадывает результаты, а именно предсказывает, поскольку результаты намного выше случайных.

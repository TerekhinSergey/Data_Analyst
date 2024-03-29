﻿# Исследование окупаемости маркетинговых кампаний


**Описание проекта:** 

Мы занимаемся анализом развлекательного приложения «Procrastinate Pro+». Несмотря на огромные вложения в рекламу, последние несколько месяцев компания терпит убытки. Наша задача — разобраться в причинах и помочь компании выйти в плюс.

**Задачи:**

1. Изучить исходные данные и провести их предобработку.
2. Подготовить функции для расчета и анализа LTV, ROI, удержания и конверсии.
3. Создать пользовательские профили. Определить основную страну, устройство и канал привлечения платящих пользователей.
4. Определить общие траты на маркетинг, средний CAC и с разбивкой по источникам трафика.
5. Оценить общую окупаемость рекламы, а также с разбивкой по рекламным каналам и странам.
6. Выделить причины неэффективности привлечения пользователей и сформулировать рекомендации для отдела маркетинга.

**Используемые библиотеки и методы:** 

*Pandas*, *NumPy*, *Matplotlib*, *Datetime*, когортный анализ, юнит-экономика, продуктовые метрики

**Выводы:**

**Реклама перестала окупаться в целом с июня**, в то время, как **резко повысился CAC в канале привлечения пользователей TipTop**, на который приходится 15% от всего трафика привлечения пользователей, а также при **постоянном крайне низком удержании пользователей из канала FaceBoom**, на который приходится еще 20% трафика

Решить данную проблему можно следующими способами в порядке убывания важности:
- **снизить маркетинговые вложения в эти два канала, увеличивая маркетинговые вложения в lambdaMediaAds, MediaTornado или YRabbit**
- **договориться о снижении цен в каналах TipTop, FaceBoom и AdNonSense**
- **поработать над увеличением удержания пользователей на каналах FaceBoom и AdNonSense**
# Анализ тарифов телеком-компании


**Описание проекта:** 

Компания «Мегалайн» — федеральный оператор сотовой связи. Клиентам предлагается два тарифных плана: «Смарт» и «Ультра». Чтобы скорректировать рекламный бюджет, коммерческий департамент хочет понять, какой тариф приносит больше денег. Нам предстоит сделать предварительный анализ тарифов на небольшой выборке клиентов. В нашем распоряжении данные 500 пользователей «Мегалайна»: кто они, откуда, каким тарифом пользуются, сколько звонков и сообщений каждый отправил за 2018 год.

**Задачи:**

1. Изучить исходные данные и провести их предобработку
2. Определить, сколько минут разговора, сообщений и интернет-трафика требуется пользователям каждого тарифа в месяц.
3. Проверить гипотезы, что средняя выручка пользователей тарифов «Ультра» и «Смарт» различаются, а также, что средняя выручка пользователи из Москвы отличается от выручки пользователей из других регионов.

**Используемые библиотеки и методы:** 

*Pandas*, *NumPy*, *Matplotlib*, *SciPy*, описательная статистика, проверка статистических гипотез.

**Выводы:**

Нами была проведена работа по подсчёту помесячной выручки с каждого пользователя на основании выборки из 500 пользователей, на основании которой можно сделать следующие выводы:
- **использование сообщений** представлено Пуассоновским распределением с большим количеством неиспользующих сообщения пользователей на обоих тарифах, но в относительном выражении таких пользователей на тарифе **`Ultra`** больше. На тарифе **`Smart`** большинство использует **до 60** сообщений, а на тарифе **`Ultra`** **до 90**.  
- **использование минут** на тарифе **`Smart`** имеет похожее на нормальное распределение, скошенное влево. Большая часть пользователей тратят примерно **по 300-600 минут**. На тарифе **`Ultra`** большинство используют **по 0-800 минут**, а большее количество намного меньше
- **использование интернет-траффика** на обоих тарифах имеет нормальное распределение. При этом, на тарифе **`Smart`** большинство использует **12-23 ГБ**, а на тарифе **`Ultra`** **10-30 Гб**. 

В среднем пользователи тарифа **`Ultra`** используют лимиты примерно на 20-30% больше, чем пользователи тарифа **`Smart`**. При этом, у первых стандартное отклонение более, чем на 50% выше, что показывает более высокую меру разброса между пользователями тарифа **`Ultra`**.
    
Также нами было выдвинуто две гипотезы:  
- средняя выручка пользователей тарифа «Ультра» равна средней выручке пользователей «Смарт»   
- средняя выручка пользователей из Москвы равна средней выручке пользователей из других регионов  

После проведенных t-тестов мы выяснили, что **скорее всего первая гипотеза всё-таки неверна**, а **вторую гипотезу нет оснований отвергать**.  

**Т.к. по данной выборке получается средняя выручка с пользователей тарифа `Ultra` почти в 1.5 раза выше, можно предположить, что оператору "Мегалайн" будет выгоднее увеличить рекламный бюджет именно на этот тариф.**


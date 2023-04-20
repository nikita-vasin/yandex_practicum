# Описание проекта Исследовательский анализ данных - данные сервиса Яндекс Недвижимость

## Данные
- `ab_project_marketing_events.csv`
- `final_ab_new_users.csv`
- `final_ab_events.csv`
- `final_ab_participants.csv`


#### Структура файла  ab_project_marketing_events.csv:  
- `name` — название маркетингового события;
- `regions` — регионы, в которых будет проводиться рекламная кампания;
- `start_dt` — дата начала кампании;
- `finish_dt` — дата завершения кампании.
- `/datasets/ab_project_marketing_events.csv` — календарь маркетинговых событий на 2020 год;

#### Структура файла final_ab_new_users.csv:
- `user_id` — идентификатор пользователя;
- `first_date` — дата регистрации;
- `region` — регион пользователя;
- `device` — устройство, с которого происходила регистрация.
- `/datasets/final_ab_new_users.csv` — все пользователи, зарегистрировавшиеся в интернет-магазине в период с 7 по 21 декабря 2020 года;

#### Структура файла final_ab_events.csv:
- `user_id` — идентификатор пользователя;
- `event_dt` — дата и время события;
- `event_name` — тип события;
- `details` — дополнительные данные о событии. Например, для покупок, purchase, в этом поле хранится стоимость покупки в долларах.
- `/datasets/final_ab_events.csv` — все события новых пользователей в период с 7 декабря 2020 по 4 января 2021 года;

#### Структура файла final_ab_participants.csv:
- `user_id` — идентификатор пользователя;
- `ab_test` — название теста;
- `group` — группа пользователя.
- `/datasets/final_ab_participants.csv` — таблица участников тестов.
## Задача
В распоряжении данные сервиса Яндекс Недвижимость — архив объявлений за несколько лет о продаже квартир в Санкт-Петербурге и соседних населённых пунктах.
Задача — выполнить предобработку данных и изучить их, чтобы найти интересные особенности и зависимости, которые существуют на рынке недвижимости.
О каждой квартире в базе содержится два типа данных: 
- добавленные пользователем
- картографические. 
К первому типу относятся площадь квартиры, её этаж и количество балконов, ко второму — расстояния до центра города, аэропорта и ближайшего парка. 
## Используемые библиотеки
- `import pandas as pd`
- `import datetime as dt`
- `import seaborn as sns`
- `import numpy as np`
- `import math as mth`
- `from scipy import stats as st`
- `import matplotlib.pyplot as plt`
- `import plotly.graph_objects as go`
- `from pandas.plotting import register_matplotlib_converters`
- `import warnings`
- `warnings.simplefilter('ignore')`
- `import folium`
- `from folium import Map, Marker, Choropleth`
- `from folium.plugins import MarkerCluster`
- `import json`


# Описание проекта по формированию модели монетизации игры «Космические братья»

## Данные
- `game_actions.csv`
- `ad_costs.csv`
- `user_source.csv`


#### Структура файла  game_actions.csv:  
- `event_datetime` — время события;
- `event` — одно из трёх событий:
    - `building` — объект построен,
    - `finished_stage_1` — первый уровень завершён,
    - `project` — проект завершён;
- `building_type` — один из трёх типов здания:
    - `assembly_shop` — сборочный цех,
    - `spaceport` — космопорт,
    - `research_center` — исследовательский центр;
- `user_id` — идентификатор пользователя;
- `project_type` — тип реализованного проекта;

#### Структура файла ad_costs.csv:
- `day` - день, в который был совершен клик по объявлению;
- `source` - источник трафика;
- `cost` - стоимость кликов.

#### Структура файла user_source.csv:
- `user_id` - идентификатор пользователя;
- `source` - источников, с которого пришёл пользователь, установивший приложение.

## Задача
Сформировать модель монетизации игрового приложения «Космические братья».
Многие игры зарабатывают с помощью рекламы. 
<br>И все они сталкиваются с противоречием;</br>
- Пользователь разозлится и уйдёт, если начать показывать ему рекламу раньше, чем игра его затянет.
- Но  чем позже создатели игры включат рекламу, тем меньше они заработают.

Пока создатели игры планируют показывать рекламу на экране с выбором постройки. Помочь им не уйти в минус.

1. Провести исследовательский анализ данных

2. Проанализировать влияние событий на совершение целевого события

3. Проверить статистические гипотезы

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

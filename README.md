

Кластеризация фильмов и телешоу Netflix
Этот проект является частью учебной программы «Неконтролируемое машинное обучение» в качестве завершающего проекта в AlmaBetter School.
Цели:
Провести исследовательский анализ данных.
Попробуйте понять, какой тип контента доступен в разных странах.
Проверьте, в последние годы Netflix все больше внимания уделяет телевидению, а не фильмам.
Кластеризация похожего контента путем сопоставления текстовых функций.
Используемые методы:
Описательная статистика.
Визуализация данных.
Машинное обучение.
Используемые библиотеки:
NumPy и Pandas — для очистки и анализа набора данных.
Matplotlib, Plotly и Seaborn — для визуализации данных.
SkLearn и nltk — для машинного обучения и кластеризации.
Используемый набор данных:
Этот набор данных состоит из телешоу и фильмов, доступных на Netflix по состоянию на 2019
год. Он получен из Flixable, сторонней поисковой системы Netflix.

Attribute Information:

show_id : Unique ID for every Movie / Tv Show
type : Identifier - A Movie or TV Show
title : Title of the Movie / Tv Show
director : Director of the Movie
cast : Actors involved in the movie / show
country : Country where the movie / show was produced
date_added : Date it was added on Netflix
release_year : Actual Releaseyear of the movie / show
rating : TV Rating of the movie / show
duration : Total Duration - in minutes or number of seasons
listed_in : Genere
description: The Summary description
Обзор проекта:
Netflix — американский стриминговый сервис по подписке и продюсерская компания. Он был основан в 1997 году Ридом Хастингсом и Марком Рэндольфом в Скоттс-Вэлли, Калифорния.

Он предлагает библиотеку фильмов и телесериалов через соглашения о распространении, а также собственные продукты, известные как Netflix Originals.

Наша цель — провести исследовательский анализ данных, чтобы понять, какой контент доступен в разных странах, и уделяет ли Netflix в последние годы все больше внимания телевидению, а не фильмам. И используйте эти идеи для кластеризации похожего контента путем сопоставления текстовых функций.

После загрузки данных мы начинаем с наблюдения за первым и последним пятью значениями, чтобы понять набор данных. Затем мы обрабатываем нулевые значения, отбрасывая их, если соответствующие переменные содержат <1% нулевых значений. Затем следует разработка функций для извлечения новых переменных из переменной datetime date_added.

Эти очищенные данные затем используются для проведения EDA, чтобы лучше понять его и определить лежащие в его основе тенденции.

Получив необходимую информацию от EDA, мы начинаем с предварительной обработки текстовых данных, удаляя знаки препинания и стоп-слова. Эти отфильтрованные данные передаются через TF — IDF Vectorizer, поскольку мы проводим текстовую кластеризацию, а модели требуется векторизация данных, чтобы предсказать желаемые результаты.

Наконец, кластеризация K-средних используется для формирования 10 отдельных кластеров с похожими точками данных.

Используя предоставленные данные, мы также внедрили простую рекомендательную систему, которая успешно генерирует десять похожих фильмов или сериалов для заданного названия.

<h1>Benchmark earthquake dataset</h1>

> Данный набор данных был собран в рамках ВКР "Применение методов машинного обучения к задаче прогнозирования землетрясений" (СПбГУ, 2019 г. ).

Этот репозиторий содержит данные о землетрясениях, произошедших за 1968-2018 гг. в различных сейсмических зонах:
* *Южная Калифорния, США* (32-36.5° с.ш., 114.75-121° з.д..)
* *Центральный Чили* (32.5-36° ю.ш., 70-72.5° з.д.)
* *Гиндукуш, Пакистан* (35-39° с.ш., 69-74.6° в.д.)
* *Центральная Япония* (34-39° с.ш., 136.5-142° в.д.)
* *о. Сицилия, Италия* (36-39° с.ш., 12-16° в.д.)

Кроме того, в нём также содержатся функции для расчёта двух наборов сейсмических индикаторов - параметров, которые можно использовать для построения моделей сейсмической активности в регионе. На данный момент реализованы два набора индикаторов: первый был предложен в работе [1] (*Adeli & Panakkat*), второй - в публикации [2] (*Reyes et al.*). Скорее всего, в будущем набор будет пополняться :)

<h2>Источники данных</h2>

Данные о землетрясениях для Южной Калифорнии, Центральной Японии, Чили и Гиндукуша взяты из каталога [Геологической службы США (USGS)](https://earthquake.usgs.gov/earthquakes/search/). 

Данные по о. Сицилия, в силу неполноты предыдущего источника для этого региона, взяты из базы данных [Национального института геофизики и вулканологии Италии (INGV)](http://cnt.rm.ingv.it/en) (важно: в ней содержатся данные лишь начиная с 01.01.1985 года, однако даже с учётом этого каталог USGS менее полон, чем национальная база INGV)

<h2>Описание данных</h2>

| *Регион*  | Сицилия, Италия | Центральная Япония  | Центральный Чили | Гиндукуш, Пакистан | Южная Калифорния, США |
| :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
| ***Географические координаты***  | 36-39° с.ш., 12-16° в.д. | 34-39° с.ш., 136.5-142° в.д. | 32.5-36° ю.ш., 70-72.5° з.д..|	35-39° с.ш., 69-74.6° в.д..|	32-36.5° с.ш., 114.75-121° з.д..|
|***Число событий в каталоге*** |	7619 |	4604 |	7080 |	6611 | 14457|
| ***Минимальная (cut-off) магнитуда***  | 2.5 |	4.5 |	3.5 |	4.0 |	3.0 |
| ***Максимальная магнитуда*** |	5.8 |	7.9 |	8.0 |	7.5 |	7.3 |
| ***Средняя магнитуда*** |	2.82 |	4.849 |	4.05 |	4.46 |	3.408 |
| ***Временной промежуток*** |	01.01.1985 -  31.12.2018 |	01.01.1968 – 31.12.2018 |	01.01.1968 – 31.12.2018 |	01.01.1968 – 31.12.2018 |	01.01.1968 – 31.12.2018 |
| ***Источник данных*** |	INGV |	USGS |	USGS |	USGS |	USGS |


<h2>Структура данных</h2>
Все данные находятся в формате .csv (разделители - точки с запятой). Ниже приведены описания семантики столбцов таблиц в каждой из папок:
<h3>Raw data</h3>

<h3>Adeli and Panakkat seismicity indicators</h3>
<h3>Reyes et al. seismicity indicators</h3>


<h2>Источники литературы</h2>

[1] A. Panakkat, and H. Adeli, “Neural network models for earthquake magnitude prediction using multiple seismicity indicators,” International Journal of Neural Systems, vol. 17(1), pp. 13–33, 2007.

[2] F. Martínez-Álvarez, A. Morales-Esteban, and J. Reyes, “Neural networks to predict earthquakes in Chile,” Applied Soft Computing, vol. 13, pp. 1314-1328, 2013.

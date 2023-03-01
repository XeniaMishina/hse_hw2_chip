# hse_hw2_chip

- Ссылка на Google Colab: https://colab.research.google.com/drive/11mn2DhvOM9NJBrJCLqhctkeqUl5U1fMS?usp=sharing
- Ссылка на тот же ipynb файл на github: https://github.com/XeniaMishina/hse_hw2_chip/blob/main/src/Mishina_hse23_HW2_chip.ipynb

Клеточная линия A549, гистоновая метка H3K4me1

. | Реплика 1 | Реплика 2 | Контроль
--- | --- | --- | ---
ID | ENCFF294ENQ | ENCFF478YXZ | ENCFF526AVE

## Анализ FascQC

Скрины некоторых графиков: (более подробно анализ можно увидеть в соответствующих html-отчетах)

ID | Basic Statistics | Per base sequence quality | Per sequence quality scores | Per sequence GC content
--- | --- | --- | --- | ---
ENCFF294ENQ | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/294_BS.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/294_PBSQ.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/294_PSQS.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/294_GC.png) |
ENCFF478YXZ | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/478_BS.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/478_PBSQ.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/478_PSQS.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/478_GC.png) |
ENCFF526AVE | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/526_BS.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/526_PBSQ.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/526_PSQS.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/526_GC.png) |

Ссылки на html-файлы анализов: 
- [ENCFF294ENQ](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/data/ENCFF294ENQ_fastqc.html)
- [ENCFF478YXZ](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/data/ENCFF478YXZ_fastqc.html)
- [ENCFF526AVE](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/data/ENCFF526AVE_fastqc.html)

Подрезания или фильтрация не требуются, качество чтений хорошее.

## Выравнивание на 16ую хромосому

ID | reads |	aligned 0 times |	aligned 0 times, % |	aligned exactly 1 time |	aligned exactly 1 time, % |	aligned >1 times |	aligned >1 times, %
--- | --- | --- | --- | --- | --- | --- | ---
ENCFF294ENQ |	38054107 | 32201394 |	84.62% | 1364942 | 3.59% |	4487771 |	11.79%
ENCFF478YXZ |	32158640 | 26855735 |	83.51% | 1191201 | 3.70% |	4111704 |	12.79%
ENCFF526AVE |	17936432 | 14749726 |	82.23% | 694391 |	3.87% |	2492315 |	13.90%

Выравнивание происходило на одну хромосому, которая составляет малую часть генома человека, соответственно и процент выравниваний получился довольно низким.
## Диаграммы Эйлера-Венна

### Реплика 1 и ENCODE

ENCFF294ENQ / ENCODE | ENCODE / ENCFF294ENQ
--- | ---
![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/venn1.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/venn2.png)

### Реплика 2 и ENCODE

ENCFF478YXZ / ENCODE | ENCODE / ENCFF478YXZ
--- | ---
![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/venn3.png) | ![](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/venn4.png)

Пересечений мало, это объясняется тем, что выравнивание было сделано на одну хромосому.
В базе данных ENCODE представлены пики для всех хромосом, поэтому их заметно больше. 
Пересечения наших пиков с ENCODE и ENCODE с нашими пиками - не одно и то же, отсюда и разница в пересечениях.


## Бонусная часть 

Гистоновая метка H3K4me1 

![theory](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/screens/theory.png)
![result](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/data/result.png)

Результат похож на теоретический, график похож на расположение гистоновой метки, которое должно было получиться. Значения низкие, но смещений почти нет.

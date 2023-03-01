# hse_hw2_chip

Ссылка на Google Colab: https://colab.research.google.com/drive/11mn2DhvOM9NJBrJCLqhctkeqUl5U1fMS?usp=sharing

Клеточная линия A549, гистоновая метка H3K4me1

. | Реплика 1 | Реплика 2 | Контроль
--- | --- | --- | ---
ID | ENCFF294ENQ | ENCFF478YXZ | ENCFF526AVE

## Анализ FascQC

Скрины некоторых графиков: (более подробно анализ можно увидеть в соответствующих html-отчетах)



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

## Диаграммы Эйлера-Венна

### Реплика 1 и ENCODE
![img](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/data/Intervene_venn_1.pdf) | ![img](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/data/Intervene_venn_2.pdf)

### Реплика 2 и ENCODE


## Бонусная часть 

![result](https://github.com/XeniaMishina/hse_hw2_chip/blob/main/data/result.png)

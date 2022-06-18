# hse22_project
#### Целью работы над проектом является поиск и изучение консервативных участков генома Z-ДНК в геномах прокариот и эукариот. В процессе выполнения проекта будут получены важные практические навыки биоинформатика -- работа в командной строке с утилитой bedtools, визуализация данных, конвертация координат участков между разными версиями генома (разными организмами) и т.п.
таксон: Alphaproteobacteria

род: Brucella

Геномы: Brucella abortus 2308, Brucella canis ATCC 23365, Brucella ceti TE10759-12, Brucella microti CCM 4915, Brucella suis 1330

[Ссылка на Colab](https://colab.research.google.com/drive/1m9gQ03XS7d0Iz4EYIZpED4ls8Vmt0e5G?usp=sharing)

### Аннотированные гены и zDNA
| Вид                       | Кол-во аннотированных генов | Доля аннотированных генов | Кол-во предсказанных zDNA | Общая длина предсказанных zDNA | Кол-во предсказанных zDNA с ZH-Score >= 500 | Общая длина предсказанных zDNA с ZH-Score >= 500 |
|:--------------------------|:---------------------------:|:-------------------------:|:-------------------------:|:------------------------------:|:-------------------------------------------:|:------------------------------------------------:|
| Brucella abortus 2308     |            3174             |         87.728544         |          1156948          |            10754144            |                    37880                    |                      366386                      |
| Brucella canis ATCC 23365 |            3169             |         87.747742         |          1206800          |            11216388            |                    38284                    |                      370432                      |
| Brucella ceti TE10759-12  |            3164             |         87.684295         |          1160316          |            10789710            |                    37914                    |                      366972                      |
| Brucella microti CCM 4915 |            3199             |         87.747742         |          1220319          |            11342546            |                    38585                    |                      373370                      |
| Brucella suis 1330        |            3179             |         87.769756         |          1207381          |            11222218            |                    38348                    |                      371054                      |

### Графики с распределением ZH-score
#### Brucella abortus 2308
![Brucella abortus 2308](/images/ZHscore/1.png)
#### Brucella canis ATCC 23365
![Brucella canis ATCC 23365](/images/ZHscore/2.png)
#### Brucella ceti TE10759-12
![Brucella ceti TE10759-12](/images/ZHscore/3.png)
#### Brucella microti CCM 4915
![Brucella microti CCM 4915](/images/ZHscore/4.png)
#### Brucella suis 1330
![Brucella suis 1330](/images/ZHscore/5.png)
### Расположение предсказанных Z-ДНК
#### Brucella abortus 2308
![Brucella abortus 2308](/images/Zplace/1.png)
#### Brucella canis ATCC 23365
![Brucella canis ATCC 23365](/images/Zplace/2.png)
#### Brucella ceti TE10759-12
![Brucella ceti TE10759-12](/images/Zplace/3.png)
#### Brucella microti CCM 4915
![Brucella microti CCM 4915](/images/Zplace/4.png)
#### Brucella suis 1330
![Brucella suis 1330](/images/Zplace/5.png)
### Распределение предсказанных zDNA
![predicted zDNA gen](/images/ALL.png)
### Гомологичные кластеры
#### Количество геномов, входящих в кластеры
![clusters in genome](/images/CIG.png)
#### Количество генов в кластерах
![genes in clusters](/images/GIC.png)

Далее были выбраны 10 кластеров с самым большим средним ZH-Score

| Кластер | Количество генов в кластере | Вид бактерии              | Белок          | Ген, кодирующий белок | Средний ZH-score | Функция белка в организме                                     |
|---------|-----------------------------|---------------------------|----------------|-----------------------|------------------|---------------------------------------------------------------|
| 1       | 5                           | Brucella abortus 2308     | WP_002964335.1 | BAB_RS21785           | 198240.544480    | replication-associated recombination protein A                |
| 1       | 5                           | Brucella canis ATCC 23365 | WP_004690912.1 | BCAN_RS05605          | 165363.922333    | replication-associated recombination protein A                |
| 1       | 5                           | Brucella ceti TE10759-12  | WP_006174324.1 | V910_RS03935          | 111108.356156    | replication-associated recombination protein A                |
| 1       | 5                           | Brucella microti CCM 4915 | WP_004685696.1 | BMI_RS05635           | 92465.416554     | replication-associated recombination protein A                |
| 1       | 5                           | Brucella suis 1330        | WP_004690912.1 | BR_RS05585            | 141866.730057    | replication-associated recombination protein A                |
| 2       | 5                           | Brucella abortus 2308     | WP_002963494.1 | BAB_RS17645           | 61928.402920     | pantoate-beta-alanine ligase activity                         |
| 2       | 5                           | Brucella canis ATCC 23365 | WP_004690555.1 | BCAN_RS01565          | 58187.162767     | pantoate-beta-alanine ligase activity                         |
| 2       | 5                           | Brucella ceti TE10759-12  | WP_006173735.1 | V910_RS07985          | 77184.423650     | pantoate-beta-alanine ligase activity                         |
| 2       | 5                           | Brucella microti CCM 4915 | WP_004682909.1 | BMI_RS01545           | 77184.423650     | pantoate-beta-alanine ligase activity                         |
| 2       | 5                           | Brucella suis 1330        | WP_004690555.1 | BR_RS01545            | 69514.254920     | pantoate-beta-alanine ligase activity                         |
| 3       | 5                           | Brucella abortus 2308     | WP_002966952.1 | BAB_RS24200           | 138924.10000     | TerC family protein                                           |
| 3       | 5                           | Brucella canis ATCC 23365 | WP_004688685.1 | BCAN_RS07985          | 138924.10000     | TerC family protein                                           |
| 3       | 5                           | Brucella ceti TE10759-12  | WP_004688685.1 | V910_RS01545          | 31057.09974      | TerC family protein                                           |
| 3       | 5                           | Brucella microti CCM 4915 | WP_004688685.1 | BMI_RS08000           | 138924.10000     | TerC family protein                                           |
| 3       | 5                           | Brucella suis 1330        | WP_004688685.1 | BR_RS07960            | 138924.10000     | TerC family protein                                           |
| 4       | 5                           | Brucella abortus 2308     | WP_002964842.1 | BAB_RS24360           | 35915.740500     | thiamine/thiamine pyrophosphate ABC transporter permease ThiP |
| 4       | 5                           | Brucella canis ATCC 23365 | WP_006132890.1 | BCAN_RS08140          | 35915.740500     | thiamine/thiamine pyrophosphate ABC transporter permease ThiP |
| 4       | 5                           | Brucella ceti TE10759-12  | WP_006174745.1 | V910_RS01390          | 23320.527629     | thiamine/thiamine pyrophosphate ABC transporter permease ThiP |
| 4       | 5                           | Brucella microti CCM 4915 | WP_004689223.1 | BMI_RS08155           | 35915.740500     | thiamine/thiamine pyrophosphate ABC transporter permease ThiP |
| 4       | 5                           | Brucella suis 1330        | WP_006192520.1 | BR_RS08115            | 35915.740500     | thiamine/thiamine pyrophosphate ABC transporter permease ThiP |
| 5       | 5                           | Brucella abortus 2308     | WP_002969577.1 | BAB_RS22905           | 105938.8615      | hypothetical protein                                          |
| 5       | 5                           | Brucella canis ATCC 23365 | WP_002969577.1 | BCAN_RS06695          | 105938.8615      | hypothetical protein                                          |
| 5       | 5                           | Brucella ceti TE10759-12  | WP_002969577.1 | V910_RS02820          | 66307.0910       | hypothetical protein                                          |
| 5       | 5                           | Brucella microti CCM 4915 | WP_002969577.1 | BMI_RS06730           | 105938.8615      | hypothetical protein                                          |
| 5       | 5                           | Brucella suis 1330        | WP_002969577.1 | BR_RS06675            | 105938.8615      | hypothetical protein                                          |
| 6       | 5                           | Brucella abortus 2308     | WP_006099340.1 | BAB_RS31825           | 2886.060020      | TonB-dependent receptor                                       |
| 6       | 5                           | Brucella canis ATCC 23365 | WP_006133555.1 | BCAN_RS15705          | 1806.207867      | TonB-dependent receptor                                       |
| 6       | 5                           | Brucella ceti TE10759-12  | WP_006175967.1 | V910_RS10735          | 1699.002821      | TonB-dependent receptor                                       |
| 6       | 5                           | Brucella microti CCM 4915 | WP_004688780.1 | BMI_RS15740           | 2040.246654      | TonB-dependent receptor                                       |
| 6       | 5                           | Brucella suis 1330        | WP_006191543.1 | BR_RS15675            | 1429.398867      | TonB-dependent receptor                                       |
| 7       | 5                           | Brucella abortus 2308     | WP_002967306.1 | BAB_RS29765           | 4660.949617      | Gfo/Idh/MocA family oxidoreductase                            |
| 7       | 5                           | Brucella canis ATCC 23365 | WP_004688980.1 | BCAN_RS12515          | 865.722333       | Gfo/Idh/MocA family oxidoreductase                            |
| 7       | 5                           | Brucella ceti TE10759-12  | WP_004688980.1 | V910_RS13815          | 5409.265887      | Gfo/Idh/MocA family oxidoreductase                            |
| 7       | 5                           | Brucella microti CCM 4915 | WP_004688980.1 | BMI_RS12480           | 158050.860333    | Gfo/Idh/MocA family oxidoreductase                            |
| 7       | 5                           | Brucella suis 1330        | WP_004688980.1 | BR_RS12475            | 865.722333       | Gfo/Idh/MocA family oxidoreductase                            |
| 8       | 5                           | Brucella abortus 2308     | WP_002967026.1 | BAB_RS25735           | 778.619500       | ParA family protein                                           |
| 8       | 5                           | Brucella canis ATCC 23365 | WP_004689316.1 | BCAN_RS09505          | 778.619500       | ParA family protein                                           |
| 8       | 5                           | Brucella ceti TE10759-12  | WP_004689316.1 | V910_RS00045          | 2106.624325      | ParA family protein                                           |
| 8       | 5                           | Brucella microti CCM 4915 | WP_004689316.1 | BMI_RS09515           | 778.619500       | ParA family protein                                           |
| 8       | 5                           | Brucella suis 1330        | WP_004689316.1 | BR_RS09470            | 778.619500       | ParA family protein                                           |
| 9       | 5                           | Brucella abortus 2308     | WP_002965857.1 | BAB_RS28525           | 22930.530886     | ABC transporter permease                                      |
| 9       | 5                           | Brucella canis ATCC 23365 | WP_002965857.1 | BCAN_RS13735          | 26495.734800     | ABC transporter permease                                      |
| 9       | 5                           | Brucella ceti TE10759-12  | WP_002965857.1 | V910_RS12660          | 22936.906314     | ABC transporter permease                                      |
| 9       | 5                           | Brucella microti CCM 4915 | WP_002965857.1 | BMI_RS13710           | 22828.791971     | ABC transporter permease                                      |
| 9       | 5                           | Brucella suis 1330        | WP_002965857.1 | BR_RS13710            | 23232.380200     | ABC transporter permease                                      |
| 10      | 5                           | Brucella abortus 2308     | WP_002965747.1 | BAB_RS27975           | 12189.571567     | arginase activity                                             |
| 10      | 5                           | Brucella canis ATCC 23365 | WP_004692171.1 | BCAN_RS14270          | 1980.781900      | arginase activity                                             |
| 10      | 5                           | Brucella ceti TE10759-12  | WP_006175260.1 | V910_RS12140          | 2950.914122      | arginase activity                                             |
| 10      | 5                           | Brucella microti CCM 4915 | WP_002965747.1 | BMI_RS14235           | 1230.145450      | arginase activity                                             |
| 10      | 5                           | Brucella suis 1330        | WP_002965747.1 | BR_RS14245            | 3443.866589      | arginase activity                                             |

### Распределение Z-ДНК относительно генов в кластерах
![zdna](/images/zdna/zcl1.png)
![zdna](/images/zdna/zcl2.png)
![zdna](/images/zdna/zcl3.png)
![zdna](/images/zdna/zcl4.png)
![zdna](/images/zdna/zcl5.png)
![zdna](/images/zdna/zcl6.png)
![zdna](/images/zdna/zcl7.png)
![zdna](/images/zdna/zcl8.png)
![zdna](/images/zdna/zcl9.png)
![zdna](/images/zdna/zcl10.png)
### Множественное белковое выравнивание
Данные файлы расположены в папке muscle

### Визуализация расположение Z-ДНК для кластеров
![clusters](/images/clusters/cl1.png)
![clusters](/images/clusters/cl2.png)
![clusters](/images/clusters/cl3.png)
![clusters](/images/clusters/cl4.png)
![clusters](/images/clusters/cl5.png)
![clusters](/images/clusters/cl6.png)
![clusters](/images/clusters/cl7.png)
![clusters](/images/clusters/cl8.png)
![clusters](/images/clusters/cl9.png)
![clusters](/images/clusters/cl10.png)
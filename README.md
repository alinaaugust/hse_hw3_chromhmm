# hse_hw3_chromhmm

### Августёнок Алина, 1 группа

##### [Ссылка](https://colab.research.google.com/drive/1wV2rjnnweVDTCivb0BAwx_PEHQ2qR8W6?usp=sharing) на ноутбук.

### Гистоновые метки:

|Название | Файл |
|---------|------|
| H4k20me1|wgEncodeBroadHistoneH1hescH4k20me1StdAlnRep1.bam |
| H3k09me3 | wgEncodeBroadHistoneH1hescH3k09me3StdAlnRep1.bam |
| H3k9ac | wgEncodeBroadHistoneH1hescH3k9acStdAlnRep1.bam |
| H3k79me2 | wgEncodeBroadHistoneH1hescH3k79me2StdAlnRep1.bam |
| H3k4me3 | wgEncodeBroadHistoneH1hescH3k4me3StdAlnRep1.bam |
| H3k4me2 | wgEncodeBroadHistoneH1hescH3k4me2StdAlnRep1.bam |
| H3k4me1 | wgEncodeBroadHistoneH1hescH3k4me1StdAlnRep1.bam |
| H3k36me3 | wgEncodeBroadHistoneH1hescH3k36me3StdAlnRep1.bam |
| H3k27me3 | wgEncodeBroadHistoneH1hescH3k27me3StdAlnRep1.bam |
| H3k27ac | wgEncodeBroadHistoneH1hescH3k27acStdAlnRep1.bam |

### cellmarkfiletable.txt
Файл также прикреплен в папке data.

|Клеточная линия|Гистоновая метка|Файл гистоновой метки|Файл контроля|
|---------------|----------------|---------------------|-------------|
| H1 | H3k4me1 | H3k4me1.bam | Control.bam |
| H1 | H3k27ac | H3k27ac.bam | Control.bam |
| H1 | H3k09me3 | H3k09me3.bam | Control.bam |
| H1 | H3k36me3 | H3k36me3.bam | Control.bam |
| H1 | H3k4me3 | H3k4me3.bam | Control.bam |
| H1 | H3k79me2 | H3k79me2.bam | Control.bam |
| H1 | H3k4me2 | H3k4me2.bam | Control.bam |
| H1 | H4k20me1 | H4k20me1.bam | Control.bam |
| H1 | H3k27me3 | H3k27me3.bam | Control.bam |
| H1 | H3k9ac | H3k9ac.bam | Control.bam |


### ChromHMM
Выдача ChromHmm также может быть найдена в соответствующей папке.

|Emission| Transition | Enrichment | RefSeqTSS | RefSeqTES |
|--------|---|---|---|---|
|![image](https://github.com/alinaaugust/hse_hw3_chromhmm/assets/97590705/ddafd061-06c9-430a-b029-7e3b58454532)| ![image](https://github.com/alinaaugust/hse_hw3_chromhmm/assets/97590705/16141dc2-2841-4b2b-8ee0-a0a04dc9c8aa) | ![image](https://github.com/alinaaugust/hse_hw3_chromhmm/assets/97590705/c15cd88d-7b06-4061-b303-e05c577c9a4e) | ![image](https://github.com/alinaaugust/hse_hw3_chromhmm/assets/97590705/c56a296b-2c8c-45a5-8856-714cf85b16b3) | ![image](https://github.com/alinaaugust/hse_hw3_chromhmm/assets/97590705/a6cf3c99-50ed-4a6b-9058-e67b0fec684d) |


### Эпигенетические типы
![image](https://github.com/alinaaugust/hse_hw3_chromhmm/assets/97590705/584bf0a9-fb6d-4ce3-885b-f19dad2fa298)


|№  | Название | Описание                      | 
|---|----------|-------------------------------|
| 1.| Гетерохроматин | выражен в H3K27me3; попадает между генами; компактно расположен|
| 2.| Weak enhancer | выражен в H3K27me3, H3k4me2; попадает между генами |
| 3.| Active promoter | выражен в H3K27me3, H3k4me2, H3k4me3; попадает между генами; много на CpGIsland | 
| 4.| Strong enhancer | выражен в H3k4me2, H3k4me3; попадает между генами; много на RefSeqTSS, RefSeqTSS2kb | 
| 5.| Active promoter | выражен в H3k4me2, H3k4me3, H3k9ac; попадает на интрон; много на CpGIsland, RefSeqTSS, RefSeqTES, RefSeqExon | 
| 6.| Weak enhancer/weak trancsribed | выражен в H3k4me2; попадает между генами и на интрон; одинаково слабо выражен на всех фолдах |  
| 7.| Weak transcribed | выражен в H3k4me2, H3k4me3, H3k79me2; попадает на интрон; много на RefSeqGene, RefSeqTSS2kb |  
| 8.| Weak transcribed | выражен в H3k79me2; попадает на интрон; много на RefSeqGene |  
| 9.| Weak transcribed | слабо выражен в H3k79me2; попадает на интрон; много на RefSeqGene |  
| 10.| Weak Enhancer | не выражен практически нигде; попадает на интрон; много на RefSeqGene, RefSeqTES, ядерной ламине | 
| 11.|Weak Promoter  | выражен в H3k36me3; попадает на интрон и экзон; много на RefSeqGene, RefSeqTES, RefSeqExon | 
| 12.| Гетерохроматин | понемногу выражен везде, сильнее в H3k09me3, H3k36me3; много на RefSeqExon, RefSeqTES | 
| 13.| Гетерохроматин | выражен в H3k09me3; попадает между генами; много на ядерной ламине | 
| 14.| Репрессор | не выражен практически нигде; попадает на интрон, но больше между генами; много на ламине | 
| 15.| Гетерохроматин | слабо выражен в H3k4me1; попадает на экзон и интрон; немного на RefSeqGene, RefSeqTES, ламине| 

### Бонус
Код для бонусной части, как и для основной, приведен в ноутбуке.

![image](https://github.com/alinaaugust/hse_hw3_chromhmm/assets/97590705/57583c02-f182-4349-9869-bb99cc0c4359)


































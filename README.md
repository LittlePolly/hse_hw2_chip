# hse_hw2_chip

Ссылка на ноутбук: https://colab.research.google.com/drive/1KFyiUBuTtmk13E32yDDrAzTd2lqdU8wp?authuser=1#scrollTo=3HPmyuscGyWJ

Выбрана клеточная линия DND-41 и гистоновая метка H3K4me2 

# Анализ выдачи fastqc

Отчеты в папке data. Я не проводила дополнительную обработку чтений. Per base sequence quality у всех трех файлов демонстрирует отличные результаты качества ридов.

ENCFF000APJ (реплика 1):

![image](https://user-images.githubusercontent.com/93220053/157501068-9b458054-e616-4252-b19c-764a5b2cd50a.png)

ENCFF000APK (реплика 2):

![image](https://user-images.githubusercontent.com/93220053/157501504-a8e6838d-88b6-4006-9f5e-2ad020a8bf07.png)

ENCFF000AOG (контроль):

![image](https://user-images.githubusercontent.com/93220053/157501712-290fba7d-d20e-4ca3-8d22-91d8bd650ae0.png)

Практически все графики по остальным параметрам проходят проверку качества. Исключение составляет GC распределение. Идеально проходит проверку только реплика 1:

![image](https://user-images.githubusercontent.com/93220053/157504508-cd91c539-87b8-45f6-8c46-f3612b926c5f.png)

ENCFF000APK (реплика 2):

![image](https://user-images.githubusercontent.com/93220053/157504619-a0e9f00a-f776-40bd-8d4b-f79cd449a61a.png)

ENCFF000AOG (контроль):

![image](https://user-images.githubusercontent.com/93220053/157504699-35d838be-974a-4a88-a08c-8cce2ebb819d.png)

Можно также обратить внимание на не очень хорошие результаты Per base sequence content. 

ENCFF000APJ (реплика 1):

![image](https://user-images.githubusercontent.com/93220053/157505505-05df68cd-04e4-4ebc-b570-a81dc7b8fe46.png)

ENCFF000APK (реплика 2) (здесь все хорошо):

![image](https://user-images.githubusercontent.com/93220053/157505597-5332d5f0-efbb-4404-a5cb-a48c8b958aa8.png)

ENCFF000AOG (контроль):

![image](https://user-images.githubusercontent.com/93220053/157505644-59d01f2f-4a93-462d-9521-0fb67316bd06.png)

В остальном качество ридов хорошее.

# Таблица выравниваний на хромосому 5

|                        |      total reads |   aligned 0 times | aligned exactly 1 time| aligned >1 times |
|------------------------|------------------|-------------------|-----------------------|------------------|
|ENCFF000APJ (реплика 1) |   28705707       | 24532782 (85.46%) | 1505454 (5.24%)       |2667471  (9.29%)  |
|ENCFF000APK (реплика 2) |   7946028        | 6761353  (85.09%) | 4029930 (5.07%)       |781745  (9.84%)   |
|ENCFF000AOG (контроль)  |      41060673    | 31902898 (77.70%) | 2779973 (6.77%)       | 6377802 (15.53%) |

# Диаграммы Венна

ENCFF000APJ (реплика 1):

<img width="475" alt="диа 1 1" src="https://user-images.githubusercontent.com/93220053/157511091-39e1abb0-5270-44f5-96b3-126ec91a5dce.png">

<img width="486" alt="диа 1 2" src="https://user-images.githubusercontent.com/93220053/157511130-bed44bee-30a6-43bf-9d6b-aba2ad168ef2.png">

ENCFF000APK (реплика 2):

<img width="527" alt="диа 2 1" src="https://user-images.githubusercontent.com/93220053/157511277-7fdbe676-bf0c-412e-8177-f2309f3d806d.png">

<img width="479" alt="диа 2 2" src="https://user-images.githubusercontent.com/93220053/157511340-b2b8d552-dfcf-4d51-8a8d-b8b640cd8661.png">

Пересечений получилось не очень много по причине выравнивания только на одну хромосому, но в целом результат неплохой. 

Бонусное задание не выполнялось.

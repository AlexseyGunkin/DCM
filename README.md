# Настройка интеграции с DCM

## Навигация
* [Об интеграции ](#Об-интеграции)
* [Схема интеграции ](#Схема-интеграции)
* [Настройка интеграции в личном кабинете CallTraking ](#Настройка-интеграции-в-личном-кабинете-CallTraking)



## Об интеграции


С помощью DCM вы сможете анализировать рекламу любых медийных продуктов или просмотров видео.

При интеграции DCM начнет собирать наднные по всем взаимодействиям пользователя с вашей рекламой вместе с информацией о просмотре рекламы и переходах с неё на ваш сайт (информация по переходам доступна только для рекламных размещений в Google). 

С помощью интеграции с CallTraking вы сможете настроить передачу в DCM данных по конверсиям. После этого, вам станет доступен полноценный анализ по всем конверсионным цепочкам ваших медийных размещений.

## Схема интеграции




## Настройка интеграции в личном кабинете CallTraking

Для того чтобы настроить интеграция DCM в личном кабинете CallTraking необходимо:

**Привязать аккаунта Google в Личном кабинете CallTraking**
- зайти в личный кабинет CallTraking
![Рис.1](images/LKCT1.jpg)
- перейти во вкладку интеграции
![Рис.2](images/VkladIn1.png)
- найти в списке интеграций Double Click и нажать " подключить "
![Рис.3](images/vkl.jpg)
- откроется окно для входа в Google аккаунт , где необходимо будет авторизоваться.
![Рис.4](images/LKCT.png)
- затем появиться окно в котором необходимо будет ввести "ID профиля DCM", его можно будет найти кликнув по иконке профиля гугл в правом верхнем углу браузера "google chrome"
![Рис.5](images/DCMID2.png)
![Рис.6](images/LKID.png)


**Обратите внимание**, интеграцию нельзя включить, пока все поля не будут заполнены.


**Настройка интеграции**

Поля которые необходимо будет заполнить :

![Рис.7](images/skript1.jpg)


1) src – id для отправки, только цифры, полный url не нужен (можно получить в DCM);
![Рис.10](images/src.png)
2) type – тип конверсии, цифры и латинские буквы (можно получить в DCM Floodlight - Activity groups);
![Рис.11](images/type.png)
3) cat – категория конверсии, цифры и латинские буквы. Что бы её получить, необходимо создать в разделе Activities - Advanced properties новую сущность, категория конверсии это Activity tag string
![Рис.12](images/cat.png)

![Рис.8](images/skript2.jpg)

- Переменная u №1 – номер переменной «u», в которую передается ID для связи конверсий, вы указываете только ее номер в DCM;

- Переменная u №2 – номер переменной для передачи свободного параметра. Например, можно указать в ней название вашего проекта, латиницей. В первом поле задаете ее номер из DCM, во втором – значение. Это значение будет присвоено всем конверсиям;

- Переменная u для источника – номер переменной «u», в которую передается информация по рекламному источнику, вы указываете только ее номер в DCM;

- Переменная u для канала – номер переменной «u», в которую передается информация по рекламному каналу, вы указываете только ее номер в DCM;

- Переменная u для кампании – номер переменной «u», в которую передается информация по рекламной кампании, вы указываете только ее номер в DCM;


![Рис.9](images/skript3.jpg)


- Переменная u для объявления – номер переменной «u», в которую передается информация по рекламному объявлению, вы указываете только ее номер в DCM;

- Переменная u для ключевого слова – номер переменной «u», в которую передается информация по ключевому слову, вы указываете только ее номер в DCM.



[Вернуться к оглавлению](#навигация)

[Вернуться на главную](/README.md/#documentation)
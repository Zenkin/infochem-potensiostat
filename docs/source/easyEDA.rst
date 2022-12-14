Работа в easyEDA
=================

Регистрация
____________

Главная страница
-----------------

На главной странице справа сверху нажимаем на "Зарегистрироваться".

.. figure:: _static/Pictures/easyEDA/reg1.png
    :scale: 30 %
    :align: center



-----------------

Создание аккаунта
------------------

Вводим пароль и проходим проверку на робота.

.. figure:: _static/Pictures/easyEDA/reg2.png
    :scale: 30 %
    :align: center

----------


Завершение
----------

.. figure:: _static/Pictures/easyEDA/reg3.png
    :scale: 30 %
    :align: center

___________________________________


Создание проекта с потенциостатом
____________________________________

Переходим во вкладку с редактором.


.. figure:: _static/Pictures/easyEDA/newScheme1.png
    :scale: 30 %
    :align: center


Выбираем STD Edition.

.. figure:: _static/Pictures/easyEDA/newScheme2.png
    :scale: 30 %
    :align: center

Создаем новый проект.

.. figure:: _static/Pictures/easyEDA/newScheme3.png
    :scale: 30 %
    :align: center

Выбираем название проекта.

.. figure:: _static/Pictures/easyEDA/newScheme4.png
    :scale: 30 %
    :align: center

После этого создается файл, где можно начинать создавать нашу электросхему.


.. figure:: _static/Pictures/easyEDA/newScheme4.5.png
    :scale: 30 %
    :align: center

Нажмите сочетание клавиш "Shift+f" или зайдите во вкладку "Установить -> Символ" и в поиске введите "DS-01BP" для поиска переключателя и нажимаем на кнопку "установить".


.. figure:: _static/Pictures/easyEDA/newScheme5.png
    :scale: 30 %
    :align: center

Кнопкой на мыши "ЛКМ" устанавливаем переключатель на рабочее поле. Колесиком миши можно масштабировать рабочее поле.

.. figure:: _static/Pictures/easyEDA/newScheme6.png
    :scale: 30 %
    :align: center


Далее необходимо подключить переключатель к контактам "VCC" и "OUT+". Создаем два NetFlag с помощью "Ctrl+Q".

.. figure:: _static/Pictures/easyEDA/newScheme7.png
    :scale: 30 %
    :align: center

Подключаем NetFlag к контактам переключателя с помощью Wire, нажимая на кнопку "W" и "ЛКМ" на контакты компонента. 

.. figure:: _static/Pictures/easyEDA/newScheme8.png
    :scale: 30 %
    :align: center

Далее двойной "ЛКМ" по левому NetFlag и меняем его название на "OUT+".

.. figure:: _static/Pictures/easyEDA/newScheme9.png
    :scale: 50 %
    :align: center

Нажимаем shift+F и выбираем LCSC electronics.

.. figure:: _static/Pictures/easyEDA/newScheme10.png
    :scale: 65 %
    :align: center

В поисковой строке ищем B-2100S04P-A110 и устанавливаем на схему.

.. figure:: _static/Pictures/easyEDA/newScheme11.png
    :scale: 65 %
    :align: center

.. figure:: _static/Pictures/easyEDA/newScheme12.png
    :scale: 65 %
    :align: center

Процесс установки:

https://niuitmo-my.sharepoint.com/personal/onisoris_niuitmo_ru/_layouts/15/stream.aspx?id=%2Fpersonal%2Fonisoris%5Fniuitmo%5Fru%2FDocuments%2FMyProjects%2F%D0%9F%D0%BE%D1%82%D0%B5%D0%BD%D1%86%D0%B8%D0%BE%D1%81%D1%82%D0%B0%D1%82%2FEasyEda%2Emp4&ga=1

Далее установим линейный стабилизатор напряжения MIC5205-3.3YM5 со всей необходимой обвязкой.

Данных навыков достаточно для дальнейшего построения схемы.

Постройте две схемы: с микроконтролером и со схемой питания. После этого можно приступать к разведению платы.




Преобразование в печатную плату
________________________________

Для преобразования в печатную плату переходим во вкладку "Дизайн" нажимаем "Преобразовать схему в печатную плату", либо просто зажимаем комбинацию клавишь "Alt+P".


.. figure:: _static/Pictures/easyEDA/PCB1.png
    :scale: 50 %
    :align: center

Проверяем цепи, нажимая "Да, проверить Цепи".


.. figure:: _static/Pictures/easyEDA/PCB2.png
    :scale: 50 %
    :align: center

Для примера я разместил не соединенную землю, причем найти такие элементы можно, нажав лкм по проблемному элементу в левом столбце.

https://niuitmo-my.sharepoint.com/personal/onisoris_niuitmo_ru/_layouts/15/stream.aspx?id=%2Fpersonal%2Fonisoris%5Fniuitmo%5Fru%2FDocuments%2FMyProjects%2F%D0%9F%D0%BE%D1%82%D0%B5%D0%BD%D1%86%D0%B8%D0%BE%D1%81%D1%82%D0%B0%D1%82%2FEasyEda%2Emp4&ga=1

Перед преобразованием необходимо сохранить проект, нажимаем "Ctrl+s".
Далее нажимаем снова "Alt+P", а после "Нет, продолжить".


.. figure:: _static/Pictures/easyEDA/PCB4.png
    :scale: 50 %
    :align: center

Пример создания границ платы, размеров 81x69.9 мм. 
Обратите внимание, что вам необходимо создать границы размером 81x60.9 мм.


https://niuitmo-my.sharepoint.com/personal/onisoris_niuitmo_ru/_layouts/15/stream.aspx?id=%2Fpersonal%2Fonisoris%5Fniuitmo%5Fru%2FDocuments%2FMyProjects%2F%D0%9F%D0%BE%D1%82%D0%B5%D0%BD%D1%86%D0%B8%D0%BE%D1%81%D1%82%D0%B0%D1%82%2FEasyEda%2Emp4&ga=1

Далее необходимо создать углубления по бокам платы, а также отверстия. Для удобства можно пользоваться схемой и таблицей с координатами отверстий, указанных ниже.


.. figure:: _static/Pictures/easyEDA/drawing1.png
    :scale: 60 %
    :align: center


Диаметр отверстий 3.50 мм.

.. csv-table:: Координаты отверстий
   :header: "Отверстие № ", "X, мм", "Y, мм"
   :widths: 10, 10, 10

   "Отверстие 1", 13.00, 2.85

   "Отверстие 2", 13.00, 58.05

   "Отверстие 3", 68.00, 58.05

   "Отверстие 4", 68.00, 2.85 

Пример создания квадратных углублений и отверстий в плате:

https://niuitmo-my.sharepoint.com/personal/onisoris_niuitmo_ru/_layouts/15/stream.aspx?id=%2Fpersonal%2Fonisoris%5Fniuitmo%5Fru%2FDocuments%2FMyProjects%2F%D0%9F%D0%BE%D1%82%D0%B5%D0%BD%D1%86%D0%B8%D0%BE%D1%81%D1%82%D0%B0%D1%82%2FEasyEda%2Emp4&ga=1


В итоге ваш результат должен быть выгядеть, как на картинке:

.. figure:: _static/Pictures/easyEDA/PCB5.png
    :scale: 50 %
    :align: center


____________________________

Разведение компонентов платы
_____________________________


Разместите все компоненты платы примерно так, как показано на рисунке.
Компоненты можно поворачивать, нажимая на кнопку "R".


.. figure:: _static/Pictures/easyEDA/razvodka1.png
    :scale: 50 %
    :align: center


____________________________


Автотрассировка
_______________


Автотрассировка необходима для расчета оптимальных путей дорожек на плате.
Выберем во вкладке "Трассировка" пункт "Автотрассировка..."

.. figure:: _static/Pictures/easyEDA/trace.png
    :scale: 40 %
    :align: center

Выбираем облачный сервер трассировки и запускаем.

.. figure:: _static/Pictures/easyEDA/trace2.png
    :scale: 40 %
    :align: center

В результате получится что-то подобное.

.. figure:: _static/Pictures/easyEDA/trace3.png
    :scale: 40 %
    :align: center


Далее необходимо увеличить силовые линии "OUT+" и "BAT1_-", выбираем линии через shift и в парвом верхнем углу выставляем ширину 30 mil.

.. figure:: _static/Pictures/easyEDA/Razvodka2.png
    :scale: 40 %
    :align: center


Для снижения шумов и для удобного доступа к земле необходимо "залить" медным слоем, соедененным с землей, пространство между дорожками. Для этого выбираем инструмент Copper Area буквой E или в панеле с инструментами.


https://niuitmo-my.sharepoint.com/personal/onisoris_niuitmo_ru/_layouts/15/stream.aspx?id=%2Fpersonal%2Fonisoris%5Fniuitmo%5Fru%2FDocuments%2FMyProjects%2F%D0%9F%D0%BE%D1%82%D0%B5%D0%BD%D1%86%D0%B8%D0%BE%D1%81%D1%82%D0%B0%D1%82%2FEasyEda%2Emp4&ga=1


Для редактирования второго слоя выбираем значок карандаша у второго слоя в панеле "Слои и объекты".

Просмотреть 3D вид модели можно во вкладке "Вид" -> "3D вид".


Подготовка файлов для производства платы
_________________________________________

Для производства необходимо несколько файлов. Один из них - Boom файл со списком всех компонентов. 


.. figure:: _static/Pictures/easyEDA/boom.png
    :scale: 40 %
    :align: center

Выбираем "Экспортировать Boom".

.. figure:: _static/Pictures/easyEDA/boom2.png
    :scale: 40 %
    :align: center

.. figure:: _static/Pictures/easyEDA/boom3.png
    :scale: 80 %
    :align: center

Сохраняем проект, после чего экспортируем Gerber файл. 


.. figure:: _static/Pictures/easyEDA/gerber1.png
    :scale: 50 %
    :align: center


Нажимаем "Да, проверить...". В случае, если есть ошибки, EasyEDA покажет, в каких местах они есть и поможет их исправить. В случае, если их нет, то перекинет на следующую вкладку.

.. figure:: _static/Pictures/easyEDA/gerber2.png
    :scale: 50 %
    :align: center

Генерируем Gerber файл:

.. figure:: _static/Pictures/easyEDA/gerber3.png
    :scale: 80 %
    :align: center



После этого скачивается нужный нам файл в .zip расширении. 












































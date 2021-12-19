# Simple_API
---
## Создание и тестирование приложения для работы с API

Тут описан процесс создания приложаения с функциями API и его тестировка.


Начнем по порядку.
Чтобы написать приложения для работы с API, нужно было разобраться как работают его функции.
Я реализовала все функции указанные в ТЗ используя библиотеку **request**.

![image](https://user-images.githubusercontent.com/71213226/145867856-542c5809-2e42-42f5-8fdf-6e70420dc145.png)

Код каждой функции вы можете увидеть в директории **API**, я же приведу результаты первоначальной работы (все скриншоты кликабельны!):

Создание новой карточки животного **без фото**:
![image](https://github.com/anna01122002/Simple_API/blob/main/pics/1.png)

Получение ключа API:
![image](https://github.com/anna01122002/Simple_API/blob/main/pics/2.png)

Получение списка **My_Pets**:
![image](https://github.com/anna01122002/Simple_API/blob/main/pics/3.png)

Создание новой карточки животного:
![image](https://github.com/anna01122002/Simple_API/blob/main/pics/4.png)

Добавить фото для животного:
![image](https://github.com/anna01122002/Simple_API/blob/main/pics/5.png)

Обновить информацию о животном:
![image](https://github.com/anna01122002/Simple_API/blob/main/pics/6.png)

---

Так как в ТЗ было указано использовать как **фикстуры**, так и **параметризацию**, то я использовал обе возможности.

У нас используется 3 функции POST, поэтому для них и была применена параметризация:
![image](https://user-images.githubusercontent.com/71213226/145870780-a77ccb87-dd79-405b-987f-400d31437512.png)


В параметрах указаны не только положительные, но и отрицательные кейсы, отмеченные как **marks=pytest.mark.xfail**
![image](https://user-images.githubusercontent.com/71213226/145870945-e7807c7d-12c6-4cb6-9057-eef50a81228e.png)

Таким образом, ошибка в тест-кейсе отображается как ожидаемая, что не ломает тестировку.
![image](https://user-images.githubusercontent.com/71213226/145871157-e5a4052e-6516-4258-9dca-706363330431.png)

Так же тест по фикстуре был применен к единственной функции PUT:
![image](https://user-images.githubusercontent.com/71213226/145871287-4134389a-70d7-4e50-b779-15d1eb9417a9.png)

### Итоги
В процессе работы над этим заданием я изучила и самостоятельно создал простые функции API, а также протестировала их несколькими методами.
Всё представленное в репозитории и на скриншотах является рабочим проектом.

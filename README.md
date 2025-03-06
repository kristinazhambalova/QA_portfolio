# <a name="up" />Портфолио тестировщика

Портфолио Кристины Жамбаловой. Здесь собраны проекты, выполненные во время обучения по специальности ["Инженер по тестиртованию"](https://practicum.yandex.ru/qa-engineer-plus/) в Яндекс.Практикуме.
P.S. Портфолио пополняется

Регрессионное тестирование и ретест багов веб-приложений

## <a name="test-design" />Регрессионное тестирование и ретест багов веб-приложений

### Задание 1. Регрессионое тестирование по готовым тест-кейсам
**1. Изучи требования к функциональности приложения Mesto.**

<details>
<summary>Требования к приложению Mesto</summary>

***

**0. Главная страница**

![Главная страница](https://code.s3.yandex.net/qa/schemes/project1_mesto_1.png)

1. Вёрстка адаптивная: ширина всей страницы с содержимым должна меняться вместе с шириной окна браузера. При этом не должна появляться горизонтальная полоса прокрутки.
2. По умолчанию на странице шесть карточек с фотографиями.
3. По умолчанию в профиле указано: Жак-Ив Кусто, Исследователь океана.

**1. Редактирование профиля**

![Редактирование](https://code.s3.yandex.net/qa/schemes/project1_mesto_2.png)

У пользователя должна быть возможность редактировать свой профиль.

1. Окно должно называться «Редактировать профиль».
2. Окно должно открываться по нажатию кнопки «Редактировать», а закрываться — при клике по крестику в правом верхнем углу.
3. В окне должно быть два поля: «Имя» и «Занятие», а также кнопка «Сохранить».
4. При открытии окна: поля «Имя» и «Занятие» должны быть заполнены теми значениями, которые отображаются на странице.
5. После внесения изменений и нажатия кнопки «Сохранить» информация на странице должна обновиться, а окно автоматически закрыться.
6. При сохранении должна быть валидация:
    - оба поля обязательные;
    - в поле «Имя» должно быть от 2 до 40 символов;
    - в поле «Занятие» должно быть от 2 до 200 символов.
7. Если хотя бы одно из полей не прошло валидацию, кнопка «Сохранить» должна быть неактивной. Если оба поля прошли — активной.
8. Если поле формы «Редактировать профиль» не прошло валидацию, под ним должен появляться красный текст, сообщающий об ошибке.

**2. Добавление карточки**

![Карточка](https://code.s3.yandex.net/qa/schemes/project1_mesto_3.png)

У пользователя должна быть возможность написать название карточки и дать ссылку на картинку.

1. Окно должно называться «Новое место».
2. Окно добавления должно открываться нажатием на кнопку «+» и закрываться кликом на крестик.
3. При сохранении должна быть валидация:
    - оба поля обязательные;
    - в поле «Название» должно быть от 2 до 30 символов;
    - в поле «Ссылка на картинку» должен быть URL.
4. При сохранении новая карточка должна добавляться в начало списка карточек.
5. После нажатия кнопки «Сохранить» окно добавления карточки должно автоматически закрываться.
6. Если хотя бы одно из полей не прошло валидацию, кнопка «Сохранить» должна быть неактивной. Если оба поля прошли — активной.

**3. Лайк карточки**

![Лайк](https://code.s3.yandex.net/qa/schemes/project1_mesto_4.png)

У пользователя должна быть возможность лайкать карточки.

1. У карточки должна быть кнопка лайка.
2. Кнопка «лайк» — сердечко.
3. Если лайкнуть карточку, сердечко поменяет цвет.

**4. Удаление карточки**

![Удаление](https://code.s3.yandex.net/qa/schemes/project1_mesto_5.png)

У пользователя должна быть возможность удалять карточки.

1. У карточек должна быть кнопка удаления.
2. Кнопка «удалить» — классическая урна.
3. Карточка должна удаляться при клике на эту иконку.

**5. Просмотр фотографий карточки**

![Просмотр](https://code.s3.yandex.net/qa/schemes/project1_mesto_6.png)

У пользователя должна быть возможность просмотра фотографий.

1. Режим просмотра открывается нажатием на картинку и закрывается кликом на крестик.
2. Вёрстка адаптивная, без полосы прокрутки при изменении ширины окна.

**6. Плавное открытие и закрытие окон**

Все окна должны открываться и закрываться плавно: проявляться из прозрачности и уходить в неё при закрытии.

**7. Закрытие окон нажатием на Esc**

Окна должны закрываться нажатием на клавишу Esc.

***

</details>

**2. Загрузи тест-кейсы и изучи их.**

Тест-кейсы написаны другим тестировщиком

**3. Протестируй приложение Mesto по тест-кейсам.**

**4. Подведи итоги работы**

### Решение

[Тест-кейсы](https://docs.google.com/spreadsheets/d/1X3Bk9FFjG6eUiCkcrIFGgmVR0KKV1N4WfnOE-fbOH-k/edit?usp=sharing)

[Баг-репорты](https://docs.google.com/spreadsheets/d/1QJdaj5ZbpnOMHBPlNqsAA4owx1sZiA4ZEqHTghGqih4/edit?usp=sharing)

Итог: Удалось найти 9 багов. Не рекомендую выпускать в релиз, т.к. имеется критический баг и не выполняется важная функция приложения.

### Задание 2. Ретест багов

**1. Изучи список баг-репортов, которые нашли другие тестировщики в сервисе Mesto.**

**2. Убедись, что разработчики исправили баги: используй тестовый стенд и выполни ретест.**

### Решение

[Баг-репорты](https://docs.google.com/spreadsheets/d/1RYJUmewlcQLwsKowlSqQ76YztEWC2xIRltNBJEXiz44/edit?usp=sharing)

Замечания: Отсутствовал элемент “Окружение”. Названия БР неполные или плохо отражают суть проблемы. Можно добавить скрины ошибок. Можно было добавить ссылки в шагах воспроизведения.
Итог: Не все баги исправлены, а также найдены новые.

## Функциональные UI-автотесты по чек-листам проекта [id.mail.ru](https://id.mail.ru)
### Чек-лист на страницу [id.mail.ru/profile](https://id.mail.ru/profile)
#### 1. Загрузка аватарки

- [ ] Нельзя загружать фотографию меньше 160px по ширине и высоте
- [ ] Нельзя загружать документы форматов не JPG, PNG, GIF или BMP.
- [ ] Загрузка фотографии формата jpg 
- [ ] Загрузка фотографии формата bmp 
- [ ] Загрузка фотографии формата gif 
- [ ] Загрузка аватарки открывается по нажатию и на аватарку
- [ ] Загрузка аватарки открывается по нажатию на кнопку "Изменить фото"

#### 1.1 Попап при загрузки аватарки меньше 160px по ширине и высоте

- [ ] При нажатии на крестик попап закрывается
- [ ] При нажатии "повторить" происходит повторная загрузка аватарки
- [ ] При нажатии "отменить" попап закрывается

#### 2. Поле Имя Фамилия Никнейм

- [x] Кириллица
- [x] Латиница
- [x] Cлова из <= 40 символ
- [x] Слова из > 40 символа - ошибка

#### 3.  День рождения

- [ ] Учитывается високосный год
- [ ] Нельзя указывать день рождения в будущем

#### 4. Пол

- [x] поменять пол можно

#### 5.  Поле Город

- [x] Нельзя ввести город на английском/несуществующий город
- [x] Ввод существующего города на русском
- [x] Есть автокомплит города

#### 6. Кнопки

- [x] Кнопка "сохранить" сохраняет изменения
- [x] Кнопка "отмена" не сохраняет изменения 
- [x] При нажатии на кнопку "сохранить", если поле (пункт 2) пустое, появится ошибка
## Функциональные UI-автотесты по чек-листам проекта [id.mail.ru](https://id.mail.ru)
### Запуск
1.  ./hub.sh
2.  ./node.sh
3.  LOGIN=<> PASSWORD=<> BROWSER='FIREFOX' [optional] python3 run_tests.py

**При создании тестового аккаунта важно зарегистрировать номер, а затем добавить резервный номер** 

### Чек-лист на страницу [id.mail.ru/profile](https://id.mail.ru/profile)

*Исполнитель: Кузнецова Анастасия*  

#### 1. Поле Имя Фамилия Никнейм

- [x] Кириллица
- [x] Латиница
- [x] Cлова из <= 40 символ
- [x] Слова из > 40 символа - ошибка

#### 2.  День рождения

- [x] Учитывается високосный год
- [x] Нельзя указывать день рождения в будущем

#### 3. Пол

- [x] поменять пол можно

#### 4.  Поле Город

- [x] Нельзя ввести город на английском/несуществующий город
- [x] Ввод существующего города на русском
- [x] Есть автокомплит города

#### 5. Кнопки

- [x] Кнопка "сохранить" сохраняет изменения
- [x] Кнопка "отмена" не сохраняет изменения 
- [x] При нажатии на кнопку "сохранить", если поле (пункт 2) пустое, появится ошибка

#### 6. Загрузка аватарки

- [X] Нельзя загружать фотографию меньше 160px по ширине и высоте
- [X] Нельзя загружать документы форматов не JPG, PNG, GIF или BMP.
- [X] Загрузка фотографии формата jpg 
- [x] Загрузка фотографии формата bmp 
- [x] Загрузка фотографии формата gif 

#### 6.6 Попап при загрузки аватарки меньше 160px по ширине и высоте

- [x] При нажатии на крестик попап закрывается
- [X] При нажатии "отменить" попап закрывается

### Чек-лист на страницу [id.mail.ru/contacts](https://id.mail.ru/contacts)

*Исполнитель: Спиридонова Александра*  

#### 1. Проверка функциональности добавления телефона

- [x] Удаление привязанного номера телефона 
- [x] Удаление еще не проверенного номера телефона 

#### 2. Проверка функциональности добавления почтового адреса

- [x] Добавление резервного почтового адреса (при их отсутствии)
- [x] Добавление резервного почтового адреса (при наличии)
- [ ] Добавление несуществующего почтового адреса (позволяет добавить некорректный email)
- [x] Удаление резервного почтово.го адреса

#### 3. Проверка всплывающего окна добавления телефона

- [x] Ввод невалидного номера (валидируется)
- [x] Ввод валидного номера  (переход на окно подтверждения кода)
- [x] Выбор префикса телефона для другой страны
- [x] Отмена добавления номера
- [x] Закрытие окна при нажатии на крестик

#### 4. Проверка всплывающего окна добавления телефона

- [x] Ввод невалидного кода (валидируется)
- [x] Подтверждение с пустым полем (просит ввести код)
- [x] Проверка ссылки изменения выбранного номера (возврат к окну добавления номера)
- [x] Закрытие окна при нажатии на крестик

#### 5. Проверка всплывающего окна добавления почтового адреса

- [x] Ввод невалидного почтового адреса (например,"ыыы", "a@.") (валидируется)
- [x] Ввод валидного почтового адреса (возврат на основную страницу)
- [x] Отмена добавления email
- [x] Закрытие окна при нажатии на крестик

#### 6. Проверка отображения сохраненных данных

- [x] Обновление вкладки 
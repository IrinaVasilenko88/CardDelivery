[![Build status](https://ci.appveyor.com/api/projects/status/1dcoq5k3n5fpia8h?svg=true)](https://ci.appveyor.com/project/IrinaVasilenko88/carddelivery)

# Обучение в Нетологии.

## Домашнее задание по курсу Автоматизированное тестирование

## Тема: Selenide

Автоматизирование тестирования формы заказа доставки карты(приложение ```app-card-delivery.jar```) с требованиями к содержимому полей:

![](https://github.com/netology-code/aqa-homeworks/blob/aqa4/selenide/pic/order.png)

- Город - один из административных центров субъектов РФ
- Дата - не ранее трёх дней с текущей даты
- Поле Фамилия и имя - разрешены только русские буквы, дефисы и пробелы
- Поле телефон - только цифры (11 цифр), символ + (на первом месте)
- Флажок согласия должен быть выставлен
- Состояние загрузки не должно длиться более 15 секунд.

Условия: если все поля заполнены корректно, то форма переходит в состояние "Загрузки":

![](https://github.com/netology-code/aqa-homeworks/blob/aqa4/selenide/pic/loading.png)

После успешной отправки формы (завершения бронирования) появится всплывающее окно об успешном завершении бронирования:

![](https://github.com/netology-code/aqa-homeworks/blob/aqa4/selenide/pic/popup.png)

**Для запуска проекта:**
1. Склонировать проект из репозитория командой 

```
git clone https://github.com/IrinaVasilenko88/CardDelivery.git
``` 
2. Открыть склонированный проект в Intellij IDEA
3. Открыть в терминале каталог ```artifacts```
4. Для запуска приложения ввести команду ```java -jar app-card-delivery.jar```
5. Для запуска в браузере ввести ссылку http://localhost:9999/
6. Запустить команду ```gradlew test```

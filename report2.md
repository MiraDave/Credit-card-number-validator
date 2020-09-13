# Отчёт о тестировании Credit Card Number Validator

13.09.2020 было проведено функциональное тестирование приложения Credit Card Number Validator

На тестирование затрачено: 4 часа

В результате тестирования выявлены следующие дефекты:

* [Ошибка при валидации карт Visa, Discover, JCB c 19-ным номером](https://github.com/MiraDave/Credit-card-number-validator/issues/1#issue-700615400)
* [Ошибка валидации карт American Express](https://github.com/MiraDave/Credit-card-number-validator/issues/2)
* [Невалидная карта Visa проходит валидацию](https://github.com/MiraDave/Credit-card-number-validator/issues/3)

**Описание процесса тестирования**

В процессе тестирования использовались следующие артефакты:

* Сайт [freeformatter](https://www.freeformatter.com/credit-card-number-generator-validator.html)

В качестве тестовых данных использовались данные с сайта [freeformatter](https://www.freeformatter.com/credit-card-number-generator-validator.html):

*Валидные номера карт*
* 4024007192953494
* 4158210551704921246
* 6011499337096935
* 6011844406925843955
* 3541500504202556
* 3545229906276964917
* 373524321004499
* 375168592684320

*Невалидные номера карт*
* 0
* -7
* N
* 67633333333335
* 4024007I92953494
* 4000000000000002


Тестирование производилось в следующем окружении:
* Windows 10 x64
* Java  "11.0.8" 2020-07-14
* Приложение IntelliJ IDEA
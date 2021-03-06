# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

17.05.2021 - 18.05.2021 было проведено смоук-тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 1 час

В результате тестирования выявлены следующие дефекты:
* [Валидатор не принимает 17-значные номера карт Laser](https://github.com/BudnikovaNastiya/Java-1.1-1/issues/2)
* [Валидатор не принимает 15-значные номера карт JCB Co Inc](https://github.com/BudnikovaNastiya/Java-1.1-1/issues/1)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* Генератор номеров кредитных карт

В качестве тестовых данных использовались данные с https://names.igopaygo.com/ru/Кредитные-карты
* Сгенерированные 16-значные номера карт Viza и MasterCard

Viza 

4024007132069641 Expected Result: OK
4572380661764346 Expected Result: OK
4556857177190116 Expected Result: OK

MasterCard

5440383251933773 Expected Result: OK
5437426357510287 Expected Result: OK
5457509749514326 Expected Result: OK
* Сгенерированные 17-значные номера карт Laser

67090297216315756 Expected Result: OK
67093833419721031 Expected Result: OK
63049263156801909 Expected Result: OK
* Сгенерированные 15-значные номера карт JCB Co Inc

210063452185428 Expected Result: OK
210067475395120 Expected Result: OK
180062458190768 Expected Result: OK

Тестирование производилось в следующем окружении:
* MacBook Pro (Retina, 13-inch, Late 2013), macOS Версия 10.15.7 (Выпуск 19H15) 10.15.7 64-bit 
* Java 11.0.11
* IntelliJ IDEA 2021.1.1

# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

27.10.2020 было проведено дымовое тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 15 минут

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Руководство по установке IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md)
* [Код](https://github.com/netology-code/javaqa-homeworks/tree/master/intro#%D0%B7%D0%B0%D0%B4%D0%B0%D1%87%D0%B0-2---credit-card-number-validator) программы Credit Card Number Validator

В качестве тестовых данных использовались примеры валидных номеров карт с сайта генератора номеров карт - [Get Credit Card Numbers](https://www.getcreditcardnumbers.com/):
* Visa 
```
4916060850394221 (result is OK)
4485849054275892 (result is OK)
4375019155548414 (result is OK) 
```

* MasterCard
```
5196150915201665 (result is OK)
5461930206783499 (result is OK)
5218884613547490 (result is OK)
```
* American Express
```
344363487646579 (result is FALSE)
342143533672544 (result is FALSE)
376132980396417 (result is FALSE)
```
* JCB
```
3158028687074372 (result is OK)
3096939838412417 (result is OK)
3528515016392478 (result is OK)
```
* Maestro
```
63637707336050 (result is FALSE)
5611730747849861 (result is FALSE)
6198252127521008259 (result is FALSE)
```

Тестирование производилось в следующем окружении:
* Windows 10 Pro
* openjdk ver.11.0.9
* Google Chrome ver.86.0.4240.111
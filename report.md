# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

27.10.2020 было проведено функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 20 минут

В результате тестирования выявлены следующие дефекты:
* [Не проходят валидацию номера карт American Express](https://github.com/Alex-nikiforova/java_HW_1.1_2/issues/1)
* [Не проходят валидацию номера карт Diners Club](https://github.com/Alex-nikiforova/java_HW_1.1_2/issues/2)


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
* Visa Electron:
```
4026675070732368 (result is OK)
4508610819931333 (result is OK)
4026743357893897 (result is OK)
```
* MasterCard
```
5196150915201665 (result is OK)
5461930206783499 (result is OK)
5218884613547490 (result is OK)
```
* American Express
```
344363487646579 (result is OK)
342143533672544 (result is OK)
376132980396417 (result is OK)
```
* JCB
```
3158028687074372 (result is OK)
3096939838412417 (result is OK)
3528515016392478 (result is OK)
```
* Maestro
```
6762107168059010 (result is OK)
6304624391249809 (result is OK)
0604281906897596 (result is OK)
```
* Diners Club
```
30340870094095 (result is OK)
38050725104732 (result is OK)
36560629396186 (result is OK)
```
Тестирование производилось в следующем окружении:
* Windows 10 Pro
* openjdk ver.11.0.9
* Google Chrome ver.86.0.4240.111
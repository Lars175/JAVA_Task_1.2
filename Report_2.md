# Отчёт о тестировании Credit Card Number Validator

### Краткое описание

<27/04/2020> - <27/04/2020> было проведено функциональное тестирование приложения <IntelliJ IDEA>.

На тестирование затрачено: 1 час.

В результате тестирования выявлены следующие дефекты:

[Issues](https://github.com/Lars175/JAVA_Task_1.2/issues/1#issue-611141051)



### Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:

- [Инструкция](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md) по установке IntelliJ IDEA
- [Форма](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/report.md) отчетности
- Тест-кейс

### Предварительные условия:

- Установить приложение IntelliJ IDEA 
- Перейти на [сайт](https://creditcardgenerator.com/visa-credit-card-generator/) генератора кредитных карт


### Шаги:

1. Открыть IntelliJ IDEA

2. Создать новый проект, добавить в открывшемся окне [код](https://github.com/Lars175/Krevetka/blob/master/Java.md)

3. Открыть сайт, сгенерировать номера карт

4. В строку String number = "6221433079697333",  указать номер карты без пробела

5. Запустить код, нажав shift+F10

6. Проверить результат.

7. Повторить шаги 4-6 с разными видами платежных систем.

### Ожидаемый результат:

- 4348281973645970, VISA  Result is OK
- 5557080978870358, MasterCard Result is OK
- 3873677396331798, DCI Result is OK
- 6221433079697333, Discover Result is OK
- 376419615904586, American Express Result is OK
- 6304523084714725, Maestro Result is OK
- 3560379179489467, JCB Result is OK
- 6267729113527088, China UnionPay Result is OK

### Фактический результат:

- 376419615904586, American Express **Result is FAIL**
- 4348281973645970, VISA  Result is OK
- 5557080978870358, MasterCard Result is OK
- 3873677396331798, DCI Result is OK
- 6221433079697333, Discover Result is OK
- 6304523084714725, Maestro Result is OK
- 3560379179489467, JCB Result is OK
- 6267729113527088, China UnionPay Result is OK

В качестве тестовых данных использовались данные [сайта](https://creditcardgenerator.com/visa-credit-card-generator/) генератора кредитных карт:

- 4348281973645970, VISA 
- 5557080978870358, MasterCard
- 3873677396331798, DCI
- 6221433079697333, Discover
- 376419615904586, American Express 
- 6304523084714725, Maestro 
- 3560379179489467, JCB 
- 6267729113527088, China UnionPay


### Тестирование производилось в следующем окружении:

OS - Win 10 PRO ver. 1709, build 16299.1087

Java version 11.0.7

IntelliJ IDEA 2020.1 Build #IC-201.6668.121 version 11.0.6+8-b576.25 amd64

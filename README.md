# forexprostools_database
База данных экономических новостей с Forexprostools.com 

### Описание

Данный репозиторий содержит исторические данные экономического календаря, который можно просмотреть здесь: [https://www.investing.com/webmaster-tools/economic-calendar](https://www.investing.com/webmaster-tools/economic-calendar)

Данные представлены в формате *json*. Данные за каждый день записаны в отдельные файлы, начиная с 1970 года. Имена файлов сгенерированы из даты новостей, которые они содержат, например *1980_10_3.json* означает, что данный файл содержит экономические новости за 1980 год 3 числа 10 месяца.

Пример содержимого файла:

```json
[
    {
        "actual": 196.0,
        "country": "United States",
        "currency": "USD",
        "name": "Nonfarm Payrolls (Oct)",
        "previous": 103.0,
        "timestamp": 1068208200,
        "volatility": 2
    },
    {
        "actual": 160.0,
        "country": "United States",
        "currency": "USD",
        "name": "U.S. Baker Hughes Oil Rig Count",
        "previous": 161.0,
        "timestamp": 1068224400,
        "volatility": 1
    },
    {
        "actual": -3.0,
        "country": "United States",
        "currency": "USD",
        "name": "CFTC Crude Oil speculative net positions",
        "previous": 27.9,
        "timestamp": 1068237000,
        "volatility": 1
    }
]
```

Сила новости отражена в переменной *volatility*, которая может принимать значение от 0 до 2. 

### Полезные ссылки

Использовать данные новостей в программе, написанной с использованием C++11 можно при помощи библиотеки: [https://github.com/NewYaroslav/forexprostools-cpp-api](https://github.com/NewYaroslav/forexprostools-cpp-api)

 
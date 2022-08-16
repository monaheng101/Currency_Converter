# Currency Converter

A simple program for converting currency in real-time using the Forex Python Library. the program is controlled by a simple command-line medu that also allows listing all currencies and handles errors. The Forex-Python library uses API calls to directly get the currency conversion rate and the uses the 'convert()' function to convert one currency to another.

Example from [w3schools](https://www.w3schools.in/python/examples/real-time-currency-converter):

### Code Sample:

    from forex_python.converter import CurrencyRates

    cr = CurrencyRates()

    amount = int(input("Please enter the amount you want to convert: "))

    from_currency = input("Please enter the currency code that has to be converted: ").upper()

    to_currency = input("Please enter the currency code to convert: ").upper()

    print("You are converting", amount, from_currency, "to", to_currency,".")

    output = cr.convert(from_currency, to_currency, amount)

    print("The converted rate is:", output)

### Program Output:

    Please enter the amount you want to convert: 1
    Please enter the currency code that has to be converted: USD
    Please enter the currency code to convert: INR
    You are converting 1 USD to INR.
    The converted rate is: 77.58766511451107

### Install forex-python

    pip install forex-python


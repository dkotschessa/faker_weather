
# STUB copied from airtravel do not use yet


# Weather Data provider for Faker

A java example:https://dius.github.io/java-faker/apidocs/com/github/javafaker/Weather.html

## Acknowlegements


`faker_weather` is a provider for the `Faker` Python package.  

## Description

`faker_weather` provides weather related fake data for testing purposes.  


## Installation

Install with pip:

``` bash
pip install faker_weather

```

Add as a provider to your Faker instance:

``` python

from faker import Faker
from faker_airtravel import WeatherProvider
fake.add_provider(WeatherProvider)

```

If you already use faker, you probably know the conventional use is:

```python
fake = Faker()

```

### TODO update examples below
### Airport Object

``` python
>>> fake.airport_object()
{'Airport': 'Tocumen International Airport',
'iata': 'PTY',
'icao': 'MPTO',
'City': 'Tocumen',
'State': 'Panama',
'Country': 'Panama'}

>>> fake.airport_name()
'Lisbon Airport'

```

### Airport Codes (IATA and ICAO)

``` python
>>> fake.airport_iata()
'LSC'

>>> fake.airport_icao()
'KOKC'
```

### Airlines
```
>>> fake.airline()
'Sichuan Airlines'

```

### Flight

The flight object is an example of how the data might be combined to create larger structures, and may not be the exact format you need.
However it does have the advantage that it will never choose the same 'origin' and 'destination' object.

```
>>>fake.flight()

{'airline': 'Maya Island Air',
 'origin': {'Airport': 'Noi Bai Airport',
  'iata': 'HAN',
  'icao': 'VVNB',
  'City': 'Hanoi',
  'State': 'Ha Noi',
  'Country': 'Vietnam'},
 'destination': {'Airport': 'Geneva Airport',
  'iata': 'GVA',
  'icao': 'LSGG',
  'City': 'Geneva',
  'State': 'Canton of Geneva',
  'Country': 'Switzerland'},
 'stops': 'non-stop',
 'price': 641}
 ```


 



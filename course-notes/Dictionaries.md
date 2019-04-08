# Dictionaries


```bash
# python idle
>>> things = ['a', 'b', 'c', 'd']
>>> print(things[1])
b
>>> things[1] = 'z'
>>> print(things[1])
z
>>> things
['a', 'z', 'c', 'd']
```


---
## dict
```bash
>>> stuff = {'name': 'Zed', 'age': 39, 'height': 6 * 12 + 2}
>>> print(stuff['name'])
Zed
>>> print(stuff['age'])
39
>>> print(stuff['height'])
74
>>> stuff['city'] = "SF"
>>> print(stuff['city'])
SF
```


endi *stuff* dictionary ni yangilaymiz

```bash
>>> stuff[1] = "Wow"
>>> stuff[2] = "Neato"
>>> print(stuff[1])
Wow
>>> print(stuff[2])
Neato
```

endi q'shgan narsalarmizni dictionary dan o'chiramiz
```bash
>>> del stuff['city']
>>> del stuff[1]
>>> del stuff[2]
>>> stuff
{'name': 'Zed', 'age': 39, 'height': 74}
``` 




# dictionary Example

yangi fayl yaratib tekshirib ko'ring
```python
# create a mapping of state to abbreviation
viloyatlar = {
    'Samarqand': 'SM',
    'Buxoro': 'BX',
    'Xorazm': 'XM',
    'Sirdaryo': 'SO',
    'Fa\'rg\'ona': 'FG'
}

# create a basic set of viloyatlar and some shaharlar in them
shaharlar = {
    'XM': 'Xiva',
    'SO': 'Guliston',
    'FG': "Marg'ilon"
}

# add some more shaharlar
shaharlar['BX'] = 'Bukhara city'
shaharlar['SM'] = 'Samarkand city'

# print  shaharlar
print('-' * 10)
print("Buxoro viloyatidagi shahar: ", shaharlar['BX'])
print("SM viloyatidagi shahar: ", shaharlar['SM'])

# print some viloyatlar
print('-' * 10)
print("Fa\'rg\'onaning abbrevaturasi:", viloyatlar['Fa\'rg\'ona'])
print("Sirdaryo's abbrevaturasi: ", viloyatlar['Sirdaryo'])

# do it by using the state then shaharlar dict
print('-' * 10)
print("Fa\'rg\'ona dagi shahar: ", shaharlar[viloyatlar['Fa\'rg\'ona']])
print("Sirdaryo dagi shahar", shaharlar[viloyatlar['Sirdaryo']])

# print viloyatlar abbreviation
print('-' * 10)
for state, abbrev in list(viloyatlar.items()):
    print(f"{state} is abbreviated {abbrev}")


# print every city in state
print('-' * 10)
for abbrev, city in list(shaharlar.items()):
    print(f"{abbrev} has the city {city}")


# now do both at the same time
print('-' * 10)
for viloyat, abbrev in list(viloyatlar.items()):
    print(f"{viloyat} ning abbrevaturasi {abbrev}")
    print(f"va {shaharlar[abbrev]} shahari bor")
    print('-' * 10)


# safely get a abbreviation by state that might not be there
state = viloyatlar.get('Toshkent')
if not state:
    print("Kechirasiz, Toshkent yo'q")

# get a city with a default value
shahar = shaharlar.get('TS', 'Mavjud Emas')
print(f"'TS' Uchun shahar: {shahar}")
```

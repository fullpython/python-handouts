# Loops and Lists

# **for** loop
```python
the_count = [1, 2, 3, 4, 5]
fruits = ['apples', 'oranges', 'pears', 'apricots']
change = [1, 'pennies', 2, 'dimes', 3, 'quarters']


print("Bu yerda mevalar: ", fruits)
print(f'Mevalar soni {the_count} tadan') # Bu yerda stringni ichiga o'zgaruvchi (the_count) joylashtiryapmiz


for number in the_count:
    print(f"This is count {number}")

for fruit in fruits:
    print(f"A fruit of type: {fruit}")

for i in change:
    print(f"I got {i}")


elements = []

for i in range(0, 6):
    print(f"Adding {i} to the list.")
    # append bu listlar tushunadigan funksiya [list obyektining funksiyasi]
    elements.append(i)

for i in elements:
    print(f"Element was: {i}")

```




## **while** loop

```python
i = 0
numbers = []
while i < 6:
    print(f"Tepada i ning qiymati {i}")
    numbers.append(i)
    i = i + 1
    print("Hozir Sonlar: ", numbers)
    print(f"Pastda i ning qiymati {i}")


print("Sonlar: ")

for num in numbers:
    print(num)
```
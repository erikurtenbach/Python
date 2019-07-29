# Python Basics

## Functions
Retorna o valor após return ou apenas realiza a operação definida <br>
Ex:
```
def least_difference(a, b, c):
    diff1 = abs(a - b)
    diff2 = abs(b - c)
    diff3 = abs(a - c)
    return min(diff1, diff2, diff3)
 ```
## Comparações
```
Operation	Description		Operation	Description
a == b	a equal to b		a != b	a not equal to b
a < b	a less than b		a > b	a greater than b
a <= b	a less than or equal to b		a >= b	a greater than or equal to b
```
## Condicionais
```
def inspect(x):
    if x == 0:
        print(x, "is zero")
    elif x > 0:
        print(x, "is positive")
    elif x < 0:
        print(x, "is negative")
    else:
        print(x, "is unlike anything I've ever seen...")
  ```
  
 ## Lists
 Armazena valores
 ex:
 ```
 planets = ['Mercury', 'Venus', 'Earth', 'Mars', 'Jupiter', 'Saturn', 'Uranus', 'Neptune']
 hands = [['J', 'Q', 'K'], ['2', '2', '2'], ['6', 'A', 'K']]
 ```
 
 ```
 planets[0]
'Mercury'

planets[0:3]
['Mercury', 'Venus', 'Earth']

planets.append('Pluto') - "adiciona ao ultimo item da lista"

planets.index('Earth')
2
```

# Data types
---

| Type    | Ma'lumot                                                 | Misol                   |
| ------- | :------------------------------------------------------- | ----------------------- |
| True    | True boolean qiymat                                      | True or False == True   |
| False   | False boolean qiymat                                     | False and True == False |
| None    | "Hech narsa" yoki "qiymat yo'q" degan ma'noni bildiradi  | x = None                |
| bytes   | Byte larni o'zida saqlaydi, text, PNG, file va boshqalar | x = b"hello"            |
| strings | text datani o'z ichida saqlaydi                          | x = "hello"             |
| numbers | integer(butun son)larni o'z ichida saqlaydi              | i = 100                 |
| floats  | decimal(haqiqiy son)larni o'z ichida saqlaydi            | i = 10.389              |
| lists   | Narsalar listini o'z ichida saqlaydi                     | j = [1,2,3,4]           |
| dicts   | key=value narsalar bo'gliqligini saqlaydi                | e = {'x': 1, 'y': 2}    |



---
# Eski stil formatlari
| Escape | Description                            | Example                         |
| ------ | -------------------------------------- | ------------------------------- |
| %d     | Decimal integers (not floating point). | "%d" % 45 == '45'               |
| %i     | Same as %d.                            | "%i" % 45 == '45'               |
| %o     | Octal number.                          | "%o" % 1000 == '1750'           |
| %u     | Unsigned decimal.                      | "%u" % -1000 == '-1000'         |
| %x     | Hexadecimal lowercase.                 | "%x" % 1000 == '3e8'            |
| %X     | Hexadecimal uppercase.                 | "%X" % 1000 == '3E8'            |
| %e     | Exponential notation, lowercase ’e’. | "%e" % 1000 == '1.000000e+03'   |
| %E     | Exponential notation, uppercase ’E’. | "%E" % 1000 == '1.000000E+03'   |
| %f     | Floating point real number.            | "%f" % 10.34 == '10.340000'     |
| %F     | Same as %f.                            | "%F" % 10.34 == '10.340000'     |
| %g     | Either %f or %e, whichever is shorter. | "%g" % 10.34 == '10.34'         |
| %G     | Same as %g but uppercase.              | "%G" % 10.34 == '10.34'         |
| %c     | Character format.                      | "%c" % 34 == '"'                |
| %r     | Repr format (debugging format).        | "%r" % int == "<type 'int'>"    |
| %s     | String format.                         | "%s there" % 'hi' == 'hi there' |
| %%     | A percent sign.                        | "%g%%" % 10.34 == '10.34%'      |

---


# Operatorlar
| Operator | Description                   | Example                     |
| -------- | ----------------------------- | --------------------------- |
| +        | Addition                      | 2 + 4 == 6                  |
| -        | Subtraction                   | 2 - 4 == -2                 |
| *        | Multiplication                | 2 * 4 == 8                  |
| **       | Power of                      | 2 ** 4 == 16                |
| /        | Division                      | 2 / 4 == 0.5                |
| //       | Floor division                | 2 // 4 == 0                 |
| %        | String interpolate or modulus | 2 % 4 == 2                  |
| <        | Less than                     | 4 < 4 == False              |
| >        | Greater than                  | 4 > 4 == False              |
| <=       | Less than equal               | 4 <= 4 == True              |
| >=       | Greater than equal            | 4 >= 4 == True              |
| ==       | Equal                         | 4 == 5 == False             |
| !=       | Not equal                     | 4 != 5 == True              |
| ( )      | Parenthesis                   | len('hi') == 2              |
| [ ]      | List brackets                 | [1,3,4]                     |
| { }      | Dict curly braces             | {'x': 5, 'y': 10}           |
| @        | At (decorators)               | @classmethod                |
| ,        | Comma                         | range(0, 10)                |
| :        | Colon                         | def X():                    |
| .        | Dot                           | self.x = 10                 |
| =        | Assign equal                  | x = 10                      |
| ;        | semi-colon                    | print("hi"); print("there") |
| +=       | Add and assign                | x = 1; x += 2               |
| -=       | Subtract and assign           | x = 1; x -= 2               |
| *=       | Multiply and assign           | x = 1; x *= 2               |
| /=       | Divide and assign             | x = 1; x /= 2               |
| //=      | Floor divide and assign       | x = 1; x //= 2              |
| %=       | Modulus assign                | x = 1; x %= 2               |
| **=      | Power assign                  | x = 1; x **= 2              |
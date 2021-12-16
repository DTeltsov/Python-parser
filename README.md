# Python-parser
Parser считывает py-файл построчно и с помощью Regex определяет тот или иной фрагмент кода к категории.
### Например:
Вот код на Python:
```
print('X_1: {0}   Y_1: {1}   Z_1 {2}'.format(x,y,z))
```

А вот что нам Parser выведет в консоль

```
print - Keyword
( - Punctuation
'X_1: {0}   Y_1: {1}   Z_1 {2}' - String
. - Punctuation
format - Keyword
( - Punctuation
x - Identifier
, - Punctuation
y - Identifier
, - Punctuation
z - Identifier
) - Punctuation
) - Punctuation
```

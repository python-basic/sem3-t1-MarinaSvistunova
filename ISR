
# 1.2. Разработка скрипта, вычисляющего сумму первых n-членов арифметической прогрессии (использование функций,
# условных операторов). Формирование отчета по выполнению задания и размещение его в портфолио,
# персональном репозитории.

def arithmeticProgression(a_1, d, n):
    a_n = a_1 + (n - 1)*d
    S_n = n*(a_1 + a_n)/2
    return S_n

# print(arithmeticProgression(5, 6, 1000)) #3002000

# 1.3. Разработка скрипта, позволяющего вычислить площадь треугольника с помощью формулы Герона. Формирование
# отчета по выполнению задания и размещение его в портфолио, персональном репозитории.

from math import sqrt
def heronsFormula(a, b, c):
    p = (a + b + c)/2
    S = sqrt(p*(p - a)*(p - b)*(p-c))
    return S

print(heronsFormula(6, 5, 2.2)) #5.28

# 1.4. Создание сценария, вычисляющего операции сложения, вычитания, умножения, деления для двух операндов.
# Формирование отчета по выполнению задания и размещение его в портфолио, персональном репозитории.

def culc(strForCulc):
    output = strForCulc
    str2 = list(output)
    operators ={
        '+': (lambda x, y: x + y),
        '-': (lambda x, y: x - y),
        '*': (lambda x, y: x * y),
        '/': (lambda x, y: x / y),
        '^': (lambda x, y: x ** y)
    }
    operator = ''
    num = ''
    for i in str2:
        if i in '0123456789.' and operator == '':
            num += i
        elif operator == '':
            x = int(num)
            if i in operators:
                operator = i
            num = ''
        else:
            num += i
    y = int(num)
    output += ' = '
    lr = (operators.get(operator)(x, y))
    output += str(lr)
    return output

print(culc("4+5"))
print(culc("4*5"))
print(culc("4/5"))
print(culc("4-5"))
print(culc("4^5"))
# print(culc(input()))

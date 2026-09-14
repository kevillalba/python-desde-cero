# 🐍 Python para Finanzas, Economía y Business Intelligence

## Guías de aprendizaje 01, 02, 03 y 04

**Nivel:** Principiante absoluto  
**Entorno:** Google Colab  
**Enfoque:** Finanzas, Economía, Business Intelligence y análisis de datos

---

# 📚 Índice

1. [Guía 01 — Variables](#guía-01--variables)
2. [Guía 02 — Tipos de datos](#guía-02--tipos-de-datos)
3. [Guía 03 — Operadores y expresiones](#guía-03--operadores-y-expresiones)
4. [Guía 04 — Estructuras de datos](#guía-04--estructuras-de-datos)

---

# Guía 01 — Variables

## 🎯 Objetivos

Al terminar esta guía podrás:

- Entender qué es una variable.
- Crear variables en Python.
- Asignar valores a variables.
- Modificar el valor de una variable.
- Utilizar variables para realizar cálculos.
- Mostrar información utilizando `print()`.
- Utilizar nombres de variables claros.
- Comprender por qué las variables son fundamentales en programación.
- Aplicar variables a problemas sencillos de Finanzas y Economía.

---

# 1. ¿Qué es programar?

Programar consiste en darle instrucciones a una computadora para que realice determinadas tareas.

Por ejemplo, imagina que quieres calcular cuánto dinero te queda después de recibir tu salario y pagar tus gastos.

Tienes:

```text
Ingresos:       $3,000
Arriendo:         $800
Alimentación:     $400
Transporte:      $200
```

Podrías hacer el cálculo manualmente:

```text
3,000 - 800 - 400 - 200 = 1,600
```

También puedes enseñarle a Python a realizar ese cálculo:

```python
income = 3000
rent = 800
food = 400
transport = 200

remaining = income - rent - food - transport

print(remaining)
```

Resultado:

```text
1600
```

La computadora realizó el cálculo siguiendo nuestras instrucciones.

---

# 2. ¿Qué es una variable?

Una variable es un **nombre que utilizamos para almacenar o referirnos a un valor**.

Por ejemplo:

```python
age = 21
```

Podemos leerlo como:

> La variable `age` contiene el valor `21`.

Otro ejemplo:

```python
name = "Alex"
```

Podemos leerlo como:

> La variable `name` contiene el texto `"Alex"`.

Otro ejemplo:

```python
balance = 2500
```

Significa:

> La variable `balance` contiene el valor `2500`.

---

# 3. Una variable como una caja

Una forma sencilla de imaginar una variable es como una caja que tiene una etiqueta.

```text
┌─────────────────┐
│       age       │
│       21        │
└─────────────────┘
```

La etiqueta es:

```text
age
```

El contenido es:

```text
21
```

Otro ejemplo:

```text
┌─────────────────┐
│     balance     │
│      2500       │
└─────────────────┘
```

Esto nos ayuda a entender que una variable tiene:

1. Un nombre.
2. Un valor.

---

# 4. Crear una variable

Para crear una variable utilizamos el signo:

```python
=
```

Por ejemplo:

```python
age = 21
```

El signo `=` significa **asignación**.

Estamos diciendo:

> Guarda el valor `21` y permite que podamos acceder a él mediante el nombre `age`.

Otro ejemplo:

```python
name = "Alex"
```

Y:

```python
balance = 5000
```

---

# 5. Tu primer programa

Copia el siguiente código en una celda de Google Colab:

```python
name = "Alex"
age = 20
city = "Miami"

print(name)
print(age)
print(city)
```

El resultado será:

```text
Alex
20
Miami
```

Acabas de crear tres variables:

```text
name
age
city
```

Cada una contiene información diferente.

---

# 6. ¿Qué hace `print()`?

`print()` sirve para mostrar información en pantalla.

Por ejemplo:

```python
print("Hello")
```

Resultado:

```text
Hello
```

También podemos mostrar una variable:

```python
name = "Alex"

print(name)
```

Resultado:

```text
Alex
```

También podemos mostrar varias variables:

```python
name = "Alex"
age = 20

print(name, age)
```

Resultado:

```text
Alex 20
```

---

# 7. Las variables pueden cambiar

Una variable puede recibir un nuevo valor.

Por ejemplo:

```python
balance = 1000

print(balance)
```

Resultado:

```text
1000
```

Ahora podemos cambiarla:

```python
balance = 1500

print(balance)
```

Resultado:

```text
1500
```

La variable `balance` ahora contiene `1500`.

---

# 8. Variables y cálculos

Las variables pueden utilizarse para realizar operaciones.

Por ejemplo:

```python
price = 100
quantity = 5

total = price * quantity

print(total)
```

Resultado:

```text
500
```

Aquí Python realizó:

```text
100 × 5 = 500
```

Lo importante es que el programa es mucho más fácil de entender porque utilizamos nombres que describen los datos.

---

# 9. Ejemplo financiero

Supongamos que recibes $4,000 al mes.

Tus gastos son:

- Arriendo: $1,200
- Alimentación: $500
- Transporte: $300

Podemos representarlo en Python:

```python
income = 4000
rent = 1200
food = 500
transport = 300
```

Ahora podemos calcular cuánto dinero queda:

```python
remaining = income - rent - food - transport

print(remaining)
```

Resultado:

```text
2000
```

---

# 10. Ejemplo de inversión

Supongamos que tienes una inversión de $10,000 y obtienes un rendimiento del 8%.

```python
investment = 10000
rate = 0.08
```

Calculamos la ganancia:

```python
profit = investment * rate

print(profit)
```

Resultado:

```text
800.0
```

La inversión generó $800 de ganancia.

---

# 11. Los nombres de las variables importan

Observa:

```python
x = 5000
y = 1000
z = x - y
```

El código funciona.

Sin embargo, es difícil saber qué representa cada variable.

Es mucho mejor:

```python
income = 5000
expenses = 1000
remaining = income - expenses
```

Ahora el código prácticamente se explica por sí mismo.

---

# 12. Utiliza nombres descriptivos

Ejemplos recomendados:

```python
monthly_income = 5000
total_expenses = 2500
account_balance = 10000
interest_rate = 0.05
student_name = "Alex"
```

Evita:

```python
a = 5000
b = 2500
c = 10000
r = 0.05
```

Cuando los programas sean más grandes, los nombres claros serán extremadamente importantes.

---

# 13. Variables con varias palabras

En Python normalmente utilizamos `snake_case`.

Ejemplo:

```python
monthly_income = 5000
```

Otros ejemplos:

```python
first_name = "Alex"
annual_income = 60000
account_balance = 5000
interest_rate = 0.05
total_expenses = 3000
```

No podemos escribir:

```python
monthly income = 5000
```

porque los espacios no son válidos en el nombre de una variable.

---

# 14. Variables con texto

Las variables también pueden almacenar texto:

```python
name = "Alex"
country = "United States"
currency = "USD"
```

El texto normalmente se escribe entre comillas.

Por ejemplo:

```python
name = "Alex"
```

Aquí:

```text
"Alex"
```

es texto.

---

# 15. Variables con números

También podemos almacenar números:

```python
age = 21
employees = 50
sales = 10000
```

Y números decimales:

```python
price = 19.99
interest_rate = 0.075
inflation = 0.032
```

En la siguiente guía aprenderemos que estos valores pertenecen a diferentes tipos de datos.

---

# 16. Variables booleanas

También podemos almacenar información que representa verdadero o falso:

```python
is_student = True
```

o:

```python
has_debt = False
```

Los valores posibles son:

```python
True
False
```

Estos valores serán muy importantes cuando aprendamos condiciones.

---

# 17. La función `type()`

Python tiene una función que permite saber qué tipo de dato contiene una variable:

```python
type()
```

Por ejemplo:

```python
age = 21

print(type(age))
```

Resultado:

```text
<class 'int'>
```

Todavía no necesitas memorizar qué significa `int`.

Lo estudiaremos en la siguiente guía.

---

# 🧪 Ejercicio 1 — Información personal

Crea las siguientes variables utilizando tus propios datos:

```text
name
age
city
country
```

Después imprime cada variable.

Ejemplo:

```python
name = "Alex"
age = 21
city = "Miami"
country = "United States"

print(name)
print(age)
print(city)
print(country)
```

### Reto

Agrega:

```text
favorite_subject
university
```

---

# 🧪 Ejercicio 2 — Finanzas personales

Imagina que tienes:

```text
Ingreso mensual:       $5,000
Arriendo:              $1,500
Alimentación:            $600
Transporte:              $300
Entretenimiento:         $250
```

Crea una variable para cada valor.

Después calcula cuánto dinero queda disponible.

Debes utilizar las variables.

Puedes comenzar:

```python
income = 5000
rent = 1500
food = 600
transport = 300
entertainment = 250

# Escribe tu cálculo aquí
```

---

# 🧪 Ejercicio 3 — Inversión

Tienes:

```text
Investment: $20,000
Annual return: 7%
```

Crea:

```python
investment = 20000
annual_return = 0.07
```

Calcula la ganancia:

```python
profit = ...
```

Después imprime el resultado.

---

# 🧩 Reto final — Mini análisis financiero

Una persona tiene:

```text
Ingresos:            $6,000
Housing:             $1,500
Food:                  $700
Transport:             $300
Entertainment:         $400
Other:                 $250
```

Crea todas las variables.

Calcula:

1. Total de gastos.
2. Dinero restante.
3. Porcentaje del ingreso que queda disponible.

Puedes comenzar:

```python
income = 6000

housing = 1500
food = 700
transport = 300
entertainment = 400
other = 250

# Escribe tus cálculos aquí
```

---

# 🎯 Resumen de la guía

En esta guía aprendiste:

- Una variable es un nombre asociado a un valor.
- `=` permite asignar un valor.
- `print()` muestra información.
- Las variables pueden utilizarse en cálculos.
- Una variable puede cambiar de valor.
- Es importante utilizar nombres descriptivos.
- Python trabaja con diferentes tipos de datos.

---

# Guía 02 — Tipos de datos

## 🎯 Objetivos

Al terminar esta guía podrás:

- Entender qué es un tipo de dato.
- Diferenciar texto, números y valores booleanos.
- Utilizar `str`, `int`, `float` y `bool`.
- Comprender `None`.
- Utilizar `type()`.
- Convertir datos de un tipo a otro.
- Entender por qué los tipos de datos son importantes.
- Aplicar estos conocimientos a Finanzas y Business Intelligence.

---

# 1. ¿Por qué existen los tipos de datos?

Imagina que tienes esta información:

```text
Nombre:             Alex
Edad:               21
Balance:            $2,500.75
¿Es estudiante?:    Sí
```

Aunque toda esta información puede almacenarse en variables, no toda representa el mismo tipo de información.

Tenemos:

```text
"Alex"       → texto
21           → número entero
2500.75      → número decimal
True         → verdadero/falso
```

Python necesita conocer el tipo de dato porque las operaciones que podemos realizar dependen del tipo de información.

---

# 2. Los principales tipos de datos

| Tipo | Nombre | Ejemplo |
|---|---|---|
| `str` | Texto | `"Alex"` |
| `int` | Número entero | `21` |
| `float` | Número decimal | `2500.75` |
| `bool` | Verdadero/Falso | `True` |
| `NoneType` | Ausencia de valor | `None` |

---

# 3. `str` — Texto

`str` significa **string**.

Representa texto.

Ejemplos:

```python
name = "Alex"
country = "United States"
currency = "USD"
stock_symbol = "AAPL"
```

Podemos comprobar el tipo:

```python
print(type(name))
```

Resultado:

```text
<class 'str'>
```

---

# 4. Las comillas importan

Observa:

```python
age = 21
```

Aquí `21` es un número.

Pero:

```python
age = "21"
```

Aquí `"21"` es texto.

Aunque visualmente parecen similares, Python los considera diferentes.

Podemos comprobarlo:

```python
age1 = 21
age2 = "21"

print(type(age1))
print(type(age2))
```

Resultado:

```text
<class 'int'>
<class 'str'>
```

---

# 5. ¿Por qué esto importa?

Observa:

```python
age = 21

next_year = age + 1

print(next_year)
```

Resultado:

```text
22
```

Tiene sentido porque estamos sumando números.

Ahora:

```python
age = "21"

next_year = age + 1

print(next_year)
```

Esto produce un error.

¿Por qué?

Porque Python está intentando hacer:

```text
texto + número
```

Los tipos de datos importan.

---

# 6. `int` — Números enteros

`int` representa números enteros.

Ejemplos:

```python
age = 21
employees = 50
products = 100
year = 2026
```

Podemos comprobarlo:

```python
print(type(age))
```

Resultado:

```text
<class 'int'>
```

---

# 7. `float` — Números decimales

`float` representa números que contienen decimales.

Ejemplos:

```python
price = 19.99
balance = 2500.50
interest_rate = 0.075
inflation = 0.032
```

Podemos comprobarlo:

```python
print(type(price))
```

Resultado:

```text
<class 'float'>
```

---

# 8. Finanzas: `int` y `float`

Esta diferencia es común en Finanzas.

Podemos tener:

```python
shares = 100
```

Tenemos 100 acciones.

Es un entero.

Pero:

```python
share_price = 125.50
```

El precio de una acción puede tener decimales.

Podemos calcular el valor de la inversión:

```python
shares = 100
share_price = 125.50

investment = shares * share_price

print(investment)
```

Resultado:

```text
12550.0
```

---

# 9. `bool` — Booleanos

Un booleano representa una condición que puede tener dos valores:

```python
True
False
```

Por ejemplo:

```python
is_student = True
has_debt = False
```

Podemos comprobarlo:

```python
print(type(is_student))
```

Resultado:

```text
<class 'bool'>
```

---

# 10. ¿Por qué son importantes los booleanos?

Porque permiten que un programa tome decisiones.

Por ejemplo:

```python
has_debt = True
```

Más adelante podremos escribir:

```python
if has_debt:
    print("The customer has debt")
```

Python ejecutará una acción dependiendo de si la condición es verdadera.

---

# 11. `None`

Existe un valor especial llamado:

```python
None
```

Representa la ausencia de un valor.

Por ejemplo:

```python
middle_name = None
```

Esto significa:

> No tenemos un segundo nombre registrado.

No significa que el texto sea `"None"`.

Podemos comprobarlo:

```python
print(type(middle_name))
```

Resultado:

```text
<class 'NoneType'>
```

---

# 12. Comparando diferentes tipos

Observa:

```python
name = "Alex"
age = 21
balance = 2500.50
is_student = True
middle_name = None
```

Tenemos:

| Variable | Valor | Tipo |
|---|---|---|
| `name` | `"Alex"` | `str` |
| `age` | `21` | `int` |
| `balance` | `2500.50` | `float` |
| `is_student` | `True` | `bool` |
| `middle_name` | `None` | `NoneType` |

Puedes comprobarlos:

```python
print(type(name))
print(type(age))
print(type(balance))
print(type(is_student))
print(type(middle_name))
```

---

# 13. Conversión de tipos

A veces recibimos información en un tipo de dato y necesitamos convertirla.

Esto se conoce como **conversión de tipos**.

---

# 14. Convertir texto a entero

Tenemos:

```python
age = "21"
```

Actualmente es texto.

Podemos convertirlo:

```python
age = int(age)
```

Ahora:

```python
print(type(age))
```

Resultado:

```text
<class 'int'>
```

---

# 15. Convertir texto a decimal

Tenemos:

```python
price = "19.99"
```

Podemos convertirlo:

```python
price = float(price)
```

Ahora `price` es un `float`.

```python
print(type(price))
```

---

# 16. Convertir un número a texto

También podemos hacer lo contrario:

```python
age = 21

age_text = str(age)
```

Ahora:

```python
print(type(age_text))
```

Resultado:

```text
<class 'str'>
```

---

# 17. Un ejemplo realista

Imagina que recibimos información desde un formulario:

```python
price = "100"
quantity = 5
```

`price` es texto.

Si queremos realizar una operación matemática, podemos convertirlo:

```python
price = int(price)

total = price * quantity

print(total)
```

Resultado:

```text
500
```

---

# 18. Finanzas

Imagina:

```python
investment = "25000"
return_rate = "0.08"
```

Ambos valores son texto.

Primero debemos convertirlos:

```python
investment = float(investment)
return_rate = float(return_rate)
```

Ahora podemos calcular:

```python
profit = investment * return_rate

print(profit)
```

Resultado:

```text
2000.0
```

---

# 19. ¿Por qué esto es importante en Business Intelligence?

En Business Intelligence y análisis de datos trabajaremos constantemente con información proveniente de:

- Excel.
- CSV.
- Bases de datos.
- APIs.
- Formularios.
- Sistemas empresariales.

Los datos pueden llegar con tipos incorrectos.

Por ejemplo:

```text
Price
"1200"
"1500"
"900"
```

Aunque parecen números, pueden estar almacenados como texto.

Si queremos hacer cálculos, tendremos que convertirlos correctamente.

Por eso entender los tipos de datos es fundamental.

---

# 🧪 Ejercicio 1 — Identificar tipos

Crea:

```python
name = "John"
age = 25
salary = 4500.75
has_car = True
phone_number = "3055551234"
```

Utiliza `type()` para descubrir el tipo de cada variable.

Antes de ejecutar el código, intenta adivinar los tipos.

---

# 🧪 Ejercicio 2 — Detectar un problema

Observa:

```python
income = "5000"
expenses = 2000

remaining = income - expenses

print(remaining)
```

Ejecuta el código.

¿Qué sucede?

### Pregunta

¿Por qué Python no puede realizar correctamente la operación?

### Pista

Debes convertir el tipo de `income`.

---

# 🧪 Ejercicio 3 — Conversión

Tienes:

```python
price = "150.50"
quantity = "3"
```

Convierte los valores correctamente y calcula:

```text
Total = precio × cantidad
```

Resultado esperado:

```text
451.5
```

---

# 🧪 Ejercicio 4 — Finanzas

Una inversión está representada por:

```python
investment = "25000"
return_rate = "0.08"
```

Convierte los valores apropiadamente y calcula:

```text
profit
```

Resultado esperado:

```text
2000
```

---

# 🧩 Reto — Analista financiero

Tienes:

```python
customer_name = "John"
age = "35"
annual_income = "72000"
investment = "15000"
return_rate = "0.06"
has_debt = True
```

Tu trabajo consiste en:

1. Identificar el tipo de cada variable.
2. Convertir los datos que necesiten conversión.
3. Calcular la ganancia de la inversión.
4. Calcular cuánto representa esa ganancia respecto a la inversión.
5. Mostrar los resultados.

El programa debería producir algo similar a:

```text
Customer: John
Age: 35
Annual income: 72000
Investment: 15000
Investment profit: 900
Return: 6%
Has debt: True
```

---

# 🎯 Lo que debes dominar

Antes de continuar debes comprender:

- Qué es `str`.
- Qué es `int`.
- Qué es `float`.
- Qué es `bool`.
- Qué es `None`.
- Por qué `"21"` y `21` son diferentes.
- Cómo utilizar `type()`.
- Cómo convertir datos utilizando `int()`.
- Cómo convertir datos utilizando `float()`.
- Cómo convertir datos utilizando `str()`.
- Por qué los tipos de datos son importantes al trabajar con información.

---

# Guía 03 — Operadores y expresiones

## 🎯 Objetivos

Al terminar esta guía podrás:

- Realizar operaciones matemáticas en Python.
- Utilizar operadores aritméticos.
- Comparar valores.
- Entender resultados `True` y `False`.
- Utilizar operadores lógicos.
- Crear expresiones.
- Aplicar operadores a problemas financieros.
- Comprender las bases que posteriormente utilizaremos con `if` y loops.

---

# 1. ¿Qué es un operador?

Un operador es un símbolo que indica a Python qué operación debe realizar.

Por ejemplo:

```python
10 + 5
```

El operador:

```text
+
```

indica una suma.

Resultado:

```text
15
```

---

# 2. Operadores aritméticos

Los principales operadores matemáticos son:

| Operador | Significado | Ejemplo | Resultado |
|---|---|---|---|
| `+` | Suma | `10 + 5` | `15` |
| `-` | Resta | `10 - 5` | `5` |
| `*` | Multiplicación | `10 * 5` | `50` |
| `/` | División | `10 / 5` | `2.0` |
| `//` | División entera | `10 // 3` | `3` |
| `%` | Residuo | `10 % 3` | `1` |
| `**` | Potencia | `2 ** 3` | `8` |

---

# 3. Suma

Utilizamos:

```python
+
```

Ejemplo:

```python
income = 5000
bonus = 1000

total_income = income + bonus

print(total_income)
```

Resultado:

```text
6000
```

---

# 4. Resta

Utilizamos:

```python
-
```

Ejemplo:

```python
income = 5000
expenses = 3200

remaining = income - expenses

print(remaining)
```

Resultado:

```text
1800
```

---

# 5. Multiplicación

Utilizamos:

```python
*
```

Ejemplo:

```python
price = 50
quantity = 4

total = price * quantity

print(total)
```

Resultado:

```text
200
```

---

# 6. División

Utilizamos:

```python
/
```

Ejemplo:

```python
total_sales = 10000
months = 4

average_sales = total_sales / months

print(average_sales)
```

Resultado:

```text
2500.0
```

---

# 7. División entera `//`

La división normal:

```python
10 / 3
```

produce aproximadamente:

```text
3.3333333333333335
```

La división entera:

```python
10 // 3
```

produce:

```text
3
```

La división entera descarta la parte decimal del resultado.

---

# 8. Módulo `%`

El operador `%` devuelve el residuo de una división.

Ejemplo:

```python
10 % 3
```

Resultado:

```text
1
```

Porque:

```text
10 ÷ 3 = 3
```

y sobra:

```text
1
```

---

# 9. ¿Para qué puede servir `%`?

Supongamos que tenemos $103 y queremos saber cuánto dinero sobra después de formar grupos de $10:

```python
money = 103

remaining = money % 10

print(remaining)
```

Resultado:

```text
3
```

---

# 10. Potencia `**`

Podemos calcular potencias utilizando:

```python
**
```

Ejemplo:

```python
result = 2 ** 3

print(result)
```

Resultado:

```text
8
```

Porque:

```text
2 × 2 × 2 = 8
```

---

# 11. Ejemplo financiero: crecimiento

Supongamos una inversión:

```python
investment = 10000
growth_rate = 0.05
```

Calculamos el crecimiento:

```python
growth = investment * growth_rate

print(growth)
```

Resultado:

```text
500.0
```

---

# 12. Prioridad de operaciones

Python respeta el orden matemático de las operaciones.

Por ejemplo:

```python
result = 10 + 5 * 2

print(result)
```

Resultado:

```text
20
```

Primero:

```text
5 × 2 = 10
```

Después:

```text
10 + 10 = 20
```

Podemos utilizar paréntesis para cambiar el orden:

```python
result = (10 + 5) * 2

print(result)
```

Resultado:

```text
30
```

Primero:

```text
10 + 5 = 15
```

Después:

```text
15 × 2 = 30
```

---

# 13. Ejemplo financiero con paréntesis

Supongamos:

```python
income = 5000
bonus = 1000
expenses = 2000
```

Queremos calcular:

```text
(ingreso + bono) - gastos
```

Podemos escribir:

```python
remaining = (income + bonus) - expenses

print(remaining)
```

Resultado:

```text
4000
```

---

# 14. Operadores de comparación

También podemos comparar valores.

Los principales son:

| Operador | Significado |
|---|---|
| `>` | Mayor que |
| `<` | Menor que |
| `>=` | Mayor o igual |
| `<=` | Menor o igual |
| `==` | Igual |
| `!=` | Diferente |

Las comparaciones producen un booleano:

```python
True
```

o:

```python
False
```

---

# 15. Mayor que `>`

```python
balance = 5000

print(balance > 3000)
```

Resultado:

```text
True
```

Porque:

```text
5000 > 3000
```

es verdadero.

---

# 16. Menor que `<`

```python
balance = 5000

print(balance < 3000)
```

Resultado:

```text
False
```

---

# 17. Mayor o igual `>=`

```python
age = 18

print(age >= 18)
```

Resultado:

```text
True
```

---

# 18. Menor o igual `<=`

```python
age = 18

print(age <= 18)
```

Resultado:

```text
True
```

---

# 19. Igual `==`

Hay una diferencia muy importante entre:

```python
=
```

y:

```python
==
```

`=` asigna un valor:

```python
age = 20
```

`==` compara:

```python
age == 20
```

Ejemplo:

```python
age = 20

print(age == 20)
```

Resultado:

```text
True
```

---

# 20. Diferente `!=`

```python
age = 20

print(age != 18)
```

Resultado:

```text
True
```

Porque `20` es diferente de `18`.

---

# 21. Comparaciones financieras

Supongamos:

```python
income = 5000
expenses = 4500
```

Podemos preguntar:

```python
print(income > expenses)
```

Resultado:

```text
True
```

Esto significa:

> Los ingresos son mayores que los gastos.

También:

```python
print(expenses > income)
```

Resultado:

```text
False
```

---

# 22. Operadores lógicos

Los principales operadores lógicos son:

```python
and
or
not
```

Permiten combinar condiciones.

---

# 23. `and`

`and` significa:

> Las dos condiciones deben cumplirse.

Ejemplo:

```python
income = 5000
age = 25

result = income > 3000 and age >= 18

print(result)
```

Tenemos:

```text
income > 3000
```

que es `True`.

Y:

```text
age >= 18
```

que también es `True`.

Por lo tanto:

```text
True
```

---

# 24. Ejemplo financiero con `and`

Supongamos que queremos determinar si una persona cumple dos requisitos para una solicitud:

```text
Ingreso mayor a $3,000
Edad mayor o igual a 18
```

Podemos escribir:

```python
income = 5000
age = 25

eligible = income > 3000 and age >= 18

print(eligible)
```

Resultado:

```text
True
```

---

# 25. `or`

`or` significa:

> Al menos una de las condiciones debe cumplirse.

Ejemplo:

```python
has_credit_card = True
has_cash = False

can_pay = has_credit_card or has_cash

print(can_pay)
```

Resultado:

```text
True
```

La persona puede pagar porque tiene tarjeta.

---

# 26. Ejemplo económico con `or`

Supongamos que un cliente puede recibir una promoción si:

- Es estudiante.

**O**

- Es mayor de 65 años.

```python
is_student = True
age = 30

eligible = is_student or age >= 65

print(eligible)
```

Resultado:

```text
True
```

---

# 27. `not`

`not` invierte un valor booleano.

Por ejemplo:

```python
is_student = True

print(not is_student)
```

Resultado:

```text
False
```

Otro ejemplo:

```python
has_debt = False

print(not has_debt)
```

Resultado:

```text
True
```

---

# 28. Combinar operadores

Podemos combinar diferentes operadores.

Ejemplo:

```python
income = 5000
expenses = 3000
age = 25

result = income > expenses and age >= 18

print(result)
```

Resultado:

```text
True
```

Esto nos permite comenzar a expresar reglas de negocio.

---

# 29. ¿Qué es una expresión?

Una expresión es una combinación de valores, variables y operadores que Python puede evaluar.

Por ejemplo:

```python
10 + 5
```

es una expresión.

También:

```python
income - expenses
```

es una expresión.

Y:

```python
income > expenses
```

también es una expresión.

---

# 30. Ejemplo completo

Supongamos:

```python
income = 6000
expenses = 4000
savings = income - expenses

print("Income:", income)
print("Expenses:", expenses)
print("Savings:", savings)
print("Income greater than expenses:", income > expenses)
```

Resultado:

```text
Income: 6000
Expenses: 4000
Savings: 2000
Income greater than expenses: True
```

---

# 🧪 Ejercicio 1 — Operaciones básicas

Crea:

```python
price = 25
quantity = 8
```

Calcula:

```text
Total
```

Después calcula:

```text
Total + 10% de impuesto
```

---

# 🧪 Ejercicio 2 — Finanzas personales

Tienes:

```python
income = 5000
rent = 1500
food = 600
transport = 300
entertainment = 250
```

Calcula:

1. Total de gastos.
2. Dinero restante.
3. Si el dinero restante es mayor que $2,000.

---

# 🧪 Ejercicio 3 — Comparaciones

Crea:

```python
balance = 7500
```

Realiza las siguientes preguntas mediante Python:

```text
¿El balance es mayor a 5000?
¿El balance es menor a 10000?
¿El balance es igual a 7500?
¿El balance es diferente de 1000?
```

Utiliza los operadores correspondientes.

---

# 🧪 Ejercicio 4 — Operadores lógicos

Tenemos:

```python
income = 6000
age = 30
```

Determina si la persona cumple:

```text
Ingreso mayor a 5,000
Y
Edad mayor o igual a 18
```

---

# 🧪 Ejercicio 5 — `or`

Tenemos:

```python
is_student = False
age = 70
```

Determina si la persona puede recibir una promoción cuando:

```text
Es estudiante
O
Tiene 65 años o más
```

---

# 🧩 Reto final — Evaluación financiera

Tenemos:

```python
income = 7500
expenses = 5000
age = 28
has_debt = False
```

Calcula:

1. Dinero disponible.
2. Si los ingresos son mayores que los gastos.
3. Si la persona es mayor de edad.
4. Si puede ser considerada financieramente elegible bajo esta regla:

```text
Ingresos mayores que gastos
Y
Edad mayor o igual a 18
Y
No tener deuda
```

No utilices `if` todavía.

Debes resolverlo utilizando operadores y variables.

---

# 🎯 Lo que debes dominar

Debes comprender:

- `+`
- `-`
- `*`
- `/`
- `//`
- `%`
- `**`
- `>`
- `<`
- `>=`
- `<=`
- `==`
- `!=`
- `and`
- `or`
- `not`

También debes entender la diferencia entre:

```python
=
```

y:

```python
==
```

---

# Guía 04 — Estructuras de datos

## 🎯 Objetivos

Al terminar esta guía podrás:

- Entender qué es una estructura de datos.
- Comprender por qué necesitamos estructuras de datos.
- Utilizar listas.
- Utilizar tuplas.
- Utilizar diccionarios.
- Comprender conjuntos (`set`).
- Acceder a elementos.
- Modificar datos.
- Agregar y eliminar información.
- Aplicar estructuras de datos a Finanzas, Economía y Business Intelligence.

---

# 1. ¿Qué es una estructura de datos?

Hasta ahora hemos trabajado con variables individuales.

Por ejemplo:

```python
sales = 5000
```

Esto funciona perfectamente si solo necesitamos guardar un dato.

Pero imagina que una empresa tiene 1,000 ventas.

Sería muy incómodo hacer:

```python
sale1 = 100
sale2 = 250
sale3 = 400
sale4 = 300
sale5 = 500
...
```

Necesitamos una forma de almacenar muchos datos juntos.

Para eso existen las **estructuras de datos**.

---

# 2. Una comparación cotidiana

Imagina una lista de compras.

En lugar de tener:

```text
producto1 = Apples
producto2 = Milk
producto3 = Bread
producto4 = Coffee
```

podemos tener:

```text
[
    Apples,
    Milk,
    Bread,
    Coffee
]
```

En Python esto se representa mediante una lista:

```python
shopping_list = ["Apples", "Milk", "Bread", "Coffee"]
```

---

# 3. Las principales estructuras

En Python existen varias estructuras de datos.

En esta guía aprenderemos:

| Estructura | Ejemplo | Uso principal |
|---|---|---|
| `list` | `[10, 20, 30]` | Colecciones ordenadas y modificables |
| `tuple` | `(10, 20, 30)` | Colecciones ordenadas que no queremos modificar |
| `dict` | `{"name": "Alex"}` | Datos organizados mediante claves |
| `set` | `{10, 20, 30}` | Valores únicos |

Estas estructuras son fundamentales para trabajar con datos.

---

# 4. Listas

Una lista permite almacenar varios valores.

Ejemplo:

```python
prices = [100, 200, 300, 400]
```

Podemos imaginar:

```text
prices
   ↓

┌─────┬─────┬─────┬─────┐
│ 100 │ 200 │ 300 │ 400 │
└─────┴─────┴─────┴─────┘
```

---

# 5. Crear una lista

Ejemplo:

```python
expenses = [500, 200, 300, 150]
```

Podemos imprimirla:

```python
print(expenses)
```

Resultado:

```text
[500, 200, 300, 150]
```

---

# 6. Las listas pueden contener diferentes tipos

Una lista puede contener diferentes tipos de datos:

```python
person = ["Alex", 25, 5000, True]
```

Tenemos:

```text
"Alex" → str
25     → int
5000   → int
True   → bool
```

Sin embargo, en análisis de datos normalmente intentaremos mantener estructuras coherentes.

---

# 7. Índices

Cada elemento de una lista tiene una posición.

Python comienza a contar desde:

```text
0
```

No desde `1`.

Por ejemplo:

```python
prices = [100, 200, 300, 400]
```

Las posiciones son:

```text
Índice:    0    1    2    3
           ↓    ↓    ↓    ↓
Valor:    100  200  300  400
```

---

# 8. Acceder a un elemento

Podemos acceder al primer elemento:

```python
prices = [100, 200, 300, 400]

print(prices[0])
```

Resultado:

```text
100
```

Segundo elemento:

```python
print(prices[1])
```

Resultado:

```text
200
```

Tercer elemento:

```python
print(prices[2])
```

Resultado:

```text
300
```

---

# 9. ¿Por qué empieza en 0?

Esto puede parecer extraño al principio.

Python utiliza índices basados en cero.

Por lo tanto:

```text
Primer elemento → índice 0
Segundo elemento → índice 1
Tercer elemento → índice 2
Cuarto elemento → índice 3
```

Debes acostumbrarte a esto porque aparecerá constantemente en programación.

---

# 10. Cambiar un elemento

Las listas son modificables.

Tenemos:

```python
prices = [100, 200, 300]
```

Podemos cambiar el segundo elemento:

```python
prices[1] = 250
```

Ahora:

```python
print(prices)
```

Resultado:

```text
[100, 250, 300]
```

---

# 11. Agregar elementos con `append()`

Podemos agregar un elemento al final de una lista.

```python
expenses = [500, 200, 300]

expenses.append(150)

print(expenses)
```

Resultado:

```text
[500, 200, 300, 150]
```

---

# 12. Eliminar elementos con `remove()`

Podemos eliminar un valor:

```python
expenses = [500, 200, 300]

expenses.remove(200)

print(expenses)
```

Resultado:

```text
[500, 300]
```

---

# 13. Saber cuántos elementos existen

Podemos utilizar:

```python
len()
```

Ejemplo:

```python
prices = [100, 200, 300, 400]

print(len(prices))
```

Resultado:

```text
4
```

Tenemos cuatro elementos.

---

# 14. Ejemplo financiero

Supongamos que tenemos las ventas de una semana:

```python
sales = [1200, 1500, 900, 1800, 2000]
```

Podemos acceder a una venta específica:

```python
print(sales[0])
```

Resultado:

```text
1200
```

Podemos saber cuántos registros tenemos:

```python
print(len(sales))
```

Resultado:

```text
5
```

---

# 15. Sumar elementos de una lista

Python tiene una función llamada:

```python
sum()
```

Ejemplo:

```python
sales = [1200, 1500, 900, 1800, 2000]

total_sales = sum(sales)

print(total_sales)
```

Resultado:

```text
7400
```

---

# 16. Promedio de una lista

Podemos calcular un promedio utilizando:

```python
sum()
```

y:

```python
len()
```

Por ejemplo:

```python
sales = [1200, 1500, 900, 1800, 2000]

average = sum(sales) / len(sales)

print(average)
```

Resultado:

```text
1480.0
```

Esto es muy importante en análisis de datos.

---

# 17. Máximo y mínimo

Podemos obtener el valor máximo:

```python
sales = [1200, 1500, 900, 1800, 2000]

print(max(sales))
```

Resultado:

```text
2000
```

Y el mínimo:

```python
print(min(sales))
```

Resultado:

```text
900
```

---

# 18. Tuplas

Una tupla es parecida a una lista:

```python
(100, 200, 300)
```

Ejemplo:

```python
coordinates = (25.7, -80.1)
```

La diferencia importante es que una tupla **no puede modificarse después de ser creada**.

Por ejemplo:

```python
coordinates = (25.7, -80.1)
```

Podemos acceder:

```python
print(coordinates[0])
```

Resultado:

```text
25.7
```

Pero no podemos hacer:

```python
coordinates[0] = 30
```

Esto genera un error.

---

# 19. ¿Cuándo utilizar una tupla?

Una tupla puede utilizarse cuando tenemos datos que conceptualmente pertenecen juntos y no queremos modificarlos.

Por ejemplo:

```python
rgb = (255, 255, 255)
```

O:

```python
months = ("January", "February", "March")
```

También puede utilizarse para representar coordenadas:

```python
location = (25.7617, -80.1918)
```

---

# 20. Diccionarios

Los diccionarios son extremadamente importantes.

Un diccionario permite almacenar información utilizando:

```text
clave → valor
```

Por ejemplo:

```python
customer = {
    "name": "Alex",
    "age": 25,
    "income": 5000
}
```

Podemos imaginar:

```text
name   → Alex
age    → 25
income → 5000
```

---

# 21. Crear un diccionario

Ejemplo:

```python
student = {
    "name": "Alex",
    "age": 21,
    "major": "Finance"
}
```

Podemos imprimirlo:

```python
print(student)
```

Resultado:

```text
{'name': 'Alex', 'age': 21, 'major': 'Finance'}
```

---

# 22. Acceder a un valor del diccionario

Utilizamos la clave:

```python
student = {
    "name": "Alex",
    "age": 21,
    "major": "Finance"
}

print(student["name"])
```

Resultado:

```text
Alex
```

También:

```python
print(student["age"])
```

Resultado:

```text
21
```

---

# 23. Modificar un valor

Los diccionarios pueden modificarse.

Tenemos:

```python
student = {
    "name": "Alex",
    "age": 21
}
```

Podemos modificar la edad:

```python
student["age"] = 22
```

Ahora:

```python
print(student)
```

Resultado:

```text
{'name': 'Alex', 'age': 22}
```

---

# 24. Agregar información

Podemos agregar una nueva clave:

```python
student["university"] = "University of Miami"
```

Ahora:

```python
print(student)
```

Resultado:

```text
{
    'name': 'Alex',
    'age': 22,
    'university': 'University of Miami'
}
```

---

# 25. Eliminar información

Podemos eliminar una clave:

```python
del student["age"]
```

Ahora la clave `age` ya no existe.

---

# 26. ¿Por qué los diccionarios son importantes?

Los diccionarios son muy utilizados para representar entidades.

Por ejemplo, un cliente:

```python
customer = {
    "name": "John",
    "age": 35,
    "income": 72000,
    "has_debt": True
}
```

Una empresa:

```python
company = {
    "name": "ABC Corp",
    "employees": 120,
    "revenue": 5000000
}
```

Un producto:

```python
product = {
    "name": "Laptop",
    "price": 1200,
    "stock": 25
}
```

---

# 27. Listas de diccionarios

Aquí comienza una combinación muy importante para Business Intelligence.

Podemos tener varios clientes:

```python
customers = [
    {
        "name": "John",
        "age": 35,
        "income": 72000
    },
    {
        "name": "Sarah",
        "age": 28,
        "income": 55000
    },
    {
        "name": "Michael",
        "age": 42,
        "income": 90000
    }
]
```

Tenemos:

```text
Lista
  ↓
Cliente
  ↓
Diccionario
```

Esto se parece mucho a una tabla:

| name | age | income |
|---|---:|---:|
| John | 35 | 72000 |
| Sarah | 28 | 55000 |
| Michael | 42 | 90000 |

Este concepto será fundamental cuando posteriormente trabajemos con datos reales.

---

# 28. Acceder a una lista de diccionarios

Podemos obtener el primer cliente:

```python
print(customers[0])
```

Resultado:

```text
{'name': 'John', 'age': 35, 'income': 72000}
```

Podemos obtener solamente su nombre:

```python
print(customers[0]["name"])
```

Resultado:

```text
John
```

Podemos obtener sus ingresos:

```python
print(customers[0]["income"])
```

Resultado:

```text
72000
```

---

# 29. Sets

Un `set` es una estructura que almacena valores únicos.

Por ejemplo:

```python
countries = {"USA", "Canada", "Mexico"}
```

No permite duplicados.

Por ejemplo:

```python
countries = {"USA", "USA", "Canada", "Mexico"}

print(countries)
```

El resultado contendrá una sola aparición de `"USA"`.

---

# 30. ¿Cuándo son útiles los sets?

Son útiles cuando queremos identificar valores únicos.

Por ejemplo, imagina que una empresa tiene estas ventas:

```python
countries = [
    "USA",
    "Canada",
    "USA",
    "Mexico",
    "Canada",
    "USA"
]
```

Si queremos conocer los países únicos:

```python
unique_countries = set(countries)

print(unique_countries)
```

Obtendremos los países sin duplicados.

---

# 31. Comparación de estructuras

Podemos pensar:

### Lista

```python
sales = [100, 200, 300]
```

Útil cuando necesitamos:

> Una colección ordenada que puede modificarse.

### Tupla

```python
coordinates = (25.7, -80.1)
```

Útil cuando necesitamos:

> Una colección ordenada que no queremos modificar.

### Diccionario

```python
customer = {
    "name": "Alex",
    "age": 25
}
```

Útil cuando necesitamos:

> Información organizada mediante claves.

### Set

```python
countries = {"USA", "Canada", "Mexico"}
```

Útil cuando necesitamos:

> Valores únicos.

---

# 32. ¿Qué estructura utilizar?

Una pregunta importante al programar es:

> ¿Cómo debo organizar mis datos?

Por ejemplo:

Si tenemos:

```text
Ventas:
100
200
300
400
```

podemos utilizar:

```python
sales = [100, 200, 300, 400]
```

Si tenemos información de una persona:

```python
customer = {
    "name": "Alex",
    "age": 30,
    "income": 5000
}
```

Si tenemos coordenadas:

```python
location = (25.7, -80.1)
```

Si queremos países únicos:

```python
countries = {"USA", "Canada", "Mexico"}
```

---

# 33. Estructuras dentro de estructuras

Las estructuras de datos pueden combinarse.

Por ejemplo:

```python
company = {
    "name": "ABC Corp",
    "employees": [
        {
            "name": "John",
            "salary": 5000
        },
        {
            "name": "Sarah",
            "salary": 6000
        }
    ]
}
```

Tenemos:

```text
Diccionario
    ↓
Lista
    ↓
Diccionarios
```

Esto puede parecer complicado ahora, pero es muy común en programación y análisis de datos.

---

# 34. Ejemplo de Business Intelligence

Imagina que tenemos ventas:

```python
sales = [
    {
        "product": "Laptop",
        "price": 1200,
        "quantity": 2
    },
    {
        "product": "Phone",
        "price": 800,
        "quantity": 3
    },
    {
        "product": "Tablet",
        "price": 500,
        "quantity": 4
    }
]
```

Cada elemento representa una venta.

Tenemos una estructura:

```text
Lista
   ↓
Venta
   ↓
Diccionario
```

Esto es una estructura muy cercana a la información que encontraremos en aplicaciones y sistemas empresariales.

---

# 35. Cálculo manual de una venta

La primera venta tiene:

```python
{
    "product": "Laptop",
    "price": 1200,
    "quantity": 2
}
```

Podemos obtener:

```python
sales[0]["price"]
```

Resultado:

```text
1200
```

Y:

```python
sales[0]["quantity"]
```

Resultado:

```text
2
```

Podemos calcular:

```python
total = sales[0]["price"] * sales[0]["quantity"]

print(total)
```

Resultado:

```text
2400
```

---

# 🧪 Ejercicio 1 — Lista de precios

Crea:

```python
prices = [100, 250, 75, 300, 125]
```

Calcula:

1. Número de precios.
2. Precio total.
3. Precio promedio.
4. Precio máximo.
5. Precio mínimo.

Puedes utilizar:

```python
len()
sum()
max()
min()
```

---

# 🧪 Ejercicio 2 — Gastos personales

Crea una lista:

```python
expenses = [
    1200,
    500,
    300,
    250,
    150
]
```

Calcula:

1. Total de gastos.
2. Promedio de gastos.
3. Gasto más alto.
4. Gasto más bajo.

---

# 🧪 Ejercicio 3 — Modificar una lista

Tenemos:

```python
prices = [100, 200, 300]
```

Realiza las siguientes operaciones:

1. Cambia `200` por `250`.
2. Agrega `400`.
3. Elimina `100`.
4. Imprime la lista final.

Resultado esperado:

```text
[250, 300, 400]
```

---

# 🧪 Ejercicio 4 — Diccionario de estudiante

Crea un diccionario:

```python
student = {
    "name": "Tu nombre",
    "age": 0,
    "major": "Finance"
}
```

Después:

1. Cambia la edad por tu edad real.
2. Agrega una clave llamada `university`.
3. Imprime el nombre.
4. Imprime la universidad.
5. Imprime todo el diccionario.

---

# 🧪 Ejercicio 5 — Cliente financiero

Crea:

```python
customer = {
    "name": "John",
    "age": 35,
    "income": 72000,
    "debt": 15000
}
```

Calcula:

```text
Ingreso anual
Deuda
Ingreso después de deuda
```

Puedes utilizar:

```python
customer["income"]
customer["debt"]
```

---

# 🧪 Ejercicio 6 — Lista de clientes

Crea:

```python
customers = [
    {
        "name": "John",
        "income": 72000
    },
    {
        "name": "Sarah",
        "income": 55000
    },
    {
        "name": "Michael",
        "income": 90000
    }
]
```

Obtén:

1. Nombre del primer cliente.
2. Ingreso del segundo cliente.
3. Nombre del tercer cliente.

Utiliza los índices de la lista.

---

# 🧪 Ejercicio 7 — Países únicos

Tenemos:

```python
countries = [
    "USA",
    "Canada",
    "USA",
    "Mexico",
    "Canada",
    "USA",
    "Brazil"
]
```

Utiliza un `set` para obtener únicamente los países diferentes.

---

# 🧩 Reto final — Mini dataset de ventas

Tenemos:

```python
sales = [
    {
        "product": "Laptop",
        "price": 1200,
        "quantity": 2
    },
    {
        "product": "Phone",
        "price": 800,
        "quantity": 3
    },
    {
        "product": "Tablet",
        "price": 500,
        "quantity": 4
    }
]
```

Tu objetivo es analizar manualmente los datos.

### Parte 1

Obtén el primer producto:

```text
Laptop
```

### Parte 2

Obtén el precio del teléfono.

### Parte 3

Obtén la cantidad de tablets vendidas.

### Parte 4

Calcula el valor de la primera venta:

```text
price × quantity
```

### Parte 5

Calcula el valor de la segunda venta.

### Parte 6

Calcula el valor de la tercera venta.

### Parte 7

Calcula el total de ventas.

El resultado debería ser:

```text
Laptop: 2400
Phone: 2400
Tablet: 2000

Total sales: 6800
```

---

# 🧠 Reto adicional — Pensamiento de analista

Imagina que tienes una empresa con cientos de ventas.

Cada venta tiene:

```text
Producto
Precio
Cantidad
Fecha
Cliente
```

Pregunta:

> ¿Qué estructura de datos utilizarías para representar todas las ventas?

Una buena solución inicial sería:

```python
sales = [
    {
        "product": "Laptop",
        "price": 1200,
        "quantity": 2,
        "date": "2026-09-01",
        "customer": "John"
    },
    {
        "product": "Phone",
        "price": 800,
        "quantity": 3,
        "date": "2026-09-02",
        "customer": "Sarah"
    }
]
```

Tenemos:

```text
Lista
   ↓
Diccionario
   ↓
Información de una venta
```

Este patrón será muy importante posteriormente cuando trabajemos con:

- Datos.
- APIs.
- JSON.
- Bases de datos.
- Pandas.
- Business Intelligence.
- Automatización.

---

# 🎯 Lo que debes dominar

Antes de avanzar debes comprender:

## Listas

```python
items = [10, 20, 30]
```

Debes saber:

```python
items[0]
items.append(40)
items.remove(20)
len(items)
```

---

## Tuplas

```python
items = (10, 20, 30)
```

Debes entender que una tupla no puede modificarse después de crearla.

---

## Diccionarios

```python
customer = {
    "name": "Alex",
    "age": 25
}
```

Debes saber acceder:

```python
customer["name"]
```

Modificar:

```python
customer["age"] = 26
```

Y agregar:

```python
customer["income"] = 5000
```

---

## Sets

```python
countries = {"USA", "Canada", "Mexico"}
```

Debes entender que un `set` almacena valores únicos.

---

# 🧠 La idea más importante de esta guía

Una variable individual:

```python
income = 5000
```

sirve para almacenar un dato.

Una estructura de datos:

```python
incomes = [5000, 6000, 7000, 4500]
```

permite almacenar muchos datos.

Un diccionario:

```python
customer = {
    "name": "Alex",
    "income": 5000
}
```

permite representar una entidad con diferentes atributos.

Una lista de diccionarios:

```python
customers = [
    {
        "name": "Alex",
        "income": 5000
    },
    {
        "name": "Sarah",
        "income": 6000
    }
]
```

permite representar muchas entidades.

Esta idea es fundamental para comenzar a pensar como programador y posteriormente como analista de datos.

---

# 📚 Resumen de las cuatro guías

Hasta ahora has aprendido cuatro conceptos fundamentales.

## 1. Variables

Permiten almacenar valores:

```python
income = 5000
```

---

## 2. Tipos de datos

Indican qué clase de información tenemos:

```python
name = "Alex"       # str
age = 25            # int
price = 19.99       # float
is_student = True   # bool
```

---

## 3. Operadores

Permiten trabajar con los datos:

```python
income - expenses
```

o:

```python
income > expenses
```

---

## 4. Estructuras de datos

Permiten organizar múltiples datos:

```python
sales = [100, 200, 300]
```

o:

```python
customer = {
    "name": "Alex",
    "income": 5000
}
```

---

# 🧠 Cómo pensar en Python

Una buena forma de comenzar a analizar un problema es preguntarte:

### 1. ¿Qué información tengo?

Ejemplo:

```text
Ingreso
Gastos
Edad
Nombre
```

### 2. ¿Qué tipo de dato representa cada información?

```text
Nombre → str
Edad → int
Ingreso → float
Gastos → float
```

### 3. ¿Necesito guardar un dato o muchos?

Un dato:

```python
income = 5000
```

Muchos datos:

```python
incomes = [5000, 6000, 7000]
```

### 4. ¿Cómo debo organizar la información?

Una persona:

```python
customer = {
    "name": "Alex",
    "age": 25,
    "income": 5000
}
```

Muchas personas:

```python
customers = [
    {
        "name": "Alex",
        "age": 25,
        "income": 5000
    },
    {
        "name": "Sarah",
        "age": 30,
        "income": 6500
    }
]
```

### 5. ¿Qué operación necesito realizar?

Por ejemplo:

```python
total = income - expenses
```

o:

```python
average = sum(incomes) / len(incomes)
```

---

# 🚀 Próximos temas

Una vez que estos cuatro conceptos estén claros, el siguiente paso natural será aprender:

```text
Variables
    ↓
Tipos de datos
    ↓
Operadores
    ↓
Estructuras de datos
    ↓
Condicionales
    ↓
Loops
    ↓
Funciones
    ↓
Funciones con parámetros
    ↓
Return
    ↓
Módulos
    ↓
Lambda
    ↓
Manejo de errores
    ↓
Archivos
    ↓
Pandas
    ↓
Análisis de datos
    ↓
Visualización
    ↓
Business Intelligence
```

La recomendación es **no avanzar demasiado rápido**.

Antes de aprender loops y funciones, debes sentirte cómodo con:

- Variables.
- Tipos de datos.
- Operadores.
- Listas.
- Diccionarios.
- Índices.
- `len()`.
- `sum()`.
- `min()`.
- `max()`.
- `type()`.
- Conversión de tipos.

Estos conceptos serán utilizados constantemente en los siguientes temas.

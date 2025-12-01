Moviendo Hacia delantes 


paso = int(input("Ingrese cantidad de pasos de la tortuga: "))



print("La tortuga avanzará " + str(paso) + " pasos")



print("-" * paso + ">")



1️⃣ paso = int(input("Ingrese cantidad de pasos de la tortuga: "))

📌 Esta línea hace tres cosas:

input("Ingrese cantidad de pasos de la tortuga: ")

Muestra el texto al usuario.

Espera que el usuario escriba un número en el teclado.

Convierte lo que el usuario escribió a número entero con int()

Si el usuario escribe 30, queda como 30 (entero), no como texto.

Guarda ese número en la variable paso

Ahora paso = 30 (por ejemplo).

2️⃣ print("La tortuga avanzará " + str(paso) + " pasos")

📌 Esta línea muestra un mensaje en pantalla:

"La tortuga avanzará " es un texto.

str(paso) convierte el número a texto para poder unirlo.

" pasos" es otro texto.

🔍 Ejemplo:
Si paso = 30
Imprime:

La tortuga avanzará 30 pasos

3️⃣ print("-" * paso + ">")

📌 Esta línea crea una representación visual del avance de la tortuga:

"-" * paso
Multiplica el símbolo - tantas veces como el número ingresado.

Si paso = 5
produce: "-----"

+ ">"
Agrega una flecha al final, simulando la tortuga.

print(...)
Lo muestra en pantalla.

🔍 Ejemplo:
Si paso = 10
Imprime:

----------> 
<h1>Movimiento hacia abajo</h1>

⭐ Resultado completo si el usuario escribe 30
Ingrese cantidad de pasos de la tortuga: 30
La tortuga avanzará 30 pasos
-------------------------------> 
🐢⬇️ Movimiento hacia abajo

El código:

print("|\n"*paso + "v")


genera muchas líneas hacia abajo, una debajo de otra:

|
|
|
|
v


Cada | representa el rastro que deja la tortuga al moverse.

Cada \n hace un salto de línea, así que los | “bajan”.

La v al final es la tortuga mirando hacia abajo.

Por eso el dibujo final muestra a la tortuga desplazándose verticalmente hacia abajo.

🐢 ¿Quieres verlo más claro?

Si paso = 3:

|
|
v


Si paso = 6:

|
|
|
|
|
v


Entre más pasos pidas, más baja avanzara.
<h1>Union de los dos movientos</h1>
paso = int(input("Ingrese cantidad de pasos de la tortuga "))
print("La tortuga avanzará  " + str(paso) + "pasos")
giro = int(input("Ingrese cantidad de pasos hacia abajo  "))
print("La tortuga avanzará  " + str(giro) + "pasos")
print("|\n"* paso + "-"* giro + ">")
1️⃣ Línea 1
python
Copiar código
paso = int(input("Ingrese cantidad de pasos de la tortuga "))
input() muestra un mensaje al usuario y espera que escriba algo.

int() convierte lo que escriba el usuario a un número entero.

El valor ingresado se guarda en la variable paso.

Ejemplo: si escribes 3, entonces paso = 3.

2️⃣ Línea 2
python
Copiar código
print("La tortuga avanzará  " + str(paso) + "pasos")
str(paso) convierte el número de pasos a texto para poder concatenarlo con otros textos.

print() muestra en pantalla un mensaje.

Salida si paso = 3:

nginx
Copiar código
La tortuga avanzará  3pasos
3️⃣ Línea 3
python
Copiar código
giro = int(input("Ingrese cantidad de pasos hacia abajo  "))
Igual que la línea 1, pero ahora pedimos un número de pasos “hacia abajo” (vertical).

Se guarda en la variable giro.

4️⃣ Línea 4
python
Copiar código
print("La tortuga avanzará  " + str(giro) + "pasos")
Igual que la línea 2, muestra en pantalla la cantidad de pasos hacia abajo que ingresaste.

Ejemplo si giro = 4:

nginx
Copiar código
La tortuga avanzará  4pasos
5️⃣ Línea 5
python
Copiar código
print("|\n"* paso + "-"* giro + ">")
Esta línea hace el dibujo del movimiento de la tortuga solo con caracteres:

"|\n"* paso

"|\n" significa: imprimir una barra vertical | y luego un salto de línea.

* paso repite eso la cantidad de veces que ingresaste en paso.

Ejemplo: si paso = 3

Copiar código
|
|
|
"-"* giro

"-" se repite giro veces, formando una línea horizontal.

Ejemplo: si giro = 4

diff
Copiar código
----
+ ">"

Añade el símbolo > al final de la línea horizontal, simulando la cabeza de la tortuga.

Combinando todo con paso = 3 y giro = 4:

diff
Copiar código
|
|
|
---->
Esto simula que la tortuga avanza 3 pasos verticales y luego gira hacia la derecha 4 pasos.

💡 Resumen:

input() pide datos al usuario.

int() convierte esos datos en números.

print() muestra texto en pantalla.

"*" replica caracteres múltiples veces para dibujar el recorrido.

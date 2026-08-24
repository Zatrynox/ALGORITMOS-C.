# COMPLEJIDAD ALGORÍTMICA — PRIMERA CLASE

---

##  Complejidad Algorítmica

La complejidad algoritmica, ayuda a comparar cual efectividad de algoritmo es mejor, entre uno u otro.

### EFICIENCIA + EFICACIA = EFECTIVIDAD

---

## Tipos de Complejidad

Hay dos tipos de complejidad:

* **Complejidad TEMPORAL**
* **Complejidad ESPACIAL**

###  TEMPORAL

Encuentra solucion en el menor tiempo posible

###  ESPACIAL

Busca distintas soluciones

> **(DEPENDEN DEL TAMAÑO DEL PROBLEMA)**

---

#  Complejidad Temporal: `T(n)`

### 1° Cronometrar el tiempo

**(SUBJETIVO, YA QUE DEPENDE DE LA POTENCIA DEL DISPOSITIVO QUE LO TESTEA)**

---

### 2° Contar pasos con una medida abstracta

**(POSIBLE MEJOR RESULTADO)**

---

#  EJEMPLO 1

## Escribir la suma de 2 numeros

### 🔹 Funcion sumar

```python
def Sumar2Nros(nr1 , nr2):  
    suma = nr1 + nr2  
    return suma
```

### 🔹 Registrar datos

```python
nr1 = int(input("Ingresar numero 1: ")) 
nr2 = int(input("Ingresar numero 2: "))
```

### 🔹 Mostrar resultado

```python
print("La suma es: ", Sumar2Nros(nr1,nr2))
```

---

#  EJEMPLO 2

## Escribir un programa para calcular el mayor de dos numeros

### 🔹 Funcion mayor

```python
def Mayor2Nrs(n1,n2):
  if n1 > n2:
    mayor = n1
  else:
    mayor = n2
  return mayor
```

### 🔹 Ingresar datos

```python
n1 = int(input("Ingresa n1: "))
n2 = int(input("Ingresa n2: "))
```

### 🔹 Calcula el mayor

```python
mayor = Mayor2Nrs(n1,n2)
```

### 🔹 Mostrar resultado

```python
print(f"El mayor de los numeros {n1} y {n2} es {mayor}")
```

---

#  EJEMPLO 3

## Escribir un programa para calcular el promedio de "n" numeros

```python
n = int(input("Ingrese la cantidad de numeros a promediar: ")) 
 
#Calculando la suma de los numeros 
i = 0 
suma = 0 
while i<n: 
  i+=1 
  nota = int(input(f"ingresar la nota {i}: ")) 
  suma = suma + nota 
 
#Calculando el promedio de notas 
 
promedio = suma/n 
 
#Mostrar resultado 
print(f"El promedio de las {n} notas son: {promedio}")
```

---

#  EJEMPLO 4

## Escribir un programa para calcular la distancia entre dos puntos de un plano cartesiano

```python
x1 = int(input("Ingrese la componente x del primer punto: ")) 
y1 = int(input("Ingrese la componente y del primer punto: ")) 

x2 = int(input("Ingrese la componente x del segundo punto: ")) 
y2 = int(input("Ingrese la componente y del segundo punto: ")) 

distancia = ((x2 - x1)**2 + (y2 - y1)**2)**0.5

print("La distancia entre los puntos es: ", distancia)
```
## OTRA FORMA MÁS COMPLEJA BY JULIUS

```python
import re

pattern = r"^\s*\d+\s*,\s*\d+\s*$"

def parser_point(point_str: str):
  match = re.match(pattern, point_str)
  if match:
    parts = point_str.split(',')
    x = int(parts[0].strip())
    y = int(parts[1].strip())
    return (x, y)
  else:
    print(f"Error: El formato de punto '{point_str}' no coincide con el patrón esperado (int,int).")
    return None

def input_point():
  while True:
    point_str = input("Ingrese un punto (ej. 1,2): ")
    parsed_point = parser_point(point_str)
    if parsed_point is not None:
      return parsed_point

def distance_points(point1, point2):
  x1, y1 = point1
  x2, y2 = point2
  return ((x1 - x2)**2 + (y1 - y2)**2)**0.5

points = []

for i in range(1, 3):
  print(f"Ingrese el punto {i}")
  points.append(input_point())

print(f"La distancia del punto1 y punto2 es: {distance_points(points[0], points[1])}")
```
 
---

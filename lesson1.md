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

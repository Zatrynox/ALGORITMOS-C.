## COMPLEJIDAD ALGORITMICA PRIMERA CLASE
Complejidad algoritmica, ayuda a comparar cual efectividad de algoritmo es mejor, entre uno u otro.
# EFICIENCIA + EFICACIA = EFECTIVIDAD
---
Hay dos tipos de complejidad, complejidad TEMPORAL y ESPACIAL
TEMPORAL: Encuentra solucion en el menor tiempo posible
ESPACIAL: Busca distintas soluciones
(DEPENDEN DEL TAMAÑO DEL PROBLEMA)

---
# Complejidad Temporal: "T(n)"
1° Cronometrar el tiempo (SUBJETIVO, YA QUE DEPENDE DE LA POTENCIA DEL DISPOSITIVO QUE LO TESTEA)
---
2° Contar pasos con una medida abstracta (POSIBLE MEJOR RESULTADO)
---

---
EJEMPLO

    # Escribir la suma de 2 numeros
# Funcion sumar

> def Sumar2Nros(nr1 , nr2):
suma = nr1 + nr2
return suma

----

# Registrar datos

> nr1 = int(input("Ingresar numero 1: ")) 
> nr2 = int(input("Ingresar numero 2: "))

---

# Mostrar resultado

> print("La suma es: ", Sumar2Nros(nr1,nr2))

---


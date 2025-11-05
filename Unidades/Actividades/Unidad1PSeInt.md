---
layout: default
title: Unidad 1 Actividades en PSeInt
---

# 💻 Códigos en PSeInt realizados

En esta sección se recopilan los programas desarrollados en **PSeInt**, junto con su descripción, propósito, diagrama de flujo y código fuente.  
Cada ejemplo busca reforzar la comprensión de la lógica algorítmica y las estructuras fundamentales de programación.

---

## 🔹 Ejemplo 1 — Cálculo del promedio de notas

**Archivo:** `promedio_notas.psc`  
**Descripción:**  
Este algoritmo permite calcular el promedio de un conjunto de notas ingresadas por el usuario.  
Primero solicita la cantidad de notas a evaluar, luego las almacena en un arreglo y finalmente calcula el promedio general.  
Además, determina si el estudiante se encuentra **aprobado** o **reprobado** según el valor del promedio (umbral = 7).

**Código:**

```pseint
Algoritmo promedio_notas;
	Definir n, i Como Entero;
	Definir notas, suma, promedio Como Real;
	Definir estado Como Caracter;
	
	Escribir ("Ingrese el número de notas:");
	Leer n;
	
	Dimensionar notas[n];
	suma = 0;
	
	Para i = 1 Hasta n Con Paso 1 Hacer
		Escribir ("Ingrese la nota ", i, ":");
		Leer notas[i];
		suma = suma + notas[i];
	Fin Para;
	
	promedio = suma / n;
	
	Si promedio >= 7 Entonces
		estado = "Aprobado";
	SiNo
		estado = "Reprobado";
	Fin Si;
	
	Escribir ("-------------------");
	Escribir ("El promedio es: ", promedio);
	Escribir ("El estado del estudiante es: ", estado);
	Escribir ("-------------------");
FinAlgoritmo
```

**IMAGEN 3:** Diagrama de flujo del cálculo del promedio de notas.  

**Diagrama de Flujo:**  
![Diagrama de Flujo](./Imagenes/promedio_notas.png)  

**Descripción del Diagrama de Flujo:**  
El diagrama inicia solicitando el número de notas, luego itera (bucle) para pedir cada nota y acumular la suma.  
Al finalizar el ciclo se calcula el promedio y se evalúa una condición (>=7). Según el resultado, se asigna el estado y se muestran los resultados finales.

---

## 🔹 Ejemplo 2 — Promedio ponderado de tres calificaciones

**Archivo:** `promedio_ponderado.psc`  
**Descripción:**  
Este algoritmo calcula el **promedio ponderado** de tres calificaciones, aplicando diferentes porcentajes de peso a cada nota:  
- Nota 1 → 30%  
- Nota 2 → 30%  
- Nota 3 → 40%  

El programa solicita al usuario ingresar las tres notas, realiza los cálculos de ponderación y muestra el promedio final con explicación de cada paso.

**Código:**

```
Algoritmo promedio_ponderado;
	// Variables
	Definir n1, n2, n3, resultado Como Real;
	Definir N1, N2, N3 Como Real;
	
	// Datos de entrada
	Escribir ("Ingrese la primera nota:");
	Leer n1;
	Escribir ("Ingrese la segunda nota:");
	Leer n2;
	Escribir ("Ingrese la tercera nota:");
	Leer n3;
	
	// Cálculos de ponderación
	N1 = n1 * 0.3;
	N2 = n2 * 0.3;
	N3 = n3 * 0.4;
	
	resultado = N1 + N2 + N3;
	
	// Resultado
	Escribir ("-------------------");
	Escribir ("Nota 1 (30%): ", N1);
	Escribir ("Nota 2 (30%): ", N2);
	Escribir ("Nota 3 (40%): ", N3);
	Escribir ("Promedio ponderado final: ", resultado);
	Escribir ("-------------------");
FinAlgoritmo
```

**IMAGEN 4:** Diagrama de flujo del promedio ponderado de tres calificaciones. 

**Diagrama de Flujo:**  
![Diagrama de Flujo](./Imagenes/promedio_ponderado.png)  

**Descripción del Diagrama de Flujo:**  
1. Inicio → Pedir 3 notas.  
2. Multiplicar cada nota por su peso (0.3, 0.3, 0.4).  
3. Sumar los resultados para obtener el promedio ponderado.  
4. Mostrar resultado → Fin.

---

## 🔹 Ejemplo 3 — Área y longitud de un círculo

**Archivo:** `area_circulo.psc`  
**Descripción:**  
Este algoritmo calcula el **área** y la **longitud (circunferencia)** de un círculo a partir del radio ingresado por el usuario.  
Se utiliza la constante π (PI) provista por PSeInt (o se define manualmente si el entorno no la incluye).

**Código:**

```pseint
Algoritmo area_circulo;
	// Declaración de variables
	Definir r, area, longit Como Real;
	Constante PI = 3.14159265358979;
	
	// Entrada
	Escribir ("Ingrese el radio del círculo (m):");
	Leer r;
	
	// Validación simple
	Si r <= 0 Entonces
		Escribir ("El radio debe ser un número positivo mayor que cero.");
	Fin Si;
	
	// Cálculos
	area = PI * r ^ 2;
	longit = 2 * PI * r;
	
	// Salida
	Escribir ("-------------------");
	Escribir ("El área del círculo es: ", area, " m^2");
	Escribir ("La longitud (circunferencia) es: ", longit, " m");
	Escribir ("-------------------");
FinAlgoritmo
```

**IMAGEN 5:** Diagrama de flujo del cálculo del área y longitud de un círculo. 

**Diagrama de Flujo:**  
![Diagrama de Flujo](./Imagenes/area_circulo.png)  

**Descripción del Diagrama de Flujo:**  
1. Inicio → Pedir radio.  
2. Calcular área con la fórmula `area = PI * r^2`.  
3. Calcular longitud con `longit = 2 * PI * r`.  
4. Mostrar área y longitud → Fin.

---

<div align="center">

<a href="../Unidad1" style="
    background: linear-gradient(90deg, #2E7D32, #66BB6A);
    color: white;
    padding: 12px 30px;
    text-decoration: none;
    font-size: 18px;
    font-weight: bold;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    display: inline-block;
    margin-top: 20px;
">
⬅️ Volver al Índice
</a>

</div>

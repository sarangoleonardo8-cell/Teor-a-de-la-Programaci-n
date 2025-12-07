layout: default
title: Unidad 2
---

# 🧩 Unidad 2 — Estructuras algorítmicas de control

---
## 📘 **Contenidos de la Unidad**

## **Estructura Algorítmicas Condicionales y Estructuras algorítmicas Repetitivas**:
Las estructuras condicionales son aquellas que permiten que un programa tome decisiones, es decir:

👉 Ejecutan una acción si se cumple una condición,

👉 y otra acción si no se cumple.

Las estructuras algorítmicas repetitivas (también llamadas estructuras de repetición o bucles) son aquellas que permiten ejecutar una o varias instrucciones varias veces, siempre que se cumpla una condición.
### ** Estructura Condicional Simple (Si .. Entonces)**
La estructura condicional simple es una estructura de decisión que permite ejecutar una instrucción solo si se cumple una condición.

👉 Si la condición es verdadera, se ejecuta la acción.

👉 Si la condición es falsa, no pasa nada y el programa sigue.

**Ejemplo**
```
Algoritmo edades
   Definir edad Como Entero
   Escribir "Ingrese su edad:"
   Leer edad

   Si edad >= 18 Entonces
      Escribir "Usted es mayor de edad"
   Fin Si
FinAlgoritmo

```
### ** Estructura Condicional Doble (Si ..Entonces, Sino ..)**
La estructura condicional doble es una estructura de decisión que permite al programa elegir entre dos opciones:

👉 Si la condición es verdadera → ejecuta una acción

👉 Si no (SINO) → ejecuta otra acción diferente

**Ejemplo**
```
Algoritmo AprobadoDesaprobado
   Definir nota Como Entero
   Escribir "Ingrese su nota:"
   Leer nota

   Si nota >= 7 Entonces
      Escribir "Aprobado"
   Sino
      Escribir "Reprobado"
   Fin Si
FinAlgoritmo

```
### ** Estructura Condicional Múltiple (En caso de ….)**
La estructura condicional múltiple permite al programa elegir entre más de dos opciones, según el valor de una variable

**Ejemplo**
```
Algoritmo CondicionalMultiple
   Definir opcion Como Entero

   Escribir "MENU"
   Escribir "1. Sumar"
   Escribir "2. Restar"
   Escribir "3. Multiplicar"
   Leer opcion

   Segun opcion Hacer
      1:
         Escribir "Elegiste Sumar"
      2:
         Escribir "Elegiste Restar"
      3:
         Escribir "Elegiste Multiplicar"
      De Otro Modo:
         Escribir "Opción inválida"
   Fin Segun
FinAlgoritmo

```
---

## 📝 **Tareas Entregadas**

<div align="center">

<table>
  <tr>
    <th>📚 Título</th>
    <th>🖊️ Descripción</th>
    <th>🔗 Enlace</th>
  </tr>
  <tr>
    <td><b>Tarea 1:</b> Control de aprendizaje de programas utilizando estructuras condicionales.</td>
    <td>Aplicar estructuras condicionales en la resolución de problemas mediante la construcción de programas simples y funcionales.</td>
    <td><a href="https://drive.google.com/file/d/1Qb1_JBOakmHkbqn1TetcU75xeT2UHu_g/view?usp=sharing">Ver deber</a></td>
  </tr>
  <tr>
    <td><b>Tarea 2:</b> Aplicación de estructuras condicionales en la resolución de problemas.</td>
    <td>Comprender y aplicar las estructuras condicionales simples, dobles y múltiples en la resolución de problemas.</td>
    <td><a href="https://drive.google.com/file/d/1CVp4YtcFJC52Xb4g3mS8W0jzJTmQZeqN/view?usp=sharing">Ver deber</a></td>
  </tr>
  <tr>
    <td><b>Tarea 3:</b> Aplicación de estructuras repetitivas en la resolución de problemas.</td>
    <td>Comprender y aplicar las estructuras repetitivas en la resolución de problemas.</td>
    <td><a href="https://drive.google.com/file/d/1cSnV3dm1kVTwGS7ijgjP8LEs4oH_uPrP/view?usp=sharing">Ver deber</a></td>
  </tr>
  <tr>
  <td><b>Tarea 4:</b> Diferencias entre los tipos de estructuras condicionales.</td>
    <td>Analizar y representar los diferentes tipos de estructuras condicionales, aplicando diagramas de flujo y codificación en lenguaje de programación.</td>
    <td><a href="https://drive.google.com/file/d/1uG1agXENyUPFQQOrXrT_Wf1nK34mLxh2/view?usp=sharing">Ver deber</a></td>
  </tr>
  <tr>
    <td><b>Tarea 5:</b> Instalacion de Programas</td>
    <td>Revisión de tutoriales oficiales de instalación de lenguajes de programación (C, Python o Java).</td>
    <td><a href="https://drive.google.com/file/d/1zeNKcmTIFCxACPx4wcPHMo48C1_BM9B1/view?usp=drive_link.md">Ver deber</a></td>
  </tr>
</table>

</div>

---

## 💾 Códigos de Programación realizados

<div align="center">

<a href="./Actividades/Unidad1" style="
    background: linear-gradient(90deg, #1E88E5, #42A5F5);
    color: white;
    padding: 10px 25px;
    text-decoration: none;
    font-size: 16px;
    font-weight: bold;
    border-radius: 8px;
    box-shadow: 0 3px 8px rgba(0,0,0,0.2);
    display: inline-block;
    margin: 5px;
">
💻 Códigos en C
</a>

<a href="./Actividades/Unidad1PSeInt" style="
    background: linear-gradient(90deg, #1E88E5, #42A5F5);
    color: white;
    padding: 10px 25px;
    text-decoration: none;
    font-size: 16px;
    font-weight: bold;
    border-radius: 8px;
    box-shadow: 0 3px 8px rgba(0,0,0,0.2);
    display: inline-block;
    margin: 5px;
">
💻 Códigos en PSeInt
</a>

</div>

---

## 💭 **Reflexión Crítica de los Aprendizajes de la Unidad**

<div style="
  border-left: 6px solid #0078D7;
  background-color: #f3f9ff;
  padding: 16px;
  border-radius: 8px;
  line-height: 1.6;
  font-size: 16px;
">

<p>
Durante el desarrollo de la <b>Unidad 1: Fundamentos de Algoritmos y Programas</b>, comprendí la importancia de estructurar el pensamiento lógico antes de escribir cualquier línea de código.
</p>

<p>
Aprendí a representar procesos mediante <b>pseudocódigo</b> y <b>diagramas de flujo</b>, lo cual facilita la comprensión del problema y evita errores en la implementación.
</p>

<p>
Además, el trabajo con <b>estructuras secuenciales</b> permitió fortalecer las bases de la programación, entendiendo que cada instrucción tiene un propósito dentro del flujo del algoritmo.
</p>

<p>
Identifiqué también las <b>principales dificultades</b>, como la traducción de la lógica humana a un lenguaje formal, lo que exige práctica constante y atención a los detalles.
</p>

<p>
En conclusión, esta unidad me ayudó a desarrollar un pensamiento más <b>analítico, ordenado y preciso</b>, cualidades fundamentales para avanzar hacia unidades más complejas de programación.
</p>

</div>

---

<p align="center">
  <a href="../principal" style="
    display:inline-block;
    background-color:#0078D7;
    color:#fff;
    padding:10px 18px;
    border-radius:8px;
    text-decoration:none;
    font-weight:bold;
  ">
    🏠 Ir a la Página Principal
  </a>
</p>

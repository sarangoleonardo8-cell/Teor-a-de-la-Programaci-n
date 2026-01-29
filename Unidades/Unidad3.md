---
Layout: Default
Title: Unidad 3
---
# 🧩 Unidad 3 — Programación modular y estructura de datos estáticas

---
## 📘 **Contenidos de la Unidad**

## **Programación modular**:
- Es una técnica donde un programa grande se divide en partes más pequeñas llamadas módulos o funciones, y cada una cumple una tarea específica.En lugar de tener todo el código junto y revuelto, lo separas por responsabilidades.
## 🔹 8. Ejemplos Prácticos en C

### 📌 Ejemplo 1: Función sin retorno

```c
#include <stdio.h>

void mostrarMensaje() {
    printf("Bienvenido a la Programación Modular\n");
}

int main() {
    mostrarMensaje();
    return 0;
}
```
### 📌 Ejemplo 2: Función con retorno

```c
#include <stdio.h>

int sumar(int a, int b) {
    return a + b;
}

int main() {
    int resultado = sumar(5, 3);
    printf("La suma es: %d\n", resultado);
    return 0;
}
```
### 📌 Ejemplo 3: Paso por valor

```c
#include <stdio.h>

void incrementar(int x) {
    x = x + 1;
}

int main() {
    int numero = 5;
    incrementar(numero);
    printf("Valor final: %d\n", numero);
    return 0;
}
```
### 📌 Ejemplo 4: Paso por referencia

```c
#include <stdio.h>

void incrementar(int *x) {
    *x = *x + 1;
}

int main() {
    int numero = 5;
    incrementar(&numero);
    printf("Valor final: %d\n", numero);
    return 0;
}
```
## **Estructuras de datos estáticas básicas**:
### Unidimensionales
```c
#include <stdio.h>

int main()
{
    int lista[5] = {8, 10, 9, 5, 1};

    printf("Arreglo unidimensional:\n");
    for (int i = 0; i < 5; i++)
    {
        printf("Elemento en la posicion %d: %d\n", i, lista[i]);
    }

    return 0;
}

```
### Bidimensionales 
```c
#include <stdio.h>

int main()
{
    int matriz[3][4] = {
        {9, 5, 8, 6},
        {2, 3, 4, 8},
        {7, 7, 2, 4}
    };

    printf("Elementos de la matriz:\n");
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 4; j++)
        {
            printf("Elemento en la posicion [%d][%d]: %d\n", i, j, matriz[i][j]);
        }
        printf("\n");
    }

    printf("Matriz completa:\n");
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 4; j++)
        {
            printf("%d ", matriz[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```
### Tridimensionales 
```c
#include <stdio.h>

int main()
{
    int arreglotridimensional[2][3][2];

    // Asignar valores capa 1
    arreglotridimensional[0][0][0] = 1;
    arreglotridimensional[0][0][1] = 2;

    arreglotridimensional[0][1][0] = 3;
    arreglotridimensional[0][1][1] = 4;

    arreglotridimensional[0][2][0] = 5;
    arreglotridimensional[0][2][1] = 6;

    // Asignar valores capa 2
    arreglotridimensional[1][0][0] = 7;
    arreglotridimensional[1][0][1] = 8;

    arreglotridimensional[1][1][0] = 9;
    arreglotridimensional[1][1][1] = 10;

    arreglotridimensional[1][2][0] = 11;
    arreglotridimensional[1][2][1] = 12;

    // Mostrar valores
    printf("Arreglo tridimensional:\n");
    for (int i = 0; i < 2; i++)
    {
        printf("Capa %d:\n", i + 1);
        for (int j = 0; j < 3; j++)
        {
            for (int k = 0; k < 2; k++)
            {
                printf("Elemento en la posicion [%d][%d][%d]: %d\n",
                       i, j, k, arreglotridimensional[i][j][k]);
            }
            printf("\n");
        }
        printf("\n");
    }

    return 0;
}
```

### 🚧 **Principales Dificultades en la Aplicación de los Contenidos**
Durante el estudio de la programación modular y las estructuras de datos estáticas, una de las principales dificultades fue comprender cómo dividir correctamente un programa en funciones y cómo comunicarlas mediante parámetros. Además, el manejo de arreglos y cadenas presentó retos al trabajar con índices, tamaños definidos y control de errores como desbordamientos. Superar estas dificultades requirió práctica y atención al orden y la lógica del código

💡 **Recomendación:** Recomiendo practicar constantemente la creación de funciones para fortalecer la programación modular y mejorar la organización del código. Asimismo, es importante prestar atención al manejo de índices y tamaños en los arreglos y cadenas para evitar errores. Finalmente, realizar ejercicios prácticos y revisar el código paso a paso ayuda a reforzar la lógica y comprender mejor el funcionamiento de las estructuras de datos.

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
Durante el desarrollo de la <b> Unidad 3 : Programación modular y estructura de datos estáticas </b> </p>
En esta unidad aprendí la importancia de la programación modular y el uso de estructuras de datos estáticas básicas para desarrollar programas ordenados y eficientes. La programación modular facilita dividir el código en funciones, mientras que los arreglos y cadenas permiten almacenar y manejar información de forma estructurada. Estos conocimientos fortalecen la lógica de programación y son fundamentales para crear soluciones claras y funcionales.
</div>


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
    <td><b>Tarea 1:</b> Control de aprendizaje de programas en Python.</td>
    <td>Evaluar la comprensión de los fundamentos del lenguaje Python mediante preguntas teóricas y prácticas.</td>
    <td><a href="https://drive.google.com/file/d/1DLU1VMxqvibVkzpi0CbA064oiLPGQXzm/view?usp=sharing">Ver deber</a></td>
  </tr>
  <tr>
    <td><b>Tarea 2:</b> Control de aprendizaje sobre modularidad y estructura de datos.</td>
    <td>Aplicar estructuras de datos compuestas y programación modular en lenguaje C para organizar, manipular y procesar información en la resolución de problemas computacionales.</td>
    <td><a href="https://drive.google.com/file/d/1AdpEF5ZMvg92MSBfK5DPTTKDmW-hX00W/view?usp=sharing">Ver deber</a></td>
  </tr>
  <tr>
    <td><b>Tarea 3:</b> Construcción de funciones y procedimientos en un lenguaje de programación.</td>
    <td>Aplicar los fundamentos de la programación modular mediante la construcción y uso de funciones y procedimientos, para resolver un problema real, garantizando un código estructurado, reutilizable y correctamente documentado.</td>
    <td><a href="https://drive.google.com/file/d/14hO6yYLiyOvbAVD9ufY5iOWgjglFUVip/view?usp=sharing">Ver deber</a></td>
  </tr>
  <tr>
  <td><b>Tarea 4:</b> Curso virtual de Cisco Networking Academy.</td>
    <td>Presentar certificado de aprobacion de curso.</td>
    <td><a href="https://drive.google.com/file/d/1kX2dnHde69br2OozRqJb7rEa19qZGeAU/view?usp=sharing">Ver deber</a></td>
  </tr>
  <tr>
    <td><b>Tarea 5:</b> Implementacion de funciones utilizando el paso de parametros por valor y por referencia. </td>
    <td> Este deber no requiere entrega.</td>
  </tr>
</table>

</div>

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

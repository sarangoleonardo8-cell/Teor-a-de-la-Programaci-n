---
Layout: Default
Title: Unidad 2
---
# 🧩 Unidad 2 — Estructuras algorítmicas de control

---
## 📘 **Contenidos de la Unidad**

## **Estructura Algorítmicas Condicionales y Estructuras algorítmicas Repetitivas**:
Las estructuras condicionales son aquellas que permiten que un programa tome decisiones, es decir:

👉 Ejecutan una acción si se cumple una condición,

👉 y otra acción si no se cumple.

Las estructuras algorítmicas repetitivas (también llamadas estructuras de repetición o bucles) son aquellas que permiten ejecutar una o varias instrucciones varias veces, siempre que se cumpla una condición.
###  Estructura Condicional Simple (Si .. Entonces)
La estructura condicional simple es una estructura de decisión que permite ejecutar una instrucción solo si se cumple una condición.

👉 Si la condición es verdadera, se ejecuta la acción.

👉 Si la condición es falsa, no pasa nada y el programa sigue.

**IMAGEN 1:** Diagrama de flujo 

![Diagrama de Flujo](./Imagenes/Captura-de-pantalla-2025-12-07-192505.png)

**Ejemplo** En c++
```
#include <stdio.h>

int main() {
    int edad;

    printf("Escriba su edad: ");
    scanf("%d", &edad);

    if (edad >= 18) {
        printf("Usted es mayor de edad");
    }

    return 0;
}
```


###  Estructura condicional Doble (Si ..Entonces, Sino ..)
La estructura condicional doble es una estructura de decisión que permite al programa elegir entre dos opciones:

👉 Si la condición es verdadera → ejecuta una acción

👉 Si no (SINO) → ejecuta otra acción diferente

**IMAGEN 2:** Diagrama de flujo 

![Diagrama de Flujo](./Imagenes/Captura-de-pantalla-2025-12-07-94150.png)

**Ejemplo** En c++
```
#include <stdio.h>

int main() {
    int nota;

    printf("Ingrese su nota: ");
    scanf("%d", &nota);

    if (nota >= 7) {
        printf("Aprobado");
    } else {
        printf("Reprobado");
    }

    return 0;
}
```
###  Estructura Condicional Múltiple (En caso de ….) 
La estructura condicional múltiple permite al programa elegir entre más de dos opciones, según el valor de una variable

**IMAGEN 3:** Diagrama de flujo 

![Diagrama de Flujo](./Imagenes/Captura-de-pantalla-2025-12-07-194811.png)

**Ejemplo** En c++
```
#include <stdio.h>

int main() {
    int opcion;

    printf("MENU\n");
    printf("1. Sumar\n");
    printf("2. Restar\n");
    printf("3. Multiplicar\n");
    scanf("%d", &opcion);

    switch (opcion) {
        case 1:
            printf("Elegiste Sumar");
            break;
        case 2:
            printf("Elegiste Restar");
            break;
        case 3:
            printf("Elegiste Multiplicar");
            break;
        default:
            printf("Opcion invalida");
            break;
    }

    return 0;
}
```
## Programa combinado realizado en Python 

###  Descripcion del problema

- La empresa eléctrica necesita analizar el consumo energético registrado por varios medidores de luz. Para ello se requiere un programa que
permita ingresar el consumo en kilovatios-hora (kWh) de N medidores eléctricos y que posteriormente realice una clasificación y un análisis 
estadístico de dichos consumos.
- El programa debe permitir al usuario indicar cuántos medidores se van a evaluar e ingresar el consumo individual de cada uno. Con esta 
información, el sistema debe:
- Clasificar cada medidor según su nivel de consumo:
  
Bajo: menos de 100 kWh

Medio: entre 100 y 300 kWh

Alto: más de 300 kWh

Contabilizar cuántos medidores pertenecen a cada categoría.

- Determinar datos estadísticos, tales como:
  
El mayor consumo registrado y el número del medidor al que pertenece.

El menor consumo registrado y el número del medidor correspondiente.

El consumo total de todos los medidores.

El promedio general de consumo.

- Finalmente, el programa debe mostrar un resumen completo con todos los resultados obtenidos.

### Programa en Python
```
# Programa para clasificar el consumo de N medidores eléctricos

# Pedimos cuántos medidores se van a ingresar
n = int(input("¿Cuántos medidores desea ingresar?: "))

consumos = []  # lista para guardar los consumos
bajo = 0
medio = 0
alto = 0

# Ingreso de datos
for i in range(1, n + 1):
    consumo = float(input(f"Ingrese el consumo del medidor {i} en kWh: "))
    consumos.append(consumo)

    # Clasificación según el consumo
    if consumo < 100:
        print(f"El medidor {i} tuvo un consumo BAJO.")
        bajo += 1
    elif consumo <= 300:
        print(f"El medidor {i} tuvo un consumo MEDIO.")
        medio += 1
    else:
        print(f"El medidor {i} tuvo un consumo ALTO.")
        alto += 1

# Calcular mayor, menor y total de consumo
mayor_consumo = max(consumos)
menor_consumo = min(consumos)
consumo_total = sum(consumos)  # suma de todos los consumos
promedio_consumo = consumo_total / n  # promedio de consumo

# Identificar medidores con mayor y menor consumo
medidor_mayor = consumos.index(mayor_consumo) + 1
medidor_menor = consumos.index(menor_consumo) + 1

# Mostrar resultados finales
print("\n--- RESULTADOS ---")
print(f"Existen {alto} medidor(es) en nivel ALTO")
print(f"Existen {medio} medidor(es) en nivel MEDIO")
print(f"Existen {bajo} medidor(es) en nivel BAJO")
print(f"El medidor con MAYOR consumo es el número {medidor_mayor} con {mayor_consumo} kWh")
print(f"El medidor con MENOR consumo es el número {medidor_menor} con {menor_consumo} kWh")
print(f"El consumo TOTAL de todos los medidores es {consumo_total} kWh")
print(f"El consumo PROMEDIO es {promedio_consumo:.2f} kWh")

```
### Diagrama de flujo
![Diagrama de Flujo](./Imagenes/ClasificarMedidoresBasico.svg)
### Programa ejecutado 
![Python](./Imagenes/Captura-de-pantalla-2025-12-08-213106.png)

---

### 🚧 **Principales Dificultades en la Aplicación de los Contenidos**
- A veces se me complica plantear bien las condiciones.
Me confundo con los operadores (==, >, <, &&, ||) y eso hace que el programa no haga exactamente lo que quiero.

- Me cuesta decidir qué estructura usar en cada caso.
A veces no sé si usar un if, un for, un while o un do…while, y eso hace que tarde más en resolver los ejercicios o que escoja una estructura que no es la más adecuada. 

💡 **Recomendación:** Practicar con ejercicios pequeños y variados ayuda bastante a comprender mejor cuándo usar cada estructura. Empezar con ejemplos simples permite entender bien las condiciones y el control de los ciclos, y poco a poco se vuelve más fácil identificar la estructura adecuada para cada problema.

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
Durante el desarrollo de la <b> Unidad 2 : Estructuras Condicionales y Repetitivas </b> </p>
Aprendí que las estructuras condicionales permiten a los programas tomar decisiones según una condición, mientras que las estructuras repetitivas hacen posible ejecutar acciones varias veces de manera automática. Estos temas son esenciales para crear programas más ordenados, dinámicos y eficientes. Gracias a esta unidad, fortalecí mi pensamiento lógico y comprendí mejor cómo resolver problemas de forma estructurada mediante la programación.
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
    <td><b>Tarea 5:</b> Cuadro comparativo entre las estructuras repetitivas </td>
    <td> Analizar y comparar las principales estructuras repetitivas utilizadas en programación, identificando sus características, diferencias y aplicaciones.</td>
    <td><a href="https://drive.google.com/file/d/1Xjj9eUn4_oHjTZy6rJ41SYteusQVtpZO/view?usp=sharing">Ver deber</a></td>
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
  </a>
</p>

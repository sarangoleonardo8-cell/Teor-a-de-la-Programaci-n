---
layout: default
title: Unidad 1 Actividades en PSeInt
---

# 💻 Códigos en PSeInt realizados

En esta sección se recopilan los programas desarrollados en **PSeInt**, junto con su descripción, propósito y código fuente.

---

## 🔹 Ejemplo 1 — Resta

**Archivo:** `MIPRIMERPROGAMA.c`  
**Descripción:** Realize primera programacion.

**Código:**
```c
#include <stdio.h>
#include <string.h>

int main(){
    float  N1,N2,resta;

    printf("ingrese N1\n");
    scanf("%f", &N1 );
    printf("ingrese N2\n");
    scanf("%f", &N2);

    resta=N1-N2;
    
    printf("El resultado es:%.2f",resta);

    return 0;
}

```

---

## 🔹 Ejemplo 2 — Lectura de nombres completos

**Archivo:** `LEERNOMBRES.c`  
**Descripción:** Programa que muestra tres formas de manejar cadenas en C para ingresar y mostrar nombres completos:  
1. Uso de un arreglo de caracteres estático.  
2. Uso de memoria dinámica con puntero y `malloc`.  
3. Uso de un puntero a cadena de solo lectura.

**Código:**
```c
#include <stdio.h>
#include <stdlib.h>
int main (){
    // Opcion 1, lista de caracteres (arreglo)
    /*char nombresCompletos[20];

    printf("Ingrese sus nombres completos\n");
    scanf("%[^\n]", nombresCompletos);
    getchar();
    printf("Sus nombres completos ingresados son: %s\n", nombresCompletos);*/

    // Opcion 2, puntero al inicio de una cadena 
   /*char * nombresCompletos = malloc(30 * sizeof(char));
     printf("Ingrese sus nombres completos\n");
    scanf("%[^\n]", nombresCompletos);
    getchar();
    printf("Sus nombres completos ingresados son: %s\n", nombresCompletos);*/

    // Opcion 3, solo lectura 
   char *nombresCompletos = "Jefferson Sarango";
     printf("Ingrese sus nombres completos\n");
    scanf("%[^\n]", nombresCompletos);
    getchar();
    printf("Sus nombres completos ingresados son: %s\n", nombresCompletos);

    //Reserva memoria dinamica 
    /*printf("ingrese sus nombres completos\n");
    scanf("%[^\n]" , nombresCompletos);
    getchar();
    printf("sus nombres ingresados son: %s\n", nombresCompletos)*/

    return 0;
}
```

---

## 🔹 Ejemplo 3 — Doble y triple de un número

**Archivo:** `dobletriple.c`  
**Descripción:** Programa que solicita un número al usuario y calcula su doble y su triple, mostrando ambos resultados.

**Código:**
```c
#include <stdio.h>
#include <string.h>

int main(){
    float valor ,doble,triple;
    printf("ingrese valor\n");
    scanf("%f", &valor);

    doble=valor*2;
    printf("el doble es:%.1f",doble);

    triple=valor*3;
    printf (" el triple es:%.1f", triple);

    return 0;


}
```

---

## 🔹 Ejemplo 4 — Conversión de pies a otras unidades

**Archivo:** `pedirpie.c`  
**Descripción:** Programa que convierte una cantidad dada en pies a yardas, pulgadas, centímetros y metros, mostrando los resultados equivalentes.

**Código:**
```c
#include <stdio.h>
#include <string.h>

int main(){
    float  pie,pg,yr,cm,mt;

    printf("ingrese pie\n");
    scanf("%f", &pie );

    yr=pie/3;
    pg=pie*12;
    cm=pg*2.54;
    mt=cm/100;

    printf("El resultado en yardas es:%.2f\n",yr);
    printf("El resultado pulgadas es:%.2f\n",pg);
    printf("El resultado centimentros es:%.2f\n",cm);
    printf("El resultado metros es:%.2f\n",mt);


    return 0;
}
```

---

## 🔹 Ejemplo 5 — Cálculo de aceleración

**Archivo:** `aceleracion.c`  
**Descripción:** Programa que calcula la aceleración de un objeto utilizando la fórmula física \( a = \frac{v_f - v_i}{t} \), donde se ingresan la velocidad inicial, la velocidad final y el tiempo.

**Código:**
```c
#include <stdio.h>
#include <string.h>

int main(){
    float  vi,vf,t,aceleracion;

    printf("ingrese velocidad inicial (m/s)\n");
    scanf("%f", &vi );

    printf("ingrese velocidad final (m/s)\n");
    scanf("%f", &vf );

    printf("ingrese el tiempo(s)\n");
    scanf("%f", &t );

    aceleracion=(vf-vi)/t;
    

    printf("la fuerza de aceleracion es:%f\n",aceleracion);
    

    return 0;
}
```

---

## 🔹 Ejemplo 6 — Conversión de metros a otras unidades

**Archivo:** `transformadordeunidades.c`
**Descripción:** Programa que convierte una cantidad en metros a kilómetros, centímetros y milímetros, mostrando los resultados con dos decimales.

**Código:**
```c
#include <stdio.h>
#include <string.h>

int main(){
    float  metros,km,cm,mm;

    printf("ingrese metros\n");
    scanf("%f", &metros );

    km=metros/1000;
    mm=1000;
    cm=metros*100;
    

    printf("El resultado en kilometros es:%.3f\n",km);
    printf("El resultado milimetros es:%.3f\n",mm);
    printf("El resultado centimentros es:%.3f\n",cm);


    return 0;
}
```
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

---
title: Crear un campo de fórmula en Lienzo de informes
description: Crear un campo de fórmula en Lienzo de informes
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: d649decb2875a3af4fd40c323a7836d4468bf04b
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 7%

---


# Crear un campo de fórmula en Lienzo de informes

El generador de campos en Lienzo de informes permite crear campos que realizan cálculos personalizados.

## Requisitos previos

Antes de comenzar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Reporting Canvas beta: información general](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Creación de un campo de fórmula

1. Cree o navegue hasta un bloque de tabla, tal como se describe en [Agregar o editar un bloque de tabla en el Lienzo de informes](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. En el encabezado de tabla del informe, haga clic en el botón **Editar** icono ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Si acaba de crear la tabla y aún no ha añadido ningún campo, haga clic en el botón Editar en el centro de la tabla.

1. Haga clic en **Nuevo +** en la parte superior del **Campos** en el panel derecho.
1. En la nueva página que se abre, haga clic en el botón **Editar** icono ![](assets/edit-icon.png) junto al nombre del campo en la esquina superior izquierda para cambiar el nombre del campo de fórmula.
1. Arrastrar **Funciones** o **Campos** del panel izquierdo al generador de campos central para añadirlos al campo de fórmula.


   >[!TIP]
   >
   >A medida que crea el campo de fórmula, la variable **Vista previa del campo** a la derecha muestra ejemplos del campo resultante.

   Cada función contiene varios rectángulos con puntos vacíos que se utilizarán como argumentos para calcular un resultado. Se pueden rellenar introduciendo texto estático o números, arrastrando y soltando un campo desde el panel izquierdo (utilizando el valor del campo en el cálculo) o arrastrando y soltando otra función (creando una función anidada). Las posibles funciones incluyen:

   | Función | Descripción | Salida |
   |---|---|---|
   | IF | Compare dos argumentos basados en un modificador seleccionado y luego realice una acción especificada basada en el valor resultante True (Is True:) o False (Is False:). Nota: actualmente, el segundo argumento no puede ser un valor estático True o False. En su lugar, puede utilizar una función anidada como ISBLANK (Nombre del proyecto) que siempre devuelva False como solución alternativa. | True/False, Date, Number o String |
   | CONCAT | Combine dos o más cadenas de forma integral para crear una cadena nueva. | Cadena |
   | CONTAINS | Evalúe si un campo de argumento de cadena (Buscar texto) está contenido en otro campo de argumento de cadena (En texto). | Verdadero/Falso |
   | EN | Evaluar si el valor de un campo de argumento (Find) coincide con el valor de al menos otro campo de argumento (Within) | Verdadero/Falso |
   | ISBLANK | Evalúe si un campo de argumento está en blanco. | Verdadero/Falso |
   | LEN | Mida la longitud (en número de caracteres) de un campo de argumento. | Número |
   | ROUND | Devuelve un número redondeado en función de la precisión seleccionada. | Número |
   | FLOOR | Devuelve el número entero más cercano, redondeado hacia abajo. | Número |
   | NÚMERO | Devuelve el valor bueno entero menor que el valor del argumento numérico (idéntico a una función Floor). | Número |
   | CADENA | Convierte el contenido de un campo de argumento en una cadena | Cadena |
   | SUBSTR | Cree una nueva cadena a partir de una cadena más grande, que contenga los caracteres entre un número de índice (Inicio) y otro (Final). | Cadena |
   | LEFT | Cree una nueva cadena a partir de una cadena más grande, que contenga caracteres que comiencen por el extremo izquierdo y contando a la derecha un número de caracteres (Longitud). | Cadena |
   | RIGHT | Cree una nueva cadena a partir de una cadena más grande, que contenga caracteres que comiencen por el extremo derecho y que cuente a la izquierda un número de caracteres (Longitud). | Cadena |
   | SUM | Agregue los valores de dos o más campos de argumento juntos. | Número |
   | SUB | Reste los valores de dos o más campos de argumento (en orden de izquierda a derecha). | Número |
   | PROD | Multiplique los valores de dos o más campos de argumento juntos. | Número |
   | DIV | Divida el valor de dos o más campos de argumento (en orden de izquierda a derecha). | Número |
   | MONTH | Devuelve un número igual al valor del mes de una fecha. | Número |
   | AÑO | Devuelve un número igual al valor de año de una fecha. | Número |
   | DATEDIFF | Calcula el número total de días entre dos fechas, redondeado a un decimal. | Número |
   | WEEKDAYDIFF | Calcula el número de días laborables entre dos fechas, redondeado a un decimal. | Número |

   {style=&quot;table-layout:auto&quot;}

1. Haga clic en el **Volver** en la esquina superior izquierda de la pantalla para volver a la tabla.

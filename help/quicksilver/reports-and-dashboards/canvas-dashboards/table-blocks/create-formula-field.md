---
title: Creación de un campo de fórmula en el lienzo de informes
description: Creación de un campo de fórmula en el lienzo de informes
hidefromtoc: true
hide: true
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 7%

---

# Creación de un campo de fórmula en el lienzo de informes

El generador de campos en el lienzo de informes permite crear campos que realicen cálculos personalizados.

## Requisitos previos

Antes de empezar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Lienzo de informes beta: descripción general](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Crear un campo de fórmula

1. Cree o navegue hasta un bloque de tabla, tal como se describe en [Agregue o edite un bloque de tabla en el lienzo de informes](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. En el encabezado de tabla del informe, haga clic en el icono **Editar** ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Si acaba de crear la tabla y aún no ha agregado ningún campo, haga clic en el botón Editar en el centro de la tabla.

1. Haga clic en **Nuevo +** en la parte superior de la lista **Campos** en el panel derecho.
1. En la nueva página que se abre, haga clic en el icono **Editar** ![](assets/edit-icon.png) junto al nombre del campo en la esquina superior izquierda para cambiar el nombre del campo de fórmula.
1. Arrastre **Funciones** o **Campos** desde el panel izquierdo al generador de campos en el centro para agregarlos al campo de fórmula.


   >[!TIP]
   >
   >A medida que crea el campo de fórmula, la **vista previa del campo** a la derecha muestra ejemplos del campo resultante.

   Cada función contiene un número de rectángulos de puntos vacíos que se utilizarán como argumentos para calcular un resultado. Estos se pueden rellenar introduciendo texto estático o números, arrastrando y soltando un campo desde el panel izquierdo (utilizando el valor del campo en el cálculo) o arrastrando y soltando otra función (creando una función anidada). Las funciones posibles incluyen:

   | Función | Descripción | Output |
   |---|---|---|
   | IF | Compare dos argumentos basados en un modificador seleccionado y, a continuación, realice una acción especificada basada en el valor True (Is True:) o False (Is False:) resultante. Nota: actualmente, el segundo argumento no puede ser un valor estático Verdadero o Falso. En su lugar, puede utilizar una función anidada como ISBLANK(Nombre del proyecto) que siempre devuelve False como solución alternativa. | Verdadero/Falso, Fecha, Número o Cadena |
   | CONCAT | Combine dos o más cadenas de extremo a extremo para crear una nueva cadena. | Cadena |
   | CONTAINS | Evalúe si un campo de argumento de cadena (texto de búsqueda) está contenido dentro de otro campo de argumento de cadena (dentro del texto). | Verdadero/Falso |
   | EN | Evalúe si el valor de un campo de argumento (Buscar) coincide con el valor de al menos otro campo de argumento (En) | Verdadero/Falso |
   | ISBLANK | Evalúe si un campo de argumento está en blanco. | Verdadero/Falso |
   | LEN | Mida la longitud (en número de caracteres) de un campo de argumento. | Número |
   | ROUND | Devuelve un número redondeado basado en la precisión seleccionada. | Número |
   | FLOOR | Devuelve el número entero más cercano, redondeado hacia abajo. | Número |
   | NÚMERO | Devuelve el mayor entero menor que el valor de un argumento numérico (idéntico a una función Floor). | Número |
   | CADENA | Convierte el contenido de un campo de argumento en una cadena | Cadena |
   | SUBSTR | Cree una nueva cadena a partir de una cadena mayor, que contenga los caracteres entre un número de índice (Inicio) y otro (Final). | Cadena |
   | LEFT | Cree una nueva cadena a partir de una cadena más grande, que contenga caracteres que empiecen por el extremo izquierdo y que cuenten a la derecha un número de caracteres (longitud). | Cadena |
   | RIGHT | Cree una nueva cadena a partir de una cadena más grande, que contenga caracteres que empiecen por el extremo derecho y que cuenten hacia la izquierda un número de caracteres (Longitud). | Cadena |
   | SUM | Agregue los valores de dos o más campos de argumento juntos. | Número |
   | SUB | Reste los valores de dos o más campos de argumento (en orden de izquierda a derecha). | Número |
   | PROD | Multiplique los valores de dos o más campos de argumento al mismo tiempo. | Número |
   | DIV | Divida el valor de dos o más campos de argumento (en orden de izquierda a derecha). | Número |
   | MONTH | Devuelve un número igual al valor de mes de una fecha. | Número |
   | AÑO | Devuelve un número igual al valor de año de una fecha. | Número |
   | DATEDIFF | Calcula el número total de días entre dos fechas, redondeado a un decimal. | Número |
   | WEEKDAYDIFF | Calcula el número de días de la semana entre dos fechas, redondeado a un decimal. | Número |

   {style="table-layout:auto"}

1. Haga clic en la flecha **Volver** situada en la esquina superior izquierda de la pantalla para volver a la tabla.

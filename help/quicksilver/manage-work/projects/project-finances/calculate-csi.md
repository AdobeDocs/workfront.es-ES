---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el Índice de Rendimiento del Programa de Costes (CSI)
description: El Índice de Rendimiento del Programa de Costes (CSI) es un cálculo automático que combina el Índice de Rendimiento de Costes (CPI) y el Índice de Rendimiento del Programa (SPI) en una métrica general que equilibra el costo y el programa.
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Calcular el Índice de Rendimiento del Programa de Costes (CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Visión General del Índice de Rendimiento del Programa de Costes (CSI)

El Índice de Rendimiento del Programa de Costes (CSI) es un cálculo automático que combina el Índice de Rendimiento de Costes (CPI) y el Índice de Rendimiento del Programa (SPI) en una métrica general que equilibra el costo y el programa. Al multiplicar estos valores juntos, una sola métrica puede representar una programación prolongada con un presupuesto inferior o viceversa. Los administradores de proyectos pueden utilizar esta opción para determinar el estado general del proyecto o de la tarea cuando se sacrifique el costo para impulsar la programación en mitad del proyecto.

>[!TIP]
>
>Adobe Workfront calcula CSI para tareas y proyectos. Workfront no calcula un valor CSI para problemas.

Puede beneficiarse de la información proporcionada por esta métrica solo si su organización cuenta con lo siguiente:

* Los usuarios están registrando la hora del trabajo que completan.\
   Esto calcula la CSI en función de las horas.
* Los usuarios o las funciones de trabajo tienen asociadas tasas de costo por hora. 

   Esto calcula la CSI en función de los costes.

## Cómo calcula Workfront el Índice de Rendimiento del Programa de Costes (CSI)

Workfront calcula el Índice de Rendimiento de Coste (CSI) de un proyecto o tarea mediante la fórmula siguiente:

```
CSI = CPI x SPI
```

Para obtener información sobre CPI, consulte el artículo [Calcular el índice de rendimiento de costes (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Para obtener información sobre SPI, consulte el artículo [Calcular el índice de rendimiento de la programación (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI tiene los tres valores posibles siguientes:

* 1 = Sigue el plan general   
* 
   >1 = Combinación de programación presupuestaria
* &lt;1 = Combinación de programación por encima del presupuesto

![](assets/csi-highlighted.png)

## Localizar el Índice de Rendimiento del Programa de Costes (CSI)

>[!CAUTION]
>
>Debe tener acceso a Ver datos financieros en su nivel de acceso y permisos para Ver el proyecto o la tarea para poder ver el valor CSI de un proyecto o tarea.

Puede ubicar CSI en las siguientes áreas de Workfront:

* Área de finanzas en la sección Detalles del proyecto .
* Área de finanzas en la sección Detalles de la tarea .
* Una vista de proyecto o tarea
* Un informe de proyecto o tarea

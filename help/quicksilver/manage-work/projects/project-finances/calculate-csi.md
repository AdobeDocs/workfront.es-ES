---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular índice de rendimiento de horario de costes (CSI)
description: El índice de rendimiento del horario de costes (CSI) es un cálculo automático que combina el índice de rendimiento de costes (CPI) y el índice de rendimiento del horario (SPI) en una métrica general que equilibra el coste y el horario.
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: 1cf679376517293f0e0f28b461bd9ecab9283035
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Calcular índice de rendimiento de horario de costes (CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Descripción general del índice de rendimiento del horario de costes (CSI)

El índice de rendimiento del horario de costes (CSI) es un cálculo automático que combina el índice de rendimiento de costes (CPI) y el índice de rendimiento del horario (SPI) en una métrica general que equilibra el coste y el horario. Al multiplicar estos valores juntos, una sola métrica puede explicar un horario prolongado con un presupuesto más bajo o viceversa. Los jefes de proyecto pueden utilizarlo para determinar el estado general de las tareas o los proyectos cuando se sacrifica el coste para controlar la programación a mitad del proyecto.

>[!TIP]
>
>Adobe Workfront calcula el CSI tanto para las tareas como para los proyectos. Workfront no calcula un valor CSI para los problemas.

Puede beneficiarse de la información proporcionada por esta métrica solo si su organización dispone de lo siguiente:

* Los usuarios están registrando el tiempo del trabajo que completan.\
  Calcula el CSI en función de las horas.
* Los usuarios o las funciones del puesto tienen asociadas tarifas de coste por hora. 

  Calcula los CSI en función de los costes.

## Cómo calcula Workfront el índice de rendimiento del horario de costes (CSI)

Workfront calcula el índice de rendimiento de costos (CSI) de un proyecto o tarea mediante la fórmula siguiente:

`CSI = CPI x SPI`

Para obtener información acerca del IRC, consulte el artículo [Calcular el índice de rendimiento de costos (IRC)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Para obtener información acerca de SPI, vea el artículo [Calcular el índice de rendimiento de horario (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI tiene los tres valores posibles siguientes:

* 1 = Sigue el plan general
* \>1 = Combinación de programación inferior al presupuesto
* &lt;1 = Combinación de horario de presupuesto excedido

![](assets/csi-highlighted.png)

## Busque el Índice de rendimiento del horario de costes (CSI)

>[!CAUTION]
>
>Debe tener acceso a Ver datos financieros en el nivel de acceso y permisos para Ver el proyecto o la tarea para poder ver el valor CSI de un proyecto o tarea.

Puede localizar CSI en las siguientes áreas de Workfront:

* Área Finanzas en la sección Detalles del proyecto.
* Área Finanzas en la sección Detalles de la tarea.
* Una vista de proyecto o tarea
* Informe de proyecto o tarea

---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el índice de rendimiento de programación de costes (CSI)
description: El índice de rendimiento de programación de costes (CSI) es un cálculo automático que combina el índice de rendimiento de costes (CPI) y el índice de rendimiento de programación (SPI) en una métrica general que equilibra el coste y la programación.
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
TQID: https://experienceleague.adobe.com/USODdaQOyE-D76BVmLLVUS1WxUMrK6Q05xZU1Xg9Gjc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 71%

---

# Calcular el índice de rendimiento de programación de costes (CSI)

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Información general sobre el índice de rendimiento de programación de costes (CSI)

El índice de rendimiento de programación de costes (CSI) es un cálculo automático que combina el índice de rendimiento de costes (CPI) y el índice de rendimiento de programación (SPI) en una métrica general que equilibra el coste y la programación. Al multiplicar estos valores juntos, una sola métrica puede explicar una programación prolongada con un presupuesto más bajo o viceversa. Los gestores de proyectos pueden utilizarlo para determinar el estado general de los proyectos o las tareas cuando se sacrifica el coste para impulsar la programación a mitad del proyecto.

>[!TIP]
>
>Adobe Workfront calcula el CSI tanto para las tareas como para los proyectos, pero no para los problemas.

Puede beneficiarse de la información proporcionada por esta métrica solo si existen los siguientes escenarios en su organización:

* Los usuarios están registrando el tiempo del trabajo que completan. Esto calcula el CSI en función de las horas.
* Los usuarios o las funciones del puesto tienen asociadas tarifas de coste por hora. Esto calcula el CSI en función de los costes.

## Cómo calcula Workfront el índice de rendimiento de programación de costes (CSI)

Workfront calcula el índice de rendimiento de costes (CSI) de un proyecto o tarea con la fórmula siguiente:

`CSI = CPI x SPI`

Para obtener más información sobre el CPI, consulte el artículo [Calcular el índice de rendimiento de costes (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Para obtener más información sobre el SPI, consulte el artículo [Calcular el índice de rendimiento de programación (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

El CSI tiene los tres valores posibles siguientes:

* 1 = Sigue el plan general
* \>1 = Combinación de programación por debajo del presupuesto
* &lt;1 = Combinación de programación por encima del presupuesto

![CSI](assets/csi-highlighted.png)

## Localizar el índice de rendimiento de programación de costes (CSI)

>[!CAUTION]
>
>Debe tener acceso a Ver datos financieros en el nivel de acceso y permisos para Ver el proyecto o la tarea para ver el valor CSI de un proyecto o tarea.

Puede localizar el CSI en las siguientes áreas de Workfront:

* Área Finanzas en la sección Detalles del proyecto.
* Área Finanzas en la sección Detalles de la tarea.
* Una vista de proyecto o de tarea.
* Informe de proyecto o tarea.

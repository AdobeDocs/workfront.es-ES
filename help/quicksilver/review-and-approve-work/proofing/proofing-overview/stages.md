---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Resumen de las etapas del flujo de trabajo automatizado
description: Las etapas de prueba son segmentos de tiempo en los que distintos usuarios revisan una prueba. A medida que la prueba pasa de una etapa a otra, Adobe Workfront notifica a los revisores de cuándo es el momento de trabajar en ella.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Resumen de las etapas del flujo de trabajo automatizado

Las etapas de prueba son segmentos de tiempo en los que distintos usuarios revisan una prueba. A medida que la prueba pasa de una etapa a otra, Adobe Workfront notifica a los revisores de cuándo es el momento de trabajar en ella.

![stage_chart.png](assets/stages-diagram-350x63.png)

Los escenarios se producen en dos situaciones diferentes:

* [Creación de una prueba con un flujo de trabajo automatizado](#create-a-proof-with-an-automated-workflow)
* [Asignar plazos a diferentes revisores en una prueba](#assign-deadlines-for-different-reviewers-on-a-proof)

## Creación de una prueba con un flujo de trabajo automatizado {#create-a-proof-with-an-automated-workflow}

Al añadir un flujo de trabajo automatizado a una prueba, se configuran las fases del trabajo de revisión que se desea que se produzcan.

Cuando se configuran etapas para una prueba con un flujo de trabajo automático:

* Puede configurar las etapas para que se ejecuten de forma consecutiva o simultánea.
* Puede configurar algunas etapas para que se activen solo después de completar una fase anterior.
* Puede convertir algunos escenarios en privados. Esto resulta útil, por ejemplo, para una agencia que revisa una prueba antes de compartirla con un cliente y no desea que los comentarios resultantes sean visibles para el cliente.

Para obtener instrucciones sobre la creación de etapas para una prueba con un flujo de trabajo automatizado, consulte [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>Si un usuario no está incluido en ninguna etapa pero tiene acceso al documento y abre la prueba, el sistema crea una etapa llamada *Workfront*.
>
>Al usuario que abrió la prueba se le asigna la función especificada en Configuración > Revisar y aprobar > Funciones para los no destinatarios que abren una prueba de documento.

## Asignar plazos a diferentes revisores en una prueba {#assign-deadlines-for-different-reviewers-on-a-proof}

Cuando asigna diferentes fechas límite de pruebas a los revisores en una prueba, el sistema crea una etapa para cada fecha límite y agrupa los revisores para cada fecha límite en la fase correspondiente. 

**Ejemplo:** Por ejemplo, si crea una prueba con cuatro revisores:

* Para los revisores Olivia y Tony, debe especificar una fecha límite para las 14:00 a partir de ahora.
* Para Aaron y Amy, especifique una fecha límite para las 17:00 unos días después.
* No especifica un plazo para usted.

El sistema crea una etapa para cada uno de estos tres &quot;grupos&quot; de revisores:

![stage.png](assets/stages-350x239.png)

Si comparte la prueba con otro revisor y no especifica una fecha límite, Workfront agrega el usuario a la Etapa 3, donde no hay fecha límite. 

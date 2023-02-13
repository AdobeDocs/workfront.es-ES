---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Administre una prueba configurada con un flujo de trabajo automatizado en [!DNL Workfront Proof]
description: Puede realizar un seguimiento del progreso de las pruebas de flujo de trabajo automatizado desde la sección Flujo de trabajo de la página Detalles de la prueba . Puede ver el trabajo realizado en cada etapa y modificar, añadir, iniciar y bloquear las etapas de la prueba.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1d0ad905-f3fb-471a-8766-096b978cdf4e
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Administre una prueba configurada con un flujo de trabajo automatizado en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Puede realizar un seguimiento del progreso de las pruebas de flujo de trabajo automatizado desde la sección Flujo de trabajo de la sección [!UICONTROL Detalles de la prueba] página. Puede ver el trabajo realizado en cada etapa y modificar, añadir, iniciar y bloquear las etapas de la prueba.

## Ver un flujo de trabajo automatizado

Puede ver el flujo de trabajo automatizado de tres formas principales:

* [Ver un escenario en detalle](#view-a-stage-in-detail)
* [Ver todas las etapas](#view-all-stages)
* [Ver todas las etapas en detalle](#view-all-stages-in-detail)

### Ver un escenario en detalle {#view-a-stage-in-detail}

1. Haga clic en el botón en la parte superior de la sección (1).

   Puede cambiar entre etapas mediante el diagrama. El escenario que está viendo está resaltado en gris (2).

1. Para ver un escenario diferente, selecciónelo en el diagrama.

![View_a_stage_in_detail.png](assets/view-a-stage-in-detail-350x249.png)

### Ver todas las etapas {#view-all-stages}

Para ver todas las etapas de un flujo de trabajo automatizado:

1. Haga clic en el botón en la parte superior de la página (3).

   En la sección se enumeran todas las etapas del flujo de trabajo automatizado, aunque los detalles están ocultos.

1. Para ver los detalles de una etapa, haga clic en el icono de signo más junto al nombre de cada etapa (4).

![View_all_stage.png](assets/view-all-stages-350x212.png)

### Ver todas las etapas en detalle {#view-all-stages-in-detail}

Para ver todas las etapas del flujo de trabajo automatizado en detalle:

1. Haga clic en el botón en la parte superior de la página (5).

   Esto le mostrará todas las etapas del flujo de trabajo automatizado con los detalles de cada etapa expandidos.

   Puede ocultar los detalles de cada etapa haciendo clic en el icono menos (6).

![View_all_stage_in_detail.png](assets/view-all-stages-in-detail-350x370.png)

## Uso del diagrama de flujo de trabajo automatizado

El diagrama de su [!UICONTROL Flujo de trabajo] se muestra en la parte superior de la sección Flujo de trabajo .

Ocultar el diagrama

1. Haga clic en el **[!UICONTROL Ocultar]** botón (1).

![Diagrama__1_.png](assets/diagram--1--350x217.png)

Las etapas del diagrama se marcan de la siguiente manera:

![dot.png](assets/dot.png)- una fase activa

![gray_dot.png](assets/grey-dot.png)- una fase inactiva\
![sbw-key-icon.png](assets/sbw-key-icon.png)  - un escenario privado

![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  - un escenario bloqueado

Las líneas entre las etapas representan las dependencias entre las etapas. Las líneas que conducen a etapas inactivas se puntean hasta que se activa el escenario.

Al pasar el ratón por encima de un escenario en el diagrama, se verá el progreso del escenario. Si el escenario no está activo y tiene derechos de edición en el escenario, podrá iniciar el escenario desde la ventana emergente utilizando la variable [!UICONTROL Iniciar etapa] botón. Del mismo modo, se muestra la opción Bloquear un escenario activo.

Para obtener más información sobre la barra de progreso, consulte  [Ver el progreso y estado de una prueba en [!DNL Workfront] Prueba](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

![Diagrama_-_stage_summary.png](assets/diagram---stage-summary-350x214.png)

## Agregar una nueva etapa

Puede agregar una nueva etapa al flujo de trabajo automatizado desde la [!UICONTROL Detalles de la prueba] página.

1. Haga clic en el **[!UICONTROL Nueva etapa]** botón (1).

![Adding_a_new_stage_1.png](assets/adding-a-new-stage-1-350x218.png)

En el **Nueva etapa** que aparece, puede rellenar los detalles y la configuración del escenario.

![Adding_a_new_stage_2.png](assets/adding-a-new-stage-2-350x332.png)

## Administrar configuración de escenario

En los detalles de la página puede modificar la configuración de cada etapa (si tiene derechos de edición):

* Cambiar, añadir o eliminar la fecha límite de la fase (1)
* Bloquear el escenario (2): esta opción aparece si el escenario está activo; para las etapas inactivas, verá la opción para Iniciar la etapa
* Modificación de la configuración mediante la edición en línea (3)
* Habilitar o deshabilitar Solo se requiere una decisión en el escenario (4)
* Cambiar la privacidad del escenario (5)

![Managing_stage_settings.png](assets/managing-stage-settings-350x93.png)

También puede mover los revisores entre etapas arrastrándolos y soltándolos de una etapa a otra. Los escenarios disponibles se resaltarán en azul con las áreas de colocación de cada etapa claramente marcadas.

![Moving_reviewers_between_stage.png](assets/moving-reviewers-between-stages-350x254.png)

## Opciones de escenario

La variable [!UICONTROL Acciones] (1) para cada etapa tiene las siguientes opciones:

* Mensaje todo (2): puede enviar un correo electrónico recordatorio a todos los revisores del escenario
* Compartir (3): puede añadir nuevos revisores al escenario
* Fase de eliminación (4): si el propietario de la prueba se encuentra en esa fase, se le pedirá que elija una nueva etapa para ellos

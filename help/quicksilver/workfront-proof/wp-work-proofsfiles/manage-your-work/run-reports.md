---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Ejecutar informes en [!DNL Workfront Proof]
description: Workfront Proof le permite ver informes para poder realizar un seguimiento del progreso del trabajo y la eficacia de sus equipos.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Ejecutar informes en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Workfront Proof le permite ver informes para poder realizar un seguimiento del progreso del trabajo y la eficacia de sus equipos.

Puede ver fácilmente la cantidad de pruebas que se crearon en su [!DNL Workfront Proof] , cuántas versiones están asociadas con cada prueba, el tiempo de respuesta y más.

## Requisitos previos

La disponibilidad de los informes depende del tipo de [!DNL Workfront Proof] niveles de cuenta y permisos de usuario.

* [Requisitos previos de la cuenta](#account-prerequisites)
* [Requisitos previos del usuario](#user-prerequisites)

### Requisitos previos de la cuenta {#account-prerequisites}

La información de informes solo está disponible con planes Premium.

### Requisitos previos del usuario {#user-prerequisites}

La información de los informes solo está disponible para los usuarios con acceso completo a todas las pruebas de su cuenta (es decir, los usuarios con al menos [Perfiles de permisos de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

En este panel puede

* Control del lapso de tiempo de los datos mostrados
* Analizar los cambios en las métricas a lo largo del tiempo
* Compruebe los detalles de un punto temporal seleccionado pasando el puntero sobre él
* Compruebe el número total de pruebas creadas en el lapso de tiempo seleccionado
* Compruebe el número promedio de versiones incluidas en los conjuntos completados de pruebas

## Visualización de informes {#viewing-reports}

1. Vaya a la **[!UICONTROL Tableros]** página.
1. Haga clic en el **[!UICONTROL Informes]** pestaña .\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. En el **[!UICONTROL Lapso de tiempo]** menú desplegable, seleccione si desea mostrar información sobre las pruebas creadas en las últimas 24 horas, 7 días, 30 días, 90 días o un período de tiempo personalizado.\
   Si selecciona un período de tiempo personalizado, seleccione las fechas de inicio y finalización y, a continuación, haga clic en **[!UICONTROL Aplicar]**.\
   La siguiente información se muestra para el período de tiempo seleccionado:\
   **Prueba creada:** Número de pruebas creadas dentro del período de tiempo seleccionado.\
   **Versiones Por Prueba:** Número promedio de versiones por prueba para todas las pruebas completadas (aprobadas o aprobadas con cambios) dentro del período de tiempo seleccionado.\
   **Tiempo de respuesta:** Promedio de tiempo desde el momento en que se creó la primera versión hasta el momento en que se tomó la decisión sobre la versión final.\
   **Hora de la primera actividad:** Tiempo promedio desde el momento en que se creó la prueba hasta el momento de la primera actividad de la prueba.\
   **Pruebas tardías:** Porcentaje medio de pruebas completadas (aprobadas o aprobadas con cambios) que tenían al menos una versión tardía dentro del período de tiempo seleccionado.\
   **Comentarios y respuestas:** Número promedio de comentarios y respuestas que se realizaron en todas las pruebas dentro del período de tiempo seleccionado.

1. (Opcional) Seleccione o anule la selección de **[!UICONTROL Mostrar intervalo mínimo-máximo]** para determinar si los valores mínimo y máximo se muestran en el gráfico.\
   Cuando se selecciona esta opción, se muestra un sombreado azul entre los valores mínimo y máximo registrados.

1. (Opcional) Puede filtrar los datos que se muestran, tal como se describe en [Filtrado de informes](#filtering-reports).

## Filtrado de informes {#filtering-reports}

De forma predeterminada, los datos mostrados en los informes incluyen toda la información de su [!DNL Workfront Proof] sistema. Puede utilizar filtros para mostrar únicamente información relevante para sus necesidades.

Para filtrar la información de informes:

1. Vaya a la **[!UICONTROL Tableros]** página.
1. Haga clic en el **[!UICONTROL Informes]** pestaña .\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Ejecute un informe, tal como se describe en [Visualización de informes](#viewing-reports).
1. Haga clic en **[!UICONTROL Filtro]**.

1. En el lado izquierdo de la página, seleccione entre las siguientes opciones de filtro:\
   **[!UICONTROL Tipo de prueba]:** Seleccione el tipo de pruebas que desea incluir en el informe.\
   **[!UICONTROL Decisiones]:** Seleccione las opciones para determinar si solo se han realizado pruebas que contengan determinadas decisiones.\
   **[!UICONTROL Destinatarios]:** Seleccione usuarios individuales para ver la información relacionada con las pruebas compartidas con los usuarios seleccionados.\
   **[!UICONTROL Propietarios de pruebas]:** Seleccione usuarios individuales para ver la información relacionada con las pruebas que poseen los usuarios seleccionados.\
   **[!UICONTROL Creadores de pruebas]:** Seleccione usuarios individuales para ver la información relacionada con las pruebas creadas por los usuarios seleccionados.\
   **[!UICONTROL Cuentas]:** Seleccione qué cuentas desea incluir en el informe.

1. Haga clic en **[!UICONTROL Aplicar]**.
1. (Opcional) Seleccione o anule la selección de **[!UICONTROL Mostrar intervalo mínimo-máximo]** para determinar si los valores mínimo y máximo se muestran en el gráfico.\
   Cuando se selecciona esta opción, se muestra un sombreado azul entre los valores mínimo y máximo registrados.

## Impresión de informes

1. Vaya a la **[!UICONTROL Tableros]** página.
1. Haga clic en el **[!UICONTROL Informes]** a continuación, haga clic en **[!UICONTROL Imprimir]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. Seleccione entre las distintas opciones de impresión disponibles.\
   Las opciones de impresión varían según el explorador y la versión del explorador que utilice.

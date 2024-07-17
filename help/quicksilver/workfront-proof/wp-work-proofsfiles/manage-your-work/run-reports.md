---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Ejecutar informes en  [!DNL Workfront Proof]
description: Workfront Proof le permite ver informes para poder realizar un seguimiento del progreso del trabajo y de la eficacia de sus equipos.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Ejecutar informes en [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* La funcionalidad de creación de informes <span class="previe">ya no está disponible en [!DNL Workfront Proof]. La ficha de informes aún se muestra, pero los datos no son precisos.</span>
> 
>* Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Workfront Proof le permite ver informes para poder realizar un seguimiento del progreso del trabajo y de la eficacia de sus equipos.

Puede ver fácilmente el número de pruebas que se crearon en su cuenta de [!DNL Workfront Proof], cuántas versiones hay asociadas a cada prueba, el tiempo de respuesta y más.

## Requisitos previos

La disponibilidad de los informes depende del tipo de cuenta de [!DNL Workfront Proof] y de los niveles de permisos de los usuarios.

* [Requisitos previos de cuenta](#account-prerequisites)
* [Requisitos previos del usuario](#user-prerequisites)

### Requisitos previos de cuenta {#account-prerequisites}

La información sobre los informes solo está disponible con los planes Premium.

### Requisitos previos del usuario {#user-prerequisites}

La información de creación de informes solo está disponible para usuarios con acceso completo a todas las pruebas de su cuenta (es decir, usuarios con al menos [Perfiles de permisos de pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

En este panel puede

* Controlar el lapso de tiempo de los datos mostrados
* Analizar los cambios en las métricas a lo largo del tiempo
* Para comprobar los detalles de un punto temporal seleccionado, pase el ratón sobre él
* Compruebe el número total de pruebas creadas en el lapso de tiempo seleccionado
* Comprobar el número promedio de versiones incluidas en los conjuntos de pruebas completados

## Visualización de informes {#viewing-reports}

1. Vaya a la página **[!UICONTROL Paneles]**.
1. Haga clic en la ficha **[!UICONTROL Informes]**.\
   ![informes_de_revisión.png](assets/proof-reports-350x193.png)

1. En el menú desplegable **[!UICONTROL Periodo de tiempo]**, seleccione si desea mostrar información sobre las pruebas creadas en las últimas 24 horas, 7 días, 30 días, 90 días o un período de tiempo personalizado.\
   Si selecciona un período de tiempo personalizado, seleccione las fechas de inicio y finalización y haga clic en **[!UICONTROL Aplicar]**.\
   Se muestra la siguiente información para el período de tiempo seleccionado:\
   **Prueba creada:** Número de pruebas creadas dentro del período de tiempo seleccionado.\
   **Versiones por prueba:** Cantidad promedio de versiones por prueba para todas las pruebas completadas (aprobadas o aprobadas con cambios) dentro del período de tiempo seleccionado.\
   **Tiempo de respuesta:** Tiempo promedio desde que se creó la primera versión hasta que se tomó la decisión sobre la versión final.\
   **Hora de la primera actividad:** Tiempo promedio desde que se creó la prueba hasta la hora de la primera actividad en la prueba.\
   **Pruebas retrasadas:** Porcentaje promedio de pruebas completadas (aprobadas o aprobadas con cambios) que tenían al menos una versión retrasada dentro del período de tiempo seleccionado.\
   **Comentarios y respuestas:** Cantidad promedio de comentarios y respuestas realizados en todas las pruebas dentro del período de tiempo seleccionado.

1. (Opcional) Seleccione o anule la selección de la opción **[!UICONTROL Mostrar rango mínimo-máximo]** para determinar si se muestran los valores mínimo y máximo en el gráfico.\
   Cuando se selecciona esta opción, se muestra un sombreado azul entre los valores mínimo y máximo registrados.

1. (Opcional) Puede filtrar los datos que se muestran, tal como se describe en [Filtrado de informes](#filtering-reports).

## Filtrado de informes {#filtering-reports}

De manera predeterminada, los datos que se muestran en los informes incluyen toda la información del sistema [!DNL Workfront Proof]. Puede utilizar filtros para mostrar únicamente la información que sea relevante para sus necesidades.

Para filtrar la información de informes:

1. Vaya a la página **[!UICONTROL Paneles]**.
1. Haga clic en la ficha **[!UICONTROL Informes]**.\
   ![informes_de_revisión.png](assets/proof-reports-350x193.png)

1. Ejecute un informe, tal como se describe en [Visualización de informes](#viewing-reports).
1. Haga clic en **[!UICONTROL Filtro]**.

1. En la parte izquierda de la página, seleccione una de las siguientes opciones de filtro:\
   **[!UICONTROL Tipo de revisión]:** Seleccione el tipo de revisiones que desea incluir en el informe.\
   **[!UICONTROL Decisiones]:** Seleccione opciones para determinar si solo se han realizado las pruebas que contienen determinadas decisiones.\
   **[!UICONTROL Destinatarios]:** Seleccione usuarios individuales para ver información relacionada con las pruebas compartidas con los usuarios seleccionados.\
   **[!UICONTROL Propietarios de revisión]:** Seleccione usuarios individuales para ver información relacionada con las pruebas que sean propiedad de los usuarios seleccionados.\
   **[!UICONTROL Creadores de pruebas]:** Seleccione usuarios individuales para ver información relacionada con las pruebas creadas por los usuarios seleccionados.\
   **[!UICONTROL Cuentas]:** Seleccione qué cuentas desea incluir en el informe.

1. Haga clic en **[!UICONTROL Aplicar]**.
1. (Opcional) Seleccione o anule la selección de la opción **[!UICONTROL Mostrar rango mínimo-máximo]** para determinar si se muestran los valores mínimo y máximo en el gráfico.\
   Cuando se selecciona esta opción, se muestra un sombreado azul entre los valores mínimo y máximo registrados.

## Impresión de informes

1. Vaya a la página **[!UICONTROL Paneles]**.
1. Haga clic en la ficha **[!UICONTROL Informes]** y, a continuación, haga clic en **[!UICONTROL Imprimir]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. Seleccione entre las distintas opciones de impresión disponibles.\
   Las opciones de impresión varían según la versión del explorador y del explorador que utilice.

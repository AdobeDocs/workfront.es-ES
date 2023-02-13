---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear un informe de valoración
description: Un informe de valoración mide en qué medida un proyecto se ajusta a los criterios establecidos anteriormente para un portafolio. Un informe de valoración a menudo refleja la misión, los valores y los objetivos estratégicos de una organización. Los administradores de Portfolio suelen definir las preguntas y respuestas del informe de valoración para garantizar que sean significativas y valiosas durante la priorización y selección del proyecto. Un [!DNL Adobe Workfront] el administrador crea los informes de valoración en función de las recomendaciones de los administradores de portafolios.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Crear un informe de valoración

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Un informe de valoración mide en qué medida un proyecto se ajusta a los criterios establecidos anteriormente para un portafolio. Un informe de valoración a menudo refleja la misión, los valores y los objetivos estratégicos de una organización.

Los administradores Portfolio suelen definir las preguntas y respuestas del informe de valoración para garantizar que sean significativas y valiosas durante la priorización y selección del proyecto. Un [!DNL Adobe Workfront] el administrador crea los informes de valoración en función de las recomendaciones de los administradores de portafolios.

Las preguntas y respuestas seleccionadas para un informe de valoración deben ser cuantificables para proporcionar un valor de alineación a fin de comparar diferentes proyectos.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>[!UICONTROL Business] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
 </tbody> 
</table>

## Crear un informe de valoración

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Informes de valoración]** y haga clic en **[!UICONTROL Nuevo informe de valoración]** para crear un nuevo informe de valoración e iniciar el generador de informes de valoración.

1. Especifique un **[!UICONTROL Nombre del informe de valoración]** y **[!UICONTROL Descripción]**.

   El nombre se muestra cuando asocia el informe de valoración con el proyecto. La descripción se muestra junto al nombre del informe de valoración en la lista del informe de valoración.

1. Haga clic en el **[!UICONTROL Agregar pregunta]** menú desplegable para abrir el [!UICONTROL pregunta de informe de valoración] y, a continuación, especifique la siguiente información para su pregunta:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pregunta]</td> 
      <td>Escriba la pregunta que desee incluir en el informe de valoración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Escriba los puntos máximos posibles para esta pregunta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Puntos negativos]</td> 
      <td>Seleccione esta opción para indicar que [!DNL Workfront] debe restar del total de puntos posibles. Las puntuaciones negativas no se pueden agregar a los puntos máximos posibles de un informe de valoración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de pantalla]</td> 
      <td>Select <strong>[!UICONTROL Value(0-100)]</strong> si desea mostrar un campo numérico en el informe de valoración en el que los usuarios pueden especificar cualquier valor entre 0 y 100.<p>O bien, seleccione <strong>[!UICONTROL Desplegable]</strong> o <strong>[!UICONTROL Botones de radio]</strong> para crear una respuesta, los usuarios pueden especificar mediante ese control. Haga clic en <strong>[!UICONTROL Agregar respuesta]</strong>y, a continuación, escriba la variable <strong>[!UICONTROL Valor]</strong> en puntos porcentuales para esta respuesta, en caso de que se cumpla. Si elige 100 %, el número de puntos asignados para esta pregunta se alcanza por completo. Si desea indicar que esta respuesta solo contiene una parte de la cantidad total de puntos asignados a esta pregunta, seleccione un valor de porcentaje inferior. Por ejemplo, si la pregunta se valora en 10 puntos y desea que esta respuesta lleve 5 de esos puntos, elija el 50% para el valor.</p>
      <p>Select <strong>[!UICONTROL Predeterminado]</strong> si desea indicar que esta respuesta es la predeterminada.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Agregar pregunta]** para agregar más preguntas y respuestas al informe de valoración, siga los mismos pasos.

   >[!NOTE]
   >
   >Puede reordenar las preguntas en el informe de valoración arrastrando y soltando las preguntas en el orden correcto.

1. Haga clic en **[!UICONTROL Guardar]** cuando haya terminado de introducir los datos.

## Aplicar un informe de valoración a un proyecto

Un usuario con [!UICONTROL administrar] Los permisos de un proyecto pueden aplicar un informe de valoración a un proyecto, una vez que el informe de valoración ha sido creado por el [!DNL Workfront] administrador.

Se agrega un informe de valoración a un proyecto como parte de la creación de un caso empresarial para el proyecto. Para obtener más información sobre cómo agregar un informe de valoración a un proyecto, consulte [Aplicar un informe de valoración a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para obtener más información sobre la creación de informes de valoración, consulte [Crear un informe de valoración](#create-a-scorecard).

Para obtener más información sobre los permisos del proyecto, consulte [Compartir un proyecto en [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

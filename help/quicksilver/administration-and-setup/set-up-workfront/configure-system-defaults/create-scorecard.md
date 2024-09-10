---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear un informe de valoración
description: Un cuadro de resultados mide en qué medida un proyecto se ajusta a los criterios previamente establecidos de un portafolio. Un informe de valoración suele reflejar la misión, los valores y los objetivos estratégicos de una organización.Los administradores de Portfolio suelen definir las preguntas y respuestas del informe de valoración para garantizar que sean significativas y valiosas durante la priorización y selección del proyecto. Un  [!DNL Adobe Workfront] administrador crea los cuadros de resultados en función de las recomendaciones de los administradores de portafolios.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 1%

---

# Crear cuadro de resultados

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Un cuadro de resultados mide en qué medida un proyecto se ajusta a los criterios previamente establecidos de un portafolio. Un cuadro de resultados suele reflejar la misión, los valores y los objetivos estratégicos de una organización.

Los administradores de Portfolio suelen definir las preguntas y respuestas del cuadro de resultados para garantizar que sean significativas y valiosas durante la priorización y selección del proyecto. Un administrador de [!DNL Adobe Workfront] crea los cuadros de resultados basándose en las recomendaciones de los administradores de portafolios.

Las preguntas y respuestas seleccionadas para un cuadro de resultados deben ser cuantificables para proporcionar un valor de alineación y comparar diferentes proyectos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Actual: [!UICONTROL Empresa] o superior</p> 
   O
   <p>Nuevo: [!UICONTROL Prime] o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Actual: [!UICONTROL plan]</p>
   O
   <p>Nuevo: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear cuadro de resultados

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Cuadros de resultados]** y, a continuación, haga clic en **[!UICONTROL Nuevo cuadro de resultados]** para iniciar el generador de cuadros de resultados y crear uno.

1. Especifique un **[!UICONTROL Nombre de informe de valoración]** y una **[!UICONTROL Descripción]**.

   El nombre se muestra al asociar el cuadro de resultados con el proyecto. La descripción se muestra junto al nombre del cuadro de mandos en la lista Cuadro de mandos.

1. Haga clic en el menú desplegable **[!UICONTROL Agregar pregunta]** para abrir la sección [!UICONTROL pregunta del cuadro de mandos] y, a continuación, especifique la siguiente información para la pregunta:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pregunta]</td> 
      <td>Escriba la pregunta que desee incluir en el informe de valoración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Puntos]</td> 
      <td>Escriba el máximo de puntos posible para esta pregunta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Puntos negativos]</td> 
      <td>Seleccione esta opción para indicar que [!DNL Workfront] debe restar del total de puntos posibles. Las puntuaciones negativas no se pueden agregar al máximo de puntos posibles de un cuadro de resultados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de pantalla]</td> 
      <td>Seleccione <strong>[!UICONTROL Value(0-100)]</strong> si desea mostrar un campo numérico en el cuadro de mandos donde los usuarios puedan especificar cualquier valor entre 0 y 100.<p>O bien, seleccione <strong>[!UICONTROL Drop Down]</strong> o <strong>[!UICONTROL Radio Buttons]</strong> para crear una respuesta que los usuarios puedan especificar mediante ese control. Haga clic en <strong>[!UICONTROL Agregar respuesta]</strong> y, a continuación, escriba el <strong>[!UICONTROL Valor]</strong> en puntos porcentuales para esta respuesta, en caso de que se complete. Si elige 100%, el número de puntos asignados para esta pregunta se alcanza por completo. Si desea indicar que esta respuesta sólo incluye una parte de la cantidad total de puntos asignados a esta pregunta, seleccione un valor porcentual inferior. Por ejemplo, si su pregunta tiene un valor de 10 puntos y desea que esta respuesta contenga 5 de esos puntos, elija 50% para su valor.</p>
      <p>Seleccione <strong>[!UICONTROL Default]</strong> si desea indicar que esta respuesta es la predeterminada.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Agregar pregunta]** para agregar más preguntas y respuestas a su cuadro de resultados, siguiendo los mismos pasos.

   >[!NOTE]
   >
   >Puede reordenar las preguntas del cuadro de resultados arrastrando y soltando las preguntas en el orden correcto.

1. Haga clic en **[!UICONTROL Guardar]** cuando termine de escribir toda la información.

   Esto crea el cuadro de resultados y los jefes de proyecto ahora pueden adjuntarlo a su caso comercial del proyecto.

## Aplicar un cuadro de resultados a un proyecto

Un usuario con permisos para [!UICONTROL administrar] en un proyecto puede aplicar un cuadro de mandos a un proyecto una vez que el administrador de [!DNL Workfront] haya creado el cuadro de mandos.

Se agrega un cuadro de mandos a un proyecto como parte de la creación de un caso empresarial para el proyecto. Para obtener más información sobre cómo agregar un cuadro de mandos a un proyecto, vea [Aplicar un cuadro de mandos a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para obtener más información acerca de los permisos del proyecto, vea [Compartir un proyecto en [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

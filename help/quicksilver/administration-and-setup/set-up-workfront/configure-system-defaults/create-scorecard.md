---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear un informe de valoración
description: Un cuadro de resultados mide en qué medida un proyecto se ajusta a los criterios previamente establecidos de un portafolio. Un informe de valoración suele reflejar la misión, los valores y los objetivos estratégicos de una organización.Los administradores de Portfolio suelen definir las preguntas y respuestas del informe de valoración para garantizar que sean significativas y valiosas durante la priorización y selección del proyecto. Un [!DNL Adobe Workfront] El administrador crea los cuadros de resultados en función de las recomendaciones de los administradores de portafolios.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Crear un informe de valoración

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Un cuadro de resultados mide en qué medida un proyecto se ajusta a los criterios previamente establecidos de un portafolio. Un cuadro de resultados suele reflejar la misión, los valores y los objetivos estratégicos de una organización.

Los administradores de Portfolio suelen definir las preguntas y respuestas del cuadro de resultados para garantizar que sean significativas y valiosas durante la priorización y selección del proyecto. Un [!DNL Adobe Workfront] El administrador crea los cuadros de resultados en función de las recomendaciones de los administradores de portafolios.

Las preguntas y respuestas seleccionadas para un cuadro de resultados deben ser cuantificables para proporcionar un valor de alineación y comparar diferentes proyectos.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Actual: [!UICONTROL Empresa] o superior</p> 
   O
   <p>Nuevo: [!UICONTROL Prime] o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td><p>Actual:[!UICONTROL plan]</p>
   O
   <p>Nuevo: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

## Crear un informe de valoración

{{step-1-to-setup}}

1. Clic **[!UICONTROL Cuadros de resultados]**, luego haga clic en **[!UICONTROL Nuevo informe de valoración]** para iniciar el generador de cuadros de resultados y crear un cuadro de resultados.

1. Especifique un **[!UICONTROL Nombre del informe de valoración]** y una **[!UICONTROL Descripción]**.

   El nombre se muestra al asociar el cuadro de resultados con el proyecto. La descripción se muestra junto al nombre del cuadro de mandos en la lista Cuadro de mandos.

1. Haga clic en **[!UICONTROL Añadir pregunta]** menú desplegable para abrir el [!UICONTROL pregunta del cuadro de resultados] y, a continuación, especifique la siguiente información para la pregunta:

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
      <td>Seleccionar <strong>[!UICONTROL Valor(0-100)]</strong> si desea mostrar un campo numérico en el cuadro de mandos en el que los usuarios pueden especificar cualquier valor entre 0 y 100.<p>O bien, seleccione <strong>Lista desplegable de [!UICONTROL]</strong> o <strong>Botones de opción [!UICONTROL]</strong> para crear una respuesta, los usuarios pueden especificar mediante ese control. Clic <strong>[!UICONTROL Agregar respuesta]</strong>, luego escriba el <strong>[!UICONTROL Valor]</strong> en puntos porcentuales para esta respuesta, en caso de que se cumpla. Si elige 100%, el número de puntos asignados para esta pregunta se alcanza por completo. Si desea indicar que esta respuesta sólo incluye una parte de la cantidad total de puntos asignados a esta pregunta, seleccione un valor porcentual inferior. Por ejemplo, si su pregunta tiene un valor de 10 puntos y desea que esta respuesta contenga 5 de esos puntos, elija 50% para su valor.</p>
      <p>Seleccionar <strong>[!UICONTROL Predeterminado]</strong> si desea indicar que esta respuesta es la predeterminada.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Añadir pregunta]** para agregar más preguntas y respuestas al informe de valoración, siga los mismos pasos.

   >[!NOTE]
   >
   >Puede reordenar las preguntas del cuadro de resultados arrastrando y soltando las preguntas en el orden correcto.

1. Clic **[!UICONTROL Guardar]** cuando haya terminado de introducir toda la información.

   Esto crea el cuadro de resultados y los jefes de proyecto ahora pueden adjuntarlo a su caso comercial del proyecto.

## Aplicar un cuadro de resultados a un proyecto

Un usuario con [!UICONTROL administrar] Los permisos de para un proyecto pueden aplicar un cuadro de resultados a un proyecto, una vez que el [!DNL Workfront] administrador.

Se agrega un cuadro de mandos a un proyecto como parte de la creación de un caso empresarial para el proyecto. Para obtener más información sobre cómo agregar un cuadro de mandos a un proyecto, consulte [Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para obtener más información sobre los permisos del proyecto, consulte [Uso compartido de un proyecto en [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

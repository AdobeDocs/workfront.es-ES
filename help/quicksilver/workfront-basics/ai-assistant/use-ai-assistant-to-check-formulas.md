---
title: Revisión de fórmulas de campos calculados con el Asistente de IA
content-type: reference
description: Puede utilizar el Asistente de IA para resolver errores en las expresiones personalizadas no válidas en los campos calculados.
author: Becky
feature: Get Started with Workfront
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 09c05db7c6a5db7db74dd95ca323415f4318489d
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Generar o revisar fórmulas de campos calculados con el Asistente de IA

Puede utilizar el Ayudante de IA para generar fórmulas basadas en una solicitud proporcionada. También puede resolver errores en las expresiones personalizadas no válidas en los campos calculados.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td><p>Nuevo: Prime o Ultimate</p>
       <p>o</p>
       <p>Actual: no disponible</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: no disponible</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Generación de una expresión de campo calculado

## Revisión de una expresión de campo calculado

Al crear el campo calculado en el generador de formularios personalizado, aparece un mensaje de error debajo del campo si la fórmula no es válida.

![Error de expresión no válido](assets/invalid-expression.png)

El Asistente de IA puede ayudarle a revisar la fórmula para convertirla en una expresión de campo calculado válida.

Para revisar una expresión de campo calculado no válida:

1. Haga clic en el icono **Asistente de IA** ![Icono del Asistente de IA](assets/ai-assistant-icon.png) cerca de la esquina superior derecha de la pantalla.
1. en el área de solicitud cerca de la parte inferior del panel Asistente de IA, introduzca una solicitud como:
   `Rewrite this formula to remove the invalid expression error`
1. Copie la expresión no válida del creador de formularios personalizados y péguela en el área de solicitud.
1. Presione **Intro**.

   El Asistente de IA puede tardar unos momentos en generar la fórmula revisada, según su tamaño o complejidad.
1. Vea la fórmula revisada en el panel Asistente para IA.
1. (Opcional) Copie la fórmula revisada del panel Asistente de IA y péguela en el campo calculado del creador de formularios personalizados.

>[!NOTE]
>
>Se recomienda probar el campo calculado para asegurarse de que recupera el resultado esperado.

Para obtener más información sobre los campos calculados en Workfront, consulte [Agregar campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '''Ejemplo de campo personalizado calculado: mostrar una marca de tiempo de estado en un formulario personalizado'
description: El siguiente campo calculado muestra la fecha en la que el estado del objeto está marcado como In Progress (INP). Puede utilizar la misma información para campos personalizados calculados para problemas, tareas o proyectos.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Ejemplo de campo personalizado calculado: mostrar una marca de tiempo de estado en un formulario personalizado

El siguiente campo calculado muestra la fecha en la que el estado del objeto está marcado como In Progress (INP). Puede utilizar la misma información para campos personalizados calculados para problemas, tareas o proyectos.

>[!NOTE]
>
>Si el estado del objeto cambia a INP, cambia a otro estado y, a continuación, a INP, Adobe Workfront captura solo la marca de tiempo del primer cambio a INP.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Editar acceso a Crear informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Administre permisos en el objeto al que está adjunto el formulario</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.<br>Para obtener más información sobre los permisos de los tableros, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Compartir informes, tableros y calendarios </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisito previo

Para agregar un campo calculado que muestre el historial de edición de un campo a un formulario personalizado, primero debe crear el formulario personalizado.

## Mostrar una marca de tiempo de estado en un formulario personalizado

1. Vaya a un formulario personalizado en el que desee agregar el campo .
1. Haga clic en **Calculado** para agregar un campo personalizado calculado al formulario.
1. Tipo a **Etiqueta** para el campo personalizado, como *Campo personalizado con marca de tiempo de estado*.
1. Haga clic en **Listo** y haga clic en **Guardar y cerrar**.
1. Vuelva a abrir el formulario personalizado y seleccione el nuevo **Campo personalizado con marca de tiempo de estado** en el formulario.
1. En el **Cálculo** , copie y pegue el siguiente cálculo para su campo personalizado:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Este cálculo es idéntico para todos los objetos y para todos los estados. En este cálculo debe utilizar siempre la clave de tres letras y no el nombre del estado del objeto.
   >
   >Para obtener más información sobre las claves de los estados, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Haga clic en **Guardar y cerrar**.

   Ahora puede crear informes sobre el campo personalizado Marca de tiempo de estado o utilizarlo en otros cálculos, en informes o en campos personalizados.

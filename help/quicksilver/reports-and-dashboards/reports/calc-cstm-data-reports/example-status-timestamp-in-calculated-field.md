---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Ejemplo de campo personalizado calculado: mostrar una marca de tiempo de estado en un formulario personalizado'
description: El siguiente campo calculado muestra la fecha en la que el estado del objeto se marca como En curso (INP). Puede utilizar la misma información para los campos personalizados calculados para problemas, tareas o proyectos.
author: Courtney
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 86%

---

# Ejemplo del campo personalizado calculado: mostrar una marca de tiempo de estado en un formulario personalizado

El siguiente campo calculado muestra la fecha en la que el estado del objeto se marca como En curso (INP). Puede utilizar la misma información para los campos personalizados calculados para problemas, tareas o proyectos.

>[!NOTE]
>
>Si el estado del objeto cambia a INP, entonces cambia a otro estado y, a continuación, vuelve a INP. Adobe Workfront captura únicamente la marca de tiempo del primer cambio a INP.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Paquete de Adobe Workfront</p> </td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront</p> </td> 
   <td>
      <p>Estándar</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configuraciones de nivel de acceso</p></td> 
   <td> <p>Editar el acceso a Creación de informes, paneles de control y calendarios</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto</p> </td> 
   <td> <p>Administrar permisos en el objeto donde se adjunta el formulario</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisito previo

Para añadir un campo calculado que muestre el historial de edición de un campo a un formulario personalizado, primero debe crear el formulario personalizado.

## Mostrar una marca de tiempo de estado en un formulario personalizado

1. Vaya a un formulario personalizado en el que desee añadir el campo.
1. Haga clic en **Calculado** para añadir un campo personalizado calculado al formulario.
1. Escriba **Label** para el campo personalizado. Por ejemplo, &quot;Campo personalizado de marca de tiempo de estado&quot;.
1. Haga clic en **Guardar + Cerrar**.
1. Vuelva a abrir el formulario personalizado y, a continuación, seleccione el nuevo **Campo personalizado de marca de tiempo de estado** en el formulario.
1. En el cuadro **Cálculo**, copie y pegue el siguiente cálculo para el campo personalizado:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Este cálculo es idéntico para todos los objetos y todos los estados. En este cálculo siempre se debe utilizar la clave de tres letras, y no el nombre del estado del objeto.
   >
   >Para obtener más información acerca de las claves de los estados, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Haga clic en **Guardar + Cerrar**.

   Ahora puede crear informes sobre el campo personalizado Marca de tiempo de estado o utilizarlo en otros cálculos, en informes o en campos personalizados.

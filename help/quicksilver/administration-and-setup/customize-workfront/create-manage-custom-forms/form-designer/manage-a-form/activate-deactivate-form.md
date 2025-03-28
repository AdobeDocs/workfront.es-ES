---
title: Desactivar o reactivar un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede reactivar o desactivar un formulario personalizado. Se recomienda desactivar los formularios personalizados en lugar de eliminar los formularios que ya no utilice para conservar los datos históricos.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: a7be72f0a594a21baed2592d8a2e467118ab1b7f
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 98%

---

# Desactivar o reactivar un formulario personalizado

Puede reactivar o desactivar un formulario personalizado. Se recomienda desactivar los formularios personalizados en lugar de eliminar los formularios que ya no utilice para conservar los datos históricos.

>[!NOTE]
>
>Si se desactiva un formulario personalizado que sigue formando parte de un tema de cola o de una definición de cola de solicitudes, se adjuntará a nuevas solicitudes. Si no desea que el formulario esté en las solicitudes, debe eliminarlo manualmente de la cola de solicitudes.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p></td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desactivar un formulario personalizado

Puede desactivar los formularios personalizados que ya no utilice sin perder los datos históricos asociados. Los usuarios no pueden añadir un formulario personalizado inactivo a los objetos, pero pueden ver y añadir datos a sus campos en objetos en los que ya estaba adjunto.

Los campos de un formulario personalizado inactivo también están disponibles para su edición en línea en una vista. Si un usuario añade un campo desde un formulario personalizado inactivo durante una edición en línea, el formulario se adjunta al objeto automáticamente, aunque el formulario personalizado esté desactivado.

Para desactivar un formulario personalizado:

{{step-1-to-setup}}

1. En el panel izquierdo, elija **Formularios personalizados**.
1. En el área **Formularios**, seleccione el formulario personalizado que desee desactivar.
1. En la columna Activo, elija **Falso** y haga clic fuera de la columna. El formulario ya no está activo.

## Reactivar un formulario personalizado

Si reactiva un formulario personalizado, conservará la configuración que tenía antes y los usuarios podrán interactuar con él como si nunca se hubiera desactivado.

{{step-1-to-setup}}

1. En el panel izquierdo, elija **Formularios personalizados**.
1. En el área **Formularios**, seleccione el formulario personalizado que desea reactivar.
1. En la columna Activo, elija **Verdadero** y haga clic fuera de la columna. El formulario ahora está activo.

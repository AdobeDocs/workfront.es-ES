---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Ejemplo de campo personalizado calculado: mostrar una marca de tiempo de estado en un formulario personalizado'
description: El siguiente campo calculado muestra la fecha en la que el estado del objeto se marca como En curso (INP). Puede utilizar la misma información para los campos personalizados calculados para problemas, tareas o proyectos.
author: Courtney
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OsYpPu9dAsSEQE6BBkvGovNR5E6I7k0BC2n48R7psLg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 343
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
1. Escriba una **Etiqueta** para el campo personalizado. Por ejemplo, &quot;Campo personalizado Marca de tiempo de estado&quot;.
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

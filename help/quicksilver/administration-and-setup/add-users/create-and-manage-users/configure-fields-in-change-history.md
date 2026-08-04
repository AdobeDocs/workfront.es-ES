---
user-type: administrator
product-area: system-administration;setup
title: Configurar campos para su seguimiento en el historial de cambios
description: Como administrador de Workfront, puede configurar qué campos de objeto y acciones rastrea Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 20%

---

# Configurar campos para realizar un seguimiento en el historial de cambios

{{highlighted-preview-article-level}}

Adobe Workfront genera actualizaciones automáticas del sistema para registrar los siguientes eventos:

* Cambios que los usuarios realizan en un campo de objeto
* Acciones que los usuarios realizan en un objeto

Estas actualizaciones del sistema incluyen el siguiente tipo de información:

* El cambio que se realizó
* El nombre del usuario que realizó el cambio
* La fecha y hora del cambio

Como administrador de Workfront, puede configurar qué campos de objeto y acciones rastrea Workfront.

Por ejemplo, puede hacer que Workfront rastree todos los cambios que los usuarios realizan en los nombres de los problemas en todo el sistema. Cualquier cambio de nombre de problema aparece como una entrada en el registro del historial de cambios. Para obtener más información, vea [Ver y administrar el historial de cambios](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Límites al seguimiento de campos

Los límites del número de campos que puede rastrear se definen en el paquete de Workfront.

| paquete de Workfront | Número máximo de campos rastreados |
|---------|----------|
| Seleccionar | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| Selección de flujo de trabajo | 1000 |
| Workflow Prime | 5000 |
| Workflow Ultimate | Sin límites |

## Añada los campos que desee rastrear

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios > Configuración**.
1. En la pantalla Configuración, haga clic en **Agregar campo**.
1. En el cuadro **Agregar campos**, seleccione un objeto. Puede empezar a escribir el nombre del objeto y, a continuación, seleccionarlo cuando aparezca en la lista.
1. A continuación, seleccione los nombres de campo que desea rastrear para ese objeto. Puede empezar a escribir el nombre del campo y, a continuación, seleccionarlo cuando aparezca en la lista.

   Tanto los campos personalizados como los campos nativos están disponibles para el objeto.
   Los campos que ya se están rastreando se muestran como seleccionados en la lista.

   ![Agregar campos para el seguimiento de cambios](assets/change-history-config-add-fields.png)

1. Después de seleccionar todos los campos que desea rastrear, haga clic en **Agregar**.

   Los campos se agregan a la lista Campos rastreados.

## Elimine los campos de los que ya no desea realizar un seguimiento

Puede eliminar campos que no desee que el sistema rastree para un tipo particular de objeto en toda la interfaz de Workfront.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios > Configuración**.
1. En la pantalla Configuración, seleccione el campo o campos sobre los que desea detener el seguimiento.

   Puede ver el mismo nombre de campo más de una vez. Los campos se agrupan por objeto para que pueda localizar el campo correcto. También puede utilizar el cuadro de búsqueda en la parte superior de la pantalla.

1. Seleccione **Eliminar** en la barra de acciones de la parte inferior de la pantalla.
1. Haz clic en **Quitar** en el mensaje de confirmación.

   Los campos se quitan de la lista Campos rastreados.



---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensaje de error: SAML 2.0 Error: User Identifier Not Found'
description: No puede establecer correctamente una conexión con ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 95%

---

# Mensaje de error: SAML 2.0 Error: User Identifier Not Found

## Problema

No puede establecer correctamente una conexión con ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Si establece una conexión de prueba satisfactoria y sigue teniendo problemas, es posible que tenga asignaciones de atributos incorrectas o problemas con los identificadores de federación. Póngase en contacto con el Servicio de atención al cliente si tiene alguna pregunta.

## Causa:

Las notificaciones en el servidor ADFS son incorrectas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

En el servidor ADFS, asegúrese de que haya una notificación para el identificador de nombre:

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Aparece el cuadro de diálogo Administración de ADFS 2.0.

1. Seleccione **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confianzas de terceros confiables]** en el panel izquierdo.

1. Haga clic con el botón derecho en la confianza del usuario de confianza relacionada con Adobe Workfront y seleccione **[!UICONTROL Editar reglas de notificación]**.
1. Compruebe que la notificación tiene un **[!UICONTROL tipo de notificación saliente]** de **[!UICONTROL Identificador de nombre]**.

![1.png](assets/1-350x287.png)

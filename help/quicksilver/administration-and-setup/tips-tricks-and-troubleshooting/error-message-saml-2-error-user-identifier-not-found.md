---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensaje de error: Error de SAML 2.0: Identificador de usuario no encontrado"
description: No puede establecer correctamente una conexión con ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---

# Mensaje de error: SAML 2.0 Error: Identificador de usuario no encontrado

## Problema

No puede establecer correctamente una conexión con ADFS.

![identificador_no_encontrado.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Si establece correctamente una conexión de prueba y sigue teniendo problemas, es posible que tenga asignaciones de atributos incorrectas o problemas con los Federation ID. Póngase en contacto con Atención al cliente si tiene alguna pregunta.

## Causa:

Las notificaciones en el servidor ADFS son incorrectas.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

En el servidor ADFS, asegúrese de que haya una notificación para el ID de nombre:

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Aparece el cuadro de diálogo Administración de ADFS 2.0.

1. Seleccione **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confianzas de usuario de confianza]** en el panel izquierdo.

1. Haga clic con el botón derecho en la confianza de usuario autenticado relacionada con Adobe Workfront y seleccione **[!UICONTROL Editar reglas de reclamación]**.
1. Compruebe que la notificación tiene **[!UICONTROL tipo de notificación saliente]** de **[!UICONTROL identificador de nombre]**.

![1.png](assets/1-350x287.png)

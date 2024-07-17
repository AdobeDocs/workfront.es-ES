---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensaje de error: Error de SAML 2.0: Identificador de usuario no encontrado"
description: No puede establecer correctamente una conexión con ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '219'
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

Las notificaciones en el servidor ADFS son incorrectas

## Requisitos de acceso

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

En el servidor ADFS, asegúrese de que haya una notificación para el ID de nombre:

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Aparece el cuadro de diálogo Administración de ADFS 2.0.

1. Seleccione **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confianzas de usuario de confianza]** en el panel izquierdo.

1. Haga clic con el botón derecho en la confianza de usuario autenticado relacionada con Adobe Workfront y seleccione **[!UICONTROL Editar reglas de reclamación]**.
1. Compruebe que la notificación tiene **[!UICONTROL tipo de notificación saliente]** de **[!UICONTROL identificador de nombre]**.

![1.png](assets/1-350x287.png)

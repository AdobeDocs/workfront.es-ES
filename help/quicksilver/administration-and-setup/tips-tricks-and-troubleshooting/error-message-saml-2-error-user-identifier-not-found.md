---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Mensaje de error: Error de SAML 2.0: Identificador de usuario no encontrado'
description: No puede establecer una conexión correcta con ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Mensaje de error: Error de SAML 2.0: Identificador de usuario no encontrado

## Problema

No puede establecer una conexión correcta con ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Si establece una conexión de prueba correcta y sigue teniendo problemas, es posible que tenga asignaciones de atributos incorrectas o problemas con los ID de federación. Póngase en contacto con el servicio de atención al cliente si tiene alguna pregunta.

## Causa:

Las solicitudes en el servidor ADFS son incorrectas

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
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

En el servidor ADFS, asegúrese de que haya una solicitud para el ID de nombre:

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Se muestra el cuadro de diálogo Administración de ADFS 2.0 .

1. Select **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confiar en las confianzas del partido]** en el panel izquierdo.

1. Haga clic con el botón derecho en la confianza de la parte que confía relacionada con Adobe Workfront y seleccione **[!UICONTROL Editar reglas de solicitud]**.
1. Compruebe que la reclamación tiene un **[!UICONTROL Tipo de reclamación saliente]** de **[!UICONTROL ID de nombre]**.

![1.png](assets/1-350x287.png)

---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensaje de error: Error de autenticación de SAML 2.0: Identificador de usuario no encontrado"
description: Cuando utiliza SAML 2.0, el error "No se encontró el identificador de usuario con error de autenticación SAML 2.0" significa que no se pasa un UID o ID de NOMBRE desde las reglas de notificación de ADFS. En ADFS, la confianza de usuario de confianza debe tener una regla de notificación que pase un UID o un valor de ID de NOMBRE. Si ejecuta una  [!DNL Workfront] conexión de prueba, debería mostrarla si se realiza correctamente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Mensaje de error: Error de autenticación de SAML 2.0: Identificador de usuario no encontrado

## Problema

Recibo este error al usar SAML 2.0: &quot;Error de autenticación de SAML 2.0: no se encontró el identificador de usuario&quot;.

## Causa

Esto sucede cuando no se pasa un **UID** o **ID DE NOMBRE** desde las **reglas de notificación de ADFS**.

En ADFS, la **confianza de usuario de confianza** necesita tener una **regla de reclamación** que pase un **UID** o un valor **NAME ID**. Cuando ejecuta una conexión de prueba **[!DNL Workfront]**, debería mostrarla si se realiza correctamente.

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

1. Al editar la **[!UICONTROL INFORMACIÓN ADFS]**, en **[!UICONTROL Confianzas de usuario de confianza]** > Seleccionar objeto >**[!UICONTROL Editar reglas de notificación]**.

1. El **[!UICONTROL atributo LDAP]** (columna izquierda) debe tener **[!UICONTROL direcciones de correo electrónico]** (o cualquier identificador único).

1. El **[!UICONTROL tipo de notificación saliente]** (columna derecha) debe ser **[!UICONTROL identificador de nombre]**.

   >[!NOTE]
   >
   >No tiene que tener las direcciones de correo electrónico de atributos LDAP. Se puede usar cualquier identificador único que identifique al usuario, pero debe pasarse a [!DNL Adobe Workfront] como **NAME ID**.

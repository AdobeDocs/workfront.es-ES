---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Mensaje de error: Error en la autenticación SAML 2.0: Identificador de usuario no encontrado'
description: Cuando utiliza SAML 2.0, el error "No se encontró el identificador de usuario fallido de autenticación SAML 2.0" significa que no se pasa un UID o ID de nombre de las reglas de reclamación de ADFS. En ADFS, el fideicomiso debe tener una regla de Reclamación que pase un UID o un valor de ID de NOMBRE. Al ejecutar un [!DNL Workfront] Probar conexión, debería mostrar esto si se realiza correctamente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Mensaje de error: Error en la autenticación SAML 2.0: Identificador de usuario no encontrado

## Problema

Recibo este error al utilizar SAML 2.0: &quot;Error en la autenticación SAML 2.0: No Se Encontró El Identificador De Usuario.&quot;

## Causa

Esto sucede cuando se **UID** o **ID DE NOMBRE** no se pasa desde la variable **Reglas de reclamación de ADFS**.

En ADFS, la variable **Confiar en la confianza de las partes** necesita tener un **Regla de reclamación** que pase un **UID** o **ID DE NOMBRE** valor. Al ejecutar un **[!DNL Workfront]Probar conexión**, debería mostrarlo si se realiza correctamente.

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

1. Al editar el **[!UICONTROL INFORMACIÓN DE ADFS]**, en el **[!UICONTROL Confiar en las confianzas del partido]** > Seleccionar objeto >**[!UICONTROL Editar reglas de solicitud]**.

1. La variable **[!UICONTROL Atributo LDAP]** (columna izquierda) debe tener **[!UICONTROL Direcciones de correo electrónico]** (o cualquier identificador único).

1. La variable **[!UICONTROL Tipo de reclamación saliente]** (columna derecha) debe ser **[!UICONTROL ID de nombre]**.

   >[!NOTE]
   >
   >No necesita tener las direcciones de correo electrónico del atributo LDAP. Se puede utilizar cualquier identificador único que identifique al usuario, pero debe pasarse a [!DNL Adobe Workfront] como el **ID DE NOMBRE**.

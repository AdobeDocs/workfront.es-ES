---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensaje de error: error de autenticación de SAML 2.0: no se encontró el identificador de usuario'
description: Cuando se utiliza SAML 2.0, el error "No se encontró el identificador de usuario con error de autenticación SAML 2.0" significa que no se pasa un ID UID o NAME desde las reglas de notificación de ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 15%

---

# Mensaje de error: Error de autenticación de SAML 2.0: Identificador de usuario no encontrado

## Problema

Recibo este error al usar SAML 2.0: &quot;Error de autenticación de SAML 2.0: no se encontró el identificador de usuario&quot;.

## Causa

Esto sucede cuando no se pasa un **UID** o **ID. DE NOMBRE** desde las **reglas de notificación de ADFS**.

En ADFS, la **confianza de usuario de confianza** necesita tener una **regla de reclamación** que pase un **UID** o un valor de **NAME ID**. Cuando ejecuta una conexión de prueba **[!DNL Workfront]**, debería mostrarla si se realiza correctamente.

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

1. Al editar la **[!UICONTROL INFORMACIÓN ADFS]**, en **[!UICONTROL Confianzas de usuario de confianza]** > Seleccionar objeto >**[!UICONTROL Editar reglas de notificación]**.

1. El **[!UICONTROL atributo LDAP]** (columna izquierda) debe tener **[!UICONTROL direcciones de correo electrónico]** (o cualquier identificador único).

1. El **[!UICONTROL tipo de notificación saliente]** (columna derecha) debe ser **[!UICONTROL identificador de nombre]**.

   >[!NOTE]
   >
   >No tiene que tener las direcciones de correo electrónico de atributos LDAP. Se puede usar cualquier identificador único que identifique al usuario, pero debe pasarse a [!DNL Adobe Workfront] como **NAME ID**.

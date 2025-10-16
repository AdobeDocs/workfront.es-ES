---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Falta tipo de licencia de usuario externo en los niveles de acceso
description: Ya no puedo ver el tipo de licencia de usuario externo en Niveles de acceso en la configuración.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 92%

---

# Falta el tipo de licencia de usuario externo en los niveles de acceso

## Problema

Ya no puedo ver el tipo de licencia de usuario externo en Niveles de acceso en la configuración.

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

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Sistema]** > **[!UICONTROL Preferencias]**.

1. En la sección **[!UICONTROL Seguridad]**, asegúrese de que la opción **[!UICONTROL Colaborar con personas sin cuentas de Workfront usando su dirección de correo electrónico]** esté habilitada.

   Si esta opción no está habilitada, el usuario externo no aparecerá en Configuración de nivel de acceso.

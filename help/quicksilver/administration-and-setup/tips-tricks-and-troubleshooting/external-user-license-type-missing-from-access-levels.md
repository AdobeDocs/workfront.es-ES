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
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 1%

---

# Falta el tipo de licencia de usuario externo en los niveles de acceso

## Problema

Ya no puedo ver el tipo de licencia de usuario externo en Niveles de acceso en la configuración.

## Requisitos de acceso

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
   <td>[!UICONTROL Administrador del sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Sistema]** > **[!UICONTROL Preferencias]**.

1. En la sección **[!UICONTROL Seguridad]**, asegúrate de que la opción **[!UICONTROL Colaborar con personas sin cuentas de Workfront usando su dirección de correo electrónico]** esté habilitada.

   Si esta opción no está habilitada, el usuario externo no aparece en Configuración de nivel de acceso.

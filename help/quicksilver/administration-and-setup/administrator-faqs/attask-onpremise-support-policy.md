---
title: Política de soporte OnPremise de AtTask
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: Adobe Workfront cambió a un modelo de 100% de Software-As-A-Service y dejó de vender software local el 31 de diciembre de 2011. A partir de 2014, AtTask OnPremise ya no es compatible, con la excepción de problemas relacionados con claves de licencia. La aplicación local ya no está disponible para descargar o instalar.
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Política de soporte OnPremise de AtTask

Adobe Workfront cambió a un modelo de 100% de Software-As-A-Service y dejó de vender software local el 31 de diciembre de 2011. A partir de 2014, AtTask OnPremise ya no es compatible, con la excepción de problemas relacionados con claves de licencia. La aplicación local ya no está disponible para descargar o instalar.

Si ya tiene la aplicación y necesita volver a instalar OnPremise, descargue la guía de instalación .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

Descargue instrucciones sobre la configuración SSL/TSL.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizar la clave de licencia On-Premise

Si necesita una nueva clave de licencia, llame al Servicio de atención al cliente de Workfront al 844-306-HELP(4357).

Una vez que haya obtenido una nueva clave de licencia,

1. Detenga el servidor atTask.
1. Cambie el nombre del archivo license.key actual (ubicado en la carpeta AtTaskDoc).
1. Copie el nuevo archivo license.key en su lugar.
1. Reinicie atTask Server.

Este artículo incluye los siguientes archivos adjuntos:

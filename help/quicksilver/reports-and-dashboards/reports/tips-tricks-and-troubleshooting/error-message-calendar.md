---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Mensaje de error en el calendario: "Este calendario tiene los derechos de visualización de un usuario desactivado".'
description: Obtenga información acerca del mensaje de error “Este calendario tiene los derechos de visualización de un usuario desactivado”.
author: Courtney
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/3yxFjvj--T8taJ2xrLTIia6YamTCwZeueTFSI-bMg4o
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 94%

---

# Mensaje de error en el calendario: “Este calendario tiene los derechos de visualización de un usuario desactivado”.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
     <p>Estándar</p>
     <p>Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles de control y calendarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en un calendario</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problema

Recibe el siguiente error al acceder a un calendario compartido con usted: 

*Este calendario tiene los derechos de visualización de un usuario desactivado. Pida a un administrador que corrija los privilegios del calendario.*

## Causa

El usuario que ha creado este calendario (su propietario original) es un usuario que se ha desactivado. 

## Solución

Puede resolver esto de la siguiente manera:

1. Copie el calendario original. Cuando copia un calendario, se convierte en su propietario. El calendario copiado debe mostrar toda la información del calendario original.\
   Para obtener más información sobre cómo copiar un calendario, consulte [Copiar un informe de calendario](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Comparta el calendario copiado con los mismos usuarios que el calendario original. Todos los usuarios deben ver la misma información en el nuevo calendario.
1. (Opcional y condicional) Si tiene permisos para administrar el calendario original, quite todos los demás usuarios con los que se comparta el calendario del área de uso compartido del calendario. Esto elimina la confusión de los usuarios que intentan mostrar el calendario incorrecto.

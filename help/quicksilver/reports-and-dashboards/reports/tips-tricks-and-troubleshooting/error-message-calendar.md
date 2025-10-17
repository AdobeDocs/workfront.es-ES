---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Mensaje de error en el calendario: "Este calendario tiene los derechos de visualización de un usuario desactivado".'
description: Obtenga información acerca del mensaje de error “Este calendario tiene los derechos de visualización de un usuario desactivado”.
author: Jenny
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 93%

---

# Mensaje de error en el calendario: “Este calendario tiene los derechos de visualización de un usuario desactivado”.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
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

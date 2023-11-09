---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Mensaje de error en el calendario: ''Este calendario tiene los derechos de visualización de un usuario desactivado''".'
description: Obtenga información acerca del mensaje de error "Este calendario tiene los derechos de visualización de un usuario desactivado".
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 5%

---

# Mensaje de error en el calendario: &quot;Este calendario tiene los derechos de visualización de un usuario desactivado&quot;.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, Trabajo</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en un calendario</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

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

---
title: Completar automáticamente una solicitud con datos de solicitudes anteriores
content-type: reference
description: Puede utilizar IA para completar automáticamente los campos de solicitud utilizando datos de solicitudes anteriores.
author: Alina
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EJR8tFVdc-sYRL5kXf-Ex9WExL0hcbkhQ1ZwEmpmU-s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 314
ht-degree: 23%

---

# Completar automáticamente una solicitud con datos de solicitudes anteriores

AI puede ayudarle a completar automáticamente los campos de solicitud en función de solicitudes anteriores. Puede aprobar o rechazar estas sugerencias antes de enviar la solicitud.

El completado automático no sobrescribe los campos que ya haya rellenado.

Los usuarios no reciben sugerencias de datos a los que no tienen acceso de otro modo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p>  </td> 
  </tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Acceso para añadir solicitudes a una cola de solicitudes</p> <p>Ver permisos superiores en la solicitud existente</p> <p>Para obtener información sobre cómo configurar una cola de solicitudes, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Obtener sugerencias al rellenar el formulario

El completado automático puede sugerir valores de campo mientras rellena el formulario. A medida que introduce valores en los campos de solicitud, Workfront compara esos valores con las solicitudes anteriores. Si el valor introducido se correlaciona estrechamente con otros valores de campo en contextos similares en solicitudes anteriores, Workfront sugiere esos valores.

Por ejemplo, si una clínica siempre utiliza el mismo código de facturación, Workfront sugeriría ese código de facturación en el campo apropiado cuando se introduzca el nombre de la clínica.

Para utilizar sugerencias basadas en solicitudes anteriores:

1. Comience a crear una solicitud.

   Para obtener instrucciones, consulte [Crear y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Empiece a rellenar los campos.

   A medida que rellena los campos, otros campos pueden mostrar sugerencias.

1. Para cada sugerencia de campo, seleccione **Aceptar** o **Rechazar** para ese campo.

   ![Aceptar o rechazar sugerencia](assets/accept-reject-suggestion.png)

   O

   Seleccione **Aceptar todo** o **Rechazar todo** en la parte superior de la página para aceptar o rechazar todas las sugerencias.

   >[!NOTE]
   >
   >Las sugerencias que no se hayan revisado se aceptarán automáticamente cuando envíe la solicitud.

---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Usar el informe de aprobación de revisión
description: Puede utilizar el informe de aprobación de revisión para ver información sobre las pruebas en su entorno.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
TQID: https://experienceleague.adobe.com/ZU6Ej5QhI7v9zoAxurBz1YsFVIuVIh2a8tR2h6vYL18
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 96%

---

# Usar el informe de aprobación de revisión

Puede utilizar el informe de aprobación de revisión para ver información sobre las pruebas en su entorno.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>paquete de Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licencia de Adobe Workfront</p> </td> 
   <td> 
   <p>Estándar</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configuración del nivel de acceso</strong> </td> 
   <td> <p>Acceso de edición a:</p> 
    <ul> 
     <li> <p>Creación de informes, paneles de control y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usar el informe de aprobación de revisión

{{step1-to-reports}}

1. Haga clic en **Nuevo informe** y desplácese hasta seleccionar **Aprobación de revisión**.

   ![Informe de aprobación de revisión](assets/proof-approval-report.png)

1. (Opcional) Añada cualquier campo adicional.
1. Haga clic en **Guardar + Cerrar**.

## Campos adicionales

Puede añadir los siguientes campos al informe de aprobación de revisión:

* **Fecha de decisión**: muestra la fecha en la que un aprobador toma una decisión sobre una prueba. También puede encontrar esta fecha en el Resumen de impresión de la prueba.
* **Fase de aprobación**: muestra la información de la fase actual.
* **Plantilla de flujo de trabajo**: muestra todas las plantillas de flujo de trabajo adjuntas a la prueba. Si no hay ninguna plantilla adjunta, la columna está en blanco.
* **Esperando decisión**: muestra true para indicar que no se ha cumplido una decisión en la última versión cuando se cumplen los siguientes criterios:

   * No se ha archivado la prueba
   * La fase en la que se encuentra el aprobador está activa
   * La prueba está pendiente de aprobación

* **Fecha límite de la revisión**: muestra la fecha límite de la revisión. Cada etapa debe tener una fecha límite asignada para que se rellene este campo. El campo muestra la fecha límite de la etapa activada más recientemente.

 

---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Usar el informe de aprobación de revisión
description: Puede utilizar el informe de aprobación de revisión para ver información sobre las pruebas en su entorno.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 98%

---

# Usar el informe de aprobación de revisión

Puede utilizar el informe de aprobación de revisión para ver información sobre las pruebas en su entorno.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Plan de Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Información general* sobre licencias de Adobe Workfront</p> </td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Nivel de acceso*</strong> </td> 
   <td> <p>Acceso de edición a:</p> 
    <ul> 
     <li> <p>Creación de informes, paneles de control y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

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

 

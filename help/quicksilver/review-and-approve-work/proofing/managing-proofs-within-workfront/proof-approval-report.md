---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Uso del informe de aprobación de pruebas
description: Puede utilizar el informe de aprobación de pruebas para ver información sobre pruebas en su entorno.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Uso del informe de aprobación de pruebas

Puede utilizar el informe de aprobación de pruebas para ver información sobre pruebas en su entorno.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>plan de Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Información general sobre las licencias de Adobe Workfront*</p> </td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Nivel de acceso*</strong> </td> 
   <td> <p>Editar acceso a:</p> 
    <ul> 
     <li> <p>Creación de informes, tableros y calendarios</p> </li> 
     <li> <p>Crear filtros, vistas y grupos</p> </li> 
    </ul> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Uso del informe de aprobación de pruebas

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, desplácese hasta seleccionar **Aprobación de prueba**.

   ![](assets/proof-approval-report.png)

1. (Opcional) Añada cualquier campo adicional.
1. Haga clic en **Guardar + Cerrar**.

## Campos adicionales

Puede añadir los siguientes campos al informe de aprobación de prueba:

* **Fecha de decisión**: Muestra la fecha en la que un aprobador toma una decisión sobre una prueba. También puede encontrar esta fecha en el resumen de impresión de la prueba.
* **Fase de aprobador**: Muestra la información del escenario actual.
* **Plantilla de flujo de trabajo**: Muestra las plantillas de flujo de trabajo adjuntas a la prueba. Si no hay ninguna plantilla adjunta, la columna está en blanco.
* **Pendiente de decisión**: Muestra true para indicar que no se ha cumplido una decisión en la versión más reciente cuando se cumpla lo siguiente:

   * La prueba no se ha archivado
   * El escenario en el que se encuentra el aprobador está activo
   * La prueba está pendiente de aprobación

* **Plazo de prueba**: Muestra la fecha límite de la prueba. Cada etapa debe tener una fecha límite asignada para que este campo se rellene. El campo muestra la fecha límite para la etapa activada más recientemente.

 

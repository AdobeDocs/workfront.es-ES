---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtro: Informe de aprobación de prueba para omitir versiones de prueba anteriores'
description: En un informe de aprobación de prueba, puede utilizar el filtro Es la versión actual del documento para incluir solo las versiones actuales de pruebas que esperan su aprobación.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Filtro: informe de aprobación de prueba para omitir versiones de prueba anteriores

En un informe de aprobación de prueba, puede usar la variable **Es la versión del documento actual** para incluir solo las versiones actuales de las pruebas que esperan su aprobación.

Esto resulta útil, por ejemplo, si se le ha solicitado que apruebe pruebas que tengan varias versiones. Cuando se ejecuta el informe Proof Approval con el filtro Is Current Document Version , el informe solo enumera la versión actual de cada prueba en espera de su aprobación, omitiendo las versiones anteriores en las que ya no necesita trabajar. 

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Filtrar el informe de aprobación de prueba para omitir las versiones de prueba anteriores

1. Si ya tiene un informe de aprobación de prueba, ábralo.

   O

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Para crear su propio informe de aprobación de pruebas, haga clic en el menú principal ![](assets/main-menu-icon.png)y haga clic en **Informes** ![](assets/reports-in-main-menu.png). Haga clic en **Nuevo informe**. En la lista que aparece, desplácese hasta y haga clic en **Aprobación de prueba**. Haga clic en **Guardar + Cerrar**, escriba a **Nombre del informe** (opcional) y haga clic en **Guardar informe**.

1. Haga clic en **Acciones de informe > Editar**.
1. Haga clic en **Filtros** y haga clic en **Agregar una regla de filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Haga clic en **Aprobación de prueba**.
1. En la lista que aparece, haga clic en **Es la versión del documento actual**.
1. Haga clic en **Guardar + Cerrar** en la esquina inferior izquierda de Adobe Workfront, haga clic en **Guardar informe** en el cuadro que aparece.

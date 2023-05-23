---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Filtro: informe de aprobación de pruebas para omitir versiones de prueba anteriores"
description: En un informe de Aprobación de pruebas, puede usar el filtro Es la versión actual del documento para incluir solamente las versiones actuales de las pruebas que esperan su aprobación.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Filtro: informe de aprobación de pruebas para omitir las versiones de prueba anteriores

En un informe de Aprobación de pruebas, puede usar el **Es la versión actual del documento** filtre para incluir solo las versiones actuales de las pruebas que esperan su aprobación.

Esto resulta útil, por ejemplo, si se le ha pedido que apruebe pruebas que tienen varias versiones. Cuando se ejecuta el informe de aprobación de pruebas con el filtro Es la versión actual del documento, el informe muestra solamente la versión actual de cada prueba en espera de aprobación, omitiendo las versiones anteriores en las que ya no necesita trabajar. 

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar un filtro </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Filtre el informe de aprobación de pruebas para omitir las versiones de prueba anteriores

1. Si ya tiene un informe de Aprobación de pruebas, ábralo.

   O

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Para crear su propio informe de Aprobación de pruebas, haga clic en el menú principal ![](assets/main-menu-icon.png), luego haga clic en **Informes** ![](assets/reports-in-main-menu.png). Clic **Nuevo informe**. En la lista que aparece, desplácese hasta y haga clic en **Aprobación de revisión**. Clic **Guardar + Cerrar**, escriba a **Nombre del informe** (opcional) y haga clic en **Guardar informe**.

1. Clic **Acciones de informe > Editar**.
1. Clic **Filtros**, luego haga clic en **Agregar una regla de filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Clic **Aprobación de revisión**.
1. En la lista que aparece, haga clic en **Es la versión actual del documento**.
1. Clic **Guardar + Cerrar** en la esquina inferior izquierda de Adobe Workfront, haga clic en **Guardar informe** en el cuadro que aparece.

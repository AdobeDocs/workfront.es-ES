---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copiar un tablero
description: Es posible copiar un tablero y todo su contenido (informes, calendarios y páginas externas). Al copiar el contenido de un tablero, es posible conservarlo tal y como aparece en el tablero original o crear elementos nuevos que sean copias de los que aparezcan en el tablero original. También es posible optar por no transferir ni copiar elementos en el nuevo tablero.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 98%

---

# Copiar un tablero

<!-- Audited: 1/2025 -->

Es posible copiar un tablero y todo su contenido (informes, calendarios y páginas externas). Al copiar el contenido de un tablero, es posible conservarlo tal y como aparece en el tablero original o crear elementos nuevos que sean copias de los que aparezcan en el tablero original. También es posible optar por no transferir ni copiar elementos en el nuevo tablero.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
    <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Estándar</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar el acceso a Informes, Paneles y Calendarios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver el acceso a un tablero</p> <p>Obtendrá acceso de administración al panel copiado</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Es necesario crear un tablero para poder copiarlo.

Para obtener información sobre cómo crear tableros, consulte [Creación de tableros](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copiar un tablero

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Paneles]**.

1. Seleccione el tablero que quiera copiar y luego haga clic en **Copiar** ![Icono de copiar](assets/copy-icon.png).\
   O\
   Abra el tablero que quiera copiar y, a continuación, haga clic en **Acciones de tablero** > **Copiar**.\
   Se mostrará el cuadro de diálogo Copia de tablero. Se mostrarán todos los elementos del tablero original.

1. En el campo **Nombre del tablero**, especifique un nombre nuevo para el tablero.
1. Para seleccionar todos los elementos del tablero existente y copiarlos en el tablero copiado, deje seleccionado **Seleccionar todo**. De forma predeterminada, los informes, calendarios o listas del tablero existente se copiarán en el tablero nuevo.\
   O\
   Para transferir solamente elementos específicos del tablero original al nuevo, anule la selección de aquellos elementos que no quiera que aparezcan en el tablero nuevo y, a continuación, elija entre las siguientes opciones para cada elemento seleccionado:

   * **Hacer una copia:** El elemento se copia desde el tablero original y se muestra una nueva versión de ese elemento en el tablero nuevo. Los cambios realizados en el elemento del nuevo tablero no se reflejan en el elemento del tablero original. Del mismo modo, los cambios realizados en el elemento del tablero original no se reflejarán en el elemento del nuevo tablero.\
     Use esta opción cuando quiera modificar el informe original del tablero original.\
     Por ejemplo: se copia un tablero llamado “Equipo B” y se le cambia el nombre a “Equipo A”. En el tablero “Equipo B” hay un informe llamado “Informe del equipo B”. Como este informe contiene datos específicos del Equipo B, selecciona la opción para realizar una copia de este informe, de modo que pueda personalizarlo para el Equipo A y cambiarle el nombre más adelante a “Informe del Equipo A”.\
     Con esta opción, se quitan los permisos de uso compartido del informe original del informe copiado. La opción Ejecutar este informe con los derechos de acceso a la información permanecerá intacta en el informe copiado.

   * **Usar original:** Muestra el elemento original en el nuevo tablero. Los cambios realizados en el elemento del nuevo tablero también se reflejarán en el elemento del tablero original. Del mismo modo, los cambios realizados en el elemento del tablero original se reflejarán en el elemento del nuevo tablero.\
     Con esta opción, se conservarán los permisos de uso compartido del informe original. La opción Ejecutar este informe con los derechos de acceso a la información también permanecerá intacta.

1. (Opcional) Cambie el nombre de los elementos que haya seleccionado.
1. Haga clic en **Copiar tablero**.
1. (Opcional) Si quisiera editar cualquiera de los informes, calendarios o páginas externas copiados en el tablero copiado, realice una de las siguientes acciones:

   * Para editar la información de cualquiera de los informes copiados, haga clic en el nombre del informe en el tablero y, a continuación, en **Acciones de informe** > **Editar**.

     Por ejemplo, es posible que quiera editar la vista, el filtro, la agrupación, la indicación, el gráfico o un informe copiado.

   * Para restablecer los permisos de los informes copiados, haga clic en el nombre del informe en el nuevo tablero y, a continuación, haga clic en **Acciones de informe** > **Uso compartido** y actualice los permisos del informe.

     Cuando se copie un informe mientras se copia un tablero, los permisos de ese informe se eliminarán.

   * Para modificar Ejecutar este informe con los derechos de acceso a la información, haga clic en el nombre del informe en el nuevo tablero y, a continuación, en **Acciones de informe** > **Editar** > **Opciones de informe**.\
     Después de copiar un informe, los permisos de Ejecutar este informe con los derechos de acceso de solo se mantendrán en las siguientes circunstancias:

     (Si ninguna de estas condiciones fuese verdadera, se quitarán los permisos Ejecutar este informe con los derechos de acceso de y la nueva opción Ejecutar este informe con los derechos de acceso de se cambiará para el usuario que creó el informe copiado).

     Si el usuario que copia el tablero y sus informes tiene derechos de acceso de administrador.

      * Si el usuario que copia el tablero y sus informes tiene derechos de acceso de administrador.
      * Si el usuario que copia el tablero y sus informes está configurado actualmente como Ejecutar este informe con los derechos de acceso de para los informes que se copian.
      * Si el usuario que copia el informe tiene permisos de administración sobre el informe.

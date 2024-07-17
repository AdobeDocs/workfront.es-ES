---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copiar un tablero
description: Puede copiar un tablero y todo su contenido (informes, calendarios y páginas externas). Al copiar el contenido de un tablero, puede elegir conservarlo tal y como aparece en el tablero original o crear elementos nuevos que sean copias de los que aparecen en el tablero original. También puede optar por no transferir ni copiar elementos en el nuevo tablero.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Copiar un tablero

Puede copiar un tablero y todo su contenido (informes, calendarios y páginas externas). Al copiar el contenido de un tablero, puede elegir conservarlo tal y como aparece en el tablero original o crear elementos nuevos que sean copias de los que aparecen en el tablero original. También puede optar por no transferir ni copiar elementos en el nuevo tablero.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar el acceso a Informes, Paneles y Calendarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver el acceso a un panel</p> <p>Obtendrá acceso de administración al panel copiado</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisitos previos

Debe crear un tablero para poder copiarlo.

Para obtener información sobre cómo crear paneles, consulte [Crear un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copiar un tablero

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) y luego haga clic en **Paneles**.

1. Seleccione el tablero que desee copiar y luego haga clic en **Copiar** ![](assets/copy-icon.png).\
   O\
   Abra el tablero que desee copiar y, a continuación, haga clic en **Acciones de tablero** > **Copiar**.\
   Aparece el cuadro de diálogo Copia de panel. Se mostrarán todos los elementos del tablero original.

1. En el campo **Nombre del panel**, especifique un nombre nuevo para el panel.
1. Para seleccionar todos los elementos en el tablero existente y copiarlos en el tablero copiado, deje seleccionado **Seleccionar todo**. De forma predeterminada, los informes, calendarios o listas del tablero existente se copiarán en el tablero nuevo.\
   O\
   Para transferir sólo elementos específicos del tablero original al nuevo, anule la selección de los elementos que no desee que aparezcan en el tablero nuevo y, a continuación, elija una de las siguientes opciones para cada elemento seleccionado:

   * **Hacer una copia:** El elemento se copia desde el tablero original y se muestra una nueva versión de ese elemento en el tablero nuevo. Los cambios realizados en el elemento en el nuevo panel no se reflejan en el elemento en el panel original. Del mismo modo, los cambios realizados en el elemento en el panel original no se reflejarán en el elemento en el nuevo panel.\
     Utilice esta opción cuando desee modificar el informe original en el tablero original.\
     Por ejemplo, se copia un tablero llamado &quot;Equipo B&quot; y se le cambia el nombre a &quot;Equipo A&quot;. En el tablero &quot;Equipo B&quot; hay un informe llamado &quot;Informe de equipo B&quot;. Dado que este informe contiene datos específicos del Equipo B, seleccione la opción para realizar una copia de este informe de modo que pueda personalizarlo para el Equipo A y cambiarle el nombre más adelante a &quot;Informe del Equipo A&quot;.\
     Con esta opción, se eliminan los permisos de uso compartido del informe original del informe copiado. La opción Ejecutar este informe con los derechos de acceso a la información permanece intacta en el informe copiado.

   * **Usar original:** Muestra el elemento original en el nuevo tablero. Los cambios realizados en el elemento en el nuevo tablero también se reflejan en el elemento en el tablero original. Del mismo modo, los cambios realizados en el elemento en el panel original se reflejarán en el elemento en el nuevo panel.\
     Con esta opción, se conservan los permisos de uso compartido del informe original. El informe Ejecutar este con los derechos de acceso a la información también permanece intacto.

1. (Opcional) Cambie el nombre de los elementos que haya seleccionado.
1. Haga clic en **Copiar tablero**.
1. (Opcional) Si desea editar cualquiera de los informes, calendarios o páginas externas copiados en el tablero copiado, realice una de las siguientes acciones:

   * Para editar la información de cualquiera de los informes copiados, haga clic en el nombre del informe en el panel y, a continuación, **Acciones de informe** > **Editar**.

     Por ejemplo, es posible que desee editar la vista, el filtro, la agrupación, el indicador o el gráfico o un informe copiado.

   * Para restablecer los permisos en los informes copiados, haga clic en el nombre del informe en el nuevo tablero y, a continuación, haga clic en **Acciones de informe** > **Compartir** y actualice los permisos en el informe.

     Cuando copia un informe mientras copia un tablero, los permisos de ese informe se eliminan.

   * Para modificar Ejecutar este informe con los derechos de acceso a la información, haga clic en el nombre del informe en el nuevo tablero y, a continuación, en **Acciones de informe** > **Editar** > **Opciones de informe**.\
     Después de copiar un informe, Ejecutar este informe con los derechos de acceso de los permisos de solo se mantienen en las siguientes circunstancias:

     (Si ninguna de estas condiciones es verdadera, se quita Ejecutar este informe con los derechos de acceso de los permisos y el nuevo Ejecutar este informe con los derechos de acceso de se cambia al usuario que creó el informe copiado).

     Si el usuario que copia el tablero y sus informes tiene derechos de acceso de administrador.

      * Si el usuario que copia el tablero y sus informes tiene derechos de acceso de administrador.
      * Si el usuario que copia el tablero y sus informes está configurado actualmente como Ejecutar este informe con los derechos de acceso de para los informes que se copian.
      * Si el usuario que copia el informe tiene permisos de administración en el informe.

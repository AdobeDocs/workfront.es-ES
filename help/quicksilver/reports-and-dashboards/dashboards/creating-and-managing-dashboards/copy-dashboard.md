---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copiar un tablero
description: Puede copiar un tablero y todo su contenido (informes, calendarios y páginas externas). Al copiar el contenido de un tablero, puede elegir mantenerlo tal como aparece en el tablero original o crear nuevos elementos que sean copias de los que aparecen en el tablero original. También puede optar por no transferir ni copiar elementos en el nuevo tablero.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Copiar un tablero

Puede copiar un tablero y todo su contenido (informes, calendarios y páginas externas). Al copiar el contenido de un tablero, puede elegir mantenerlo tal como aparece en el tablero original o crear nuevos elementos que sean copias de los que aparecen en el tablero original. También puede optar por no transferir ni copiar elementos en el nuevo tablero.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver acceso a un tablero</p> <p>Obtendrá acceso de administración al tablero copiado</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisitos previos

Debe crear un tablero antes de poder copiarlo.

Para obtener información sobre la creación de tableros, consulte [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copiar un tablero

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)y haga clic en **Tableros**.

1. Seleccione el tablero que desea copiar y, a continuación, haga clic en **Copiar** ![](assets/copy-icon.png).\
   O\
   Abra el tablero que desee copiar y, a continuación, haga clic en **Acciones del panel** > **Copiar**.\
   Aparece el cuadro de diálogo Copia de tablero . Se muestran todos los elementos del tablero original.

1. En el **Nombre del panel** , especifique un nuevo nombre para el tablero.
1. Para seleccionar todos los elementos del tablero existente y copiarlos en el tablero copiado, deje **Seleccionar todo** seleccionados. De forma predeterminada, los informes, calendarios o listas del tablero existente se copiarán en el nuevo tablero.\
   O\
   Para transferir solo elementos específicos del tablero original al nuevo, anule la selección de los elementos que no desea que aparezcan en el tablero nuevo y, a continuación, para cada elemento seleccionado, elija una de las siguientes opciones:

   * **Crear una copia:** El elemento se copia desde el tablero original y se muestra una nueva versión de ese elemento en el tablero nuevo. Los cambios realizados en el elemento del nuevo tablero no se reflejan en el elemento del tablero original. Del mismo modo, los cambios realizados en el elemento del tablero original no se reflejan en el elemento del tablero nuevo.\
      Utilice esta opción cuando desee modificar el informe original en el tablero original.\
      Por ejemplo, copiará un tablero llamado &quot;Equipo B&quot; y renómbralo como &quot;Equipo A&quot;. En el tablero &quot;Equipo B&quot; hay un informe llamado &quot;Informe Equipo B&quot;. Dado que este informe contiene datos específicos del Equipo B, puede seleccionar la opción de realizar una copia de este informe para que pueda personalizarlo para el Equipo A y cambiarle el nombre más adelante a &quot;Informe del Equipo A&quot;.\
      Con esta opción, se eliminan los permisos de uso compartido del informe original del informe copiado. Ejecutar este informe con los derechos de acceso de la información permanece intacto en el informe copiado.

   * **Usar original:** Muestra el elemento original en el nuevo tablero. Los cambios realizados en el elemento del nuevo tablero también se reflejan en el elemento del tablero original. Del mismo modo, los cambios realizados en el elemento del tablero original se reflejan en el elemento del tablero nuevo.\
      Con esta opción, se mantienen los permisos de uso compartido del informe original. Ejecute este informe con los derechos de acceso de la información también permanece intacto.

1. (Opcional) Cambie el nombre de los elementos que haya seleccionado.
1. Haga clic en **Copiar tablero**.
1. (Opcional) Si desea editar cualquiera de los informes, calendarios y páginas externas copiados en el tablero copiado, realice una de las siguientes acciones:

   * Para editar la información de cualquiera de los informes copiados, haga clic en el nombre del informe en el tablero y, a continuación, **Acciones de informe** > **Editar**.

      Por ejemplo, es posible que desee editar la vista, el filtro, la agrupación, el mensaje o el gráfico o un informe copiado.

   * Para restablecer los permisos en los informes copiados, haga clic en el nombre del informe en el nuevo tablero y, a continuación, haga clic en **Acciones de informe** > **Uso compartido** y actualizar los permisos del informe.

      Al copiar un informe mientras copia un tablero, se eliminan los permisos de ese informe.

   * Para modificar el informe Ejecutar este informe con los derechos de acceso de la información, haga clic en el nombre del informe en el nuevo tablero y, a continuación, **Acciones de informe** > **Editar** > **Opciones del informe**.\
      Después de copiar un informe, Ejecutar este informe con los derechos de acceso de los permisos solo se mantiene en las siguientes circunstancias:

      (Si ninguna de estas condiciones es verdadera, Ejecutar este informe con los derechos de acceso de los permisos se elimina y el nuevo Ejecutar este informe con los derechos de acceso de se cambia al usuario que creó el informe copiado).

      Si el usuario que copia el tablero y sus informes tiene derechos de acceso de administrador.

      * Si el usuario que copia el tablero y sus informes tiene derechos de acceso de administrador.
      * Si el usuario que copia el tablero y sus informes está configurado como Ejecutar este informe con los derechos de acceso de para los informes que se copian.
      * Si el usuario que copia el informe tiene permisos de administración en el informe.

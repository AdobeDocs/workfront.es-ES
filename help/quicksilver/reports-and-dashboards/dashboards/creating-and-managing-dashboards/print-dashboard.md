---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Imprimir un tablero
description: Puede imprimir o exportar un tablero a un archivo .PDF. Para imprimir un tablero, debe tener permiso para verlo.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: efae17458f2aa08ca2286ef5e43c68d1f9334b7b
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Imprimir un tablero

Puede imprimir o exportar un tablero a un archivo .PDF. Para imprimir un tablero, debe tener permiso para verlo.

>[!NOTE]
>
>Esta función solo se utiliza con la vista de panel estándar. No está disponible para los tableros que están incrustados en el área Proyectos ni configurados como fichas personalizadas.

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
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Ver acceso a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong>/td&gt; 
   <td> <p>Ver permisos del tablero</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

El tablero debe crearse para poder imprimirlo.

Para obtener información sobre la creación de tableros, consulte [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Comprender qué información se imprime al imprimir un tablero

Al imprimir un tablero o guardarlo como archivo .PDF, es posible que parte de la información del tablero, tal como aparece en la aplicación web de Adobe Workfront, no aparezca en el archivo impreso o exportado.

* [¿Qué se muestra?](#what-is-displayed)
* [¿Qué no se muestra?](#what-is-not-displayed)

### ¿Qué se muestra? {#what-is-displayed}

La siguiente información se incluye en el archivo de tablero impreso o exportado:

* Título del tablero
* Títulos de los informes
* Marca de tiempo de la última vez que se generó el informe
* Todos los objetos del tablero, incluidas las vistas de lista, las páginas web externas, los informes y los calendarios
* El logotipo de su empresa, si el administrador de Workfront lo ha personalizado en la barra de navegación global. Para obtener más información sobre la promoción de la marca en el sitio de Workfront, consulte [Marca la instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### ¿Qué no se muestra? {#what-is-not-displayed}

La siguiente información no está incluida en el archivo de tablero impreso o exportado:

* La barra de navegación de Workfront
* Cualquier otro formato específico de Workfront
* En función del tamaño de los informes y del número y la anchura de las columnas individuales, la exportación e impresión de un tablero puede causar que algunas columnas se corten.

## Imprimir un tablero

1. Vaya al tablero que desea imprimir.
1. Realice una de las siguientes acciones:

   * Haga clic en **Acciones del panel** > **Imprimir**

   * Press **Ctrl + P** (en Windows) o **Comando + P** (en Mac)

      >[!IMPORTANT]
      >
      >* Ninguna de estas opciones está disponible cuando el tablero está incrustado en una pestaña personalizada. Para obtener información sobre la creación de pestañas personalizadas, consulte [Crear fichas o secciones personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
      >* La opción de acceso directo del teclado no está disponible cuando se utiliza el explorador Internet Explorer.


1. En el **Destino** , seleccione entre las distintas opciones de impresión disponibles.\
   Las opciones de impresión varían según el explorador y la versión del explorador que utilice.

1. (Opcional) Guarde el tablero como archivo .PDF y, a continuación, haga clic en **Guardar** para guardar el .PDF.\
   Para obtener información sobre cómo guardar el tablero como un archivo .PDF, consulte [Exportación de un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Haga clic en **Imprimir**.

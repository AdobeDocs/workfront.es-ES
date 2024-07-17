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
>Esta función solo se puede utilizar con la vista de panel estándar. No está disponible para paneles que estén incrustados en el área de Proyectos o que se establezcan como fichas personalizadas.

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
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Ver acceso a informes, tableros y calendarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong>/td&gt; 
   <td> <p>Ver permisos en el tablero</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe crearse el tablero para poder imprimirlo.

Para obtener información sobre cómo crear paneles, consulte [Crear un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Comprender qué información se imprime al imprimir un tablero

Al imprimir un tablero o guardarlo como un archivo .PDF, es posible que parte de la información del tablero, tal como aparece en la aplicación web de Adobe Workfront, no aparezca en el archivo impreso o exportado.

* [¿Qué se muestra?](#what-is-displayed)
* [¿Qué no se muestra?](#what-is-not-displayed)

### ¿Qué se muestra? {#what-is-displayed}

En el archivo de tablero impreso o exportado se incluye la siguiente información:

* Título del panel
* Títulos del informe
* Marca de tiempo del último momento en el que se generó el informe
* Todos los objetos del tablero, incluidas las vistas de lista, las páginas web externas, los informes y los calendarios
* El logotipo de su empresa, si el administrador de Workfront lo ha personalizado en la barra de navegación global. Para obtener más información sobre cómo personalizar la marca del sitio de Workfront, consulte [Crear una marca para su instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### ¿Qué no se muestra? {#what-is-not-displayed}

La siguiente información no se incluye en el archivo de tablero impreso o exportado:

* La barra de navegación de Workfront
* Cualquier otro formato específico de Workfront
* Según el tamaño de los informes y el número y el ancho de las columnas individuales, la exportación e impresión de un tablero puede provocar que algunas columnas se corten.

## Imprimir un tablero

1. Vaya al tablero que desee imprimir.
1. Realice una de las acciones siguientes:

   * Haga clic en **Acciones de panel** > **Imprimir**

   * Presione **Ctrl+P** (en Windows) o **Comando+P** (en Mac)

     >[!IMPORTANT]
     >
     >* Ninguna de estas opciones está disponible cuando el panel está incrustado en una pestaña personalizada. Para obtener información acerca de cómo crear fichas personalizadas, vea [Crear fichas o secciones personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
     >* La opción de método abreviado de teclado no está disponible cuando se utiliza el explorador de Internet Explorer.

1. En el campo **Destino**, seleccione una de las diversas opciones de impresión disponibles.\
   Las opciones de impresión varían según la versión del explorador y del explorador que utilice.

1. (Opcional) Guarde el tablero como archivo .PDF y, a continuación, haga clic en **Guardar** para guardar el .PDF.\
   Para obtener información sobre cómo guardar el tablero como archivo .PDF, consulte [Exportar un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Haga clic en **Imprimir**.

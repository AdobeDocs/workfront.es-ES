---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Imprimir un panel de control
description: Puede imprimir o exportar un panel de control a un archivo PDF. Para imprimir un panel de control, debe tener permiso para verlo.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 98%

---

# Imprimir un panel de control

<!-- Audited: 1/2025 -->

Puede imprimir o exportar un panel de control a un archivo PDF. Para imprimir un panel de control, debe tener permiso para verlo.

>[!NOTE]
>
>Esta función solo se puede utilizar con la vista de panel de control estándar. No está disponible para paneles de control que estén incrustados en el área de Proyectos o que se establezcan como pestañas personalizadas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
      <p>Estándar</p>
      <p>Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización al panel de control</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe crearse previamente el panel de control para poder imprimirlo.

Para obtener información sobre cómo crear paneles de control, consulte [Crear un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Comprender qué información se imprime al imprimir un panel de control

Al imprimir un panel de control o guardarlo como un archivo PDF, es posible que parte de la información del panel de control, tal como aparece en la aplicación web de Adobe Workfront, no aparezca en el archivo impreso o exportado.

* [¿Qué se muestra?](#what-is-displayed)
* [¿Qué no se muestra?](#what-is-not-displayed)

### ¿Qué se muestra? {#what-is-displayed}

En el archivo del panel de control impreso o exportado se incluye la siguiente información:

* Título del panel de control
* Títulos del informe
* Marca de tiempo del último momento en el que se generó el informe
* Todos los objetos del panel de control, incluidas las vistas de lista, las páginas web externas, los informes y los calendarios
* El logotipo de su empresa, si su administrador de Workfront lo ha personalizado en la barra de navegación global. Para obtener más información sobre cómo personalizar la marca del sitio de Workfront, consulte [Marcar instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### ¿Qué no se muestra? {#what-is-not-displayed}

La siguiente información no se incluye en el archivo de panel de control impreso o exportado:

* La barra de navegación de Workfront
* Cualquier otro formato específico de Workfront
* Según el tamaño de los informes y el número y la anchura de las columnas individuales, la exportación e impresión de un panel de control puede provocar que algunas columnas se corten.

## Imprimir un panel de control

1. Vaya al panel de control que desee imprimir.
1. Realice una de las siguientes acciones:

   * Haga clic en **Acciones de panel** > **Vista preliminar**

   * Presione **Ctrl+P** (en Windows) o **Comando+P** (en Mac)

     >[!IMPORTANT]
     >
     >* Ninguna de estas opciones está disponible cuando el panel de control está incrustado en una pestaña personalizada. Para obtener información acerca de cómo crear pestañas personalizadas, consulte [Crear pestañas o secciones personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
     >* La opción de método abreviado de teclado no está disponible cuando se utiliza el explorador de Internet Explorer.

1. En el campo **Destino**, seleccione una de las diversas opciones de impresión disponibles.\
   Las opciones de impresión varían según la versión del explorador y del navegador que utilice.

1. (Opcional) Guarde el panel de control como archivo .PDF y, a continuación, haga clic en **Guardar** para guardar el PDF.\
   Para obtener información sobre cómo guardar el panel de control como archivo PDF, consulte [Exportar un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Haga clic en **Imprimir**.

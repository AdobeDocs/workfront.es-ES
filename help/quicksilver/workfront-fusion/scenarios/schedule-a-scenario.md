---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Programar un escenario en Adobe Workfront Fusion
description: De forma predeterminada, un escenario se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia se ejecuta un escenario activado.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Programar un escenario en [!DNL Adobe Workfront Fusion]

De forma predeterminada, un escenario se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia se ejecuta un escenario activado. Los escenarios de Fusion se pueden programar para que se ejecuten con tanta frecuencia como cada 5 minutos.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Programar un escenario

1. En la esquina superior derecha de la página de detalles del escenario, haga clic en **[!UICONTROL Opciones]** > **[!UICONTROL Programación]**

   O

   Haga clic en el icono **[!UICONTROL Programación]** (reloj) en el módulo de déclencheur del escenario.

1. Introduzca información en los campos siguientes:

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ejecutar escenario]</td> 
      <td> <p>Seleccione la frecuencia con la que desea ejecutar el escenario y, a continuación, seleccione el intervalo.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL A intervalos regulares]</strong> </p> <p>Introduzca el número de minutos entre ejecuciones. El valor predeterminado es 15 minutos.</p> </li> 
        <li> <p><strong>[!UICONTROL Una Vez]</strong> </p> <p>Escriba la fecha y la hora en que desea que se ejecute el escenario. Usar el formato <code>MM/DD/YYYY h:mm A</code>. Ejemplo: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Todos los días]</strong> </p> <p>Introduzca la hora a la que desea que se ejecute el escenario. Usar el formato <code>h:mm A</code>. Ejemplo: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Días de la semana]</strong> </p> <p>Días: seleccione los días de la semana en los que desea que se ejecute el escenario. Puede seleccionar uno o más días.</p> <p>Hora: introduzca la hora a la que desea que se ejecute el escenario en los días seleccionados. Usar el formato <code>h:mm A</code>. Ejemplo: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Días del mes]</strong> </p> <p>Días: seleccione los días del mes en que desea que se ejecute el escenario. Puede seleccionar uno o más días.</p> <p>Hora: introduzca la hora a la que desea que se ejecute el escenario en los días seleccionados. Usar el formato <code>h:mm A</code>. Ejemplo: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Fechas especificadas]</strong> </p> <p>Meses: seleccione los meses en los que desea ejecutar el escenario. Puede seleccionar uno o más meses.</p> <p>Días: seleccione los días del mes en que desea que se ejecute el escenario. Puede seleccionar uno o más días.</p> <p>Hora: introduzca la hora a la que desea que se ejecute el escenario en los días seleccionados. Usar el formato <code>h:mm A</code>. Ejemplo: <code>11:00 PM</code></p> </li> 
       </ul> <p>Nota: Debe existir una fecha para que un escenario se ejecute en esa fecha. Por ejemplo, un escenario programado solo para el 31 del mes no se ejecutará en febrero, abril, junio, septiembre o noviembre, porque esos meses no tienen un día 31.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Programación avanzada]</td> 
      <td>Puede definir intervalos de tiempo específicos durante los cuales se ejecutará el escenario. Puede especificar intervalos de hora del día, días laborables o meses. Para cada intervalo, haga clic en <strong>[!UICONTROL Agregar]</strong> y rellene los campos como se describe en el campo [!UICONTROL Ejecutar escenario].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Iniciar]</td> 
      <td>Escriba la fecha y la hora después de las cuales desea que se ejecute el escenario. Usar el formato <code>MM/DD/YYYY h:mm A</code>. Ejemplo: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Fin]</td> 
      <td>Escriba la fecha y la hora antes de las cuales desea que se ejecute el escenario. Usar el formato <code>MM/DD/YYYY h:mm A</code>. Ejemplo: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Aceptar]** para guardar la configuración de programación y volver al escenario.

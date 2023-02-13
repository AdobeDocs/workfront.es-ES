---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copiar módulos o escenarios en [!DNL Adobe Workfront Fusion]
description: Copiar módulos o escenarios en [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Copiar módulos o escenarios en [!DNL Adobe Workfront Fusion]

Puede copiar módulos, grupos de módulos o escenarios completos en [!DNL Adobe Workfront Fusion]. Esta capacidad le permite reutilizar escenarios o partes de escenarios sin tener que crearlos de nuevo

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr>
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Debe añadir módulos a un escenario para poder copiarlos.

## Copiar un módulo o un grupo de módulos

Al copiar un módulo, la copia conserva todos los valores de campo y la configuración del módulo original.

Puede pegar el módulo o los módulos en otra área del mismo escenario o en un escenario diferente.

Tenga en cuenta lo siguiente al pegar módulos en un escenario diferente.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Cualquier valor de campo que extraiga información de otro módulo que no haya copiado ya no podrá acceder a esa información. Debe configurar estos campos para extraer información del nuevo escenario.
* Si pega los módulos en un escenario propiedad de otro equipo u organización, todas las conexiones deben actualizarse a conexiones propiedad del grupo u organización propietario del nuevo escenario.

### Copiar módulos

Copiar un grupo de módulos es similar a copiar un solo módulo.

1. Haga clic con el botón derecho en el módulo que desee copiar.

   >[!NOTE]
   >
   >Para seleccionar más de un módulo, mantenga presionada la tecla [!UICONTROL shift] y haciendo clic en los módulos que desea copiar. Al copiar un grupo de módulos, también se copia cualquier línea de conexión, filtro o lógica de enrutamiento entre ellos.

1. Select **[!UICONTROL Módulo Copiar]**.
1. Mueva el cursor al área del escenario en el que desea la copia del escenario.
1. Haga clic con el botón derecho y seleccione **[!UICONTROL Pegar]**.
1. Para conectar los módulos pegados al escenario, arrástrelos a la ubicación adecuada del escenario.

   También puede utilizar métodos abreviados del teclado para copiar y pegar.

## Copiar un escenario mediante la clonación

Al clonar un escenario, se crea una copia del mismo, que luego se puede editar.

1. Abra la página de detalles del escenario:

   1. Haga clic en el **[!UICONTROL Situación]** en el panel izquierdo y, a continuación, haga clic en un escenario en el que desee obtener más información.

      O

      Si está trabajando en el escenario en la variable [El editor de escenarios de [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), haga clic en la flecha izquierda ![](assets/exit-editing-arrow.png) cerca de la esquina superior izquierda de la ventana.

1. Clic con el botón derecho **[!UICONTROL Opciones]** en la parte superior derecha de la página.
1. Select **[!UICONTROL Clonar]**.
1. (Opcional) Introduzca un nombre para el nuevo escenario.
1. (Opcional) Active **[!UICONTROL Mantenga los estados de cualquier módulo nuevo igual que los que se están duplicando]** para garantizar que el escenario copiado también incluya información sobre los registros más recientes procesados por el escenario original.
1. Haga clic en **[!UICONTROL Guardar]** para crear el escenario.

## Copiar un escenario utilizando modelos

Los modelos de escenario representan los valores de organización, asignación y campo de un escenario determinado en un momento dado. Puede exportar un modelo de escenario a un archivo JSON del equipo y luego importarlo al crear un nuevo escenario. Los escenarios importados desde un modelo de escenario se pueden editar.

Un modelo de escenario representa todo el escenario. Si desea copiar solo ciertos módulos de un escenario, consulte [Copiar un módulo o un grupo de módulos](#copy-a-module-or-a-group-of-modules) en este artículo.

>[!NOTE]
>
>Para obtener información sobre los modelos en el contexto de [!DNL Adobe Workfront], consulte [Información general sobre modelos](../../administration-and-setup/blueprints/blueprints-overview.md).

### Exportación de un modelo de escenario

1. En el escenario, haga clic en el botón **[!UICONTROL Más]** en el área de configuración del escenario.
1. Haga clic en **[!UICONTROL Modelo de exportación]**.

   Se crea un archivo JSON y se descarga a su equipo. Puede encontrar este archivo en su [!DNL Downloads] carpeta.

### Importar un modelo

>[!IMPORTANT]
>
>Si importa un modelo a un escenario existente, el modelo de escenario reemplaza al escenario existente. No se puede adjuntar un modelo a un escenario existente.

1. Empiece a crear un nuevo escenario.
1. En el escenario, haga clic en el botón **[!UICONTROL Más]** en el área de configuración del escenario.
1. Haga clic en **[!UICONTROL Modelo de importación]**.
1. En el cuadro de diálogo que aparece, haga clic en **[!UICONTROL Examinar]**
1. Vaya al modelo que desea importar y haga clic en **[!UICONTROL Apertura]**.
1. Haga clic en **[!UICONTROL Guardar]**.

   Se crea un archivo JSON y se descarga a su equipo. Puede encontrar este archivo en su [!UICONTROL Descargas] carpeta.

## Copiar y reutilizar escenarios mediante plantillas

Puede crear plantillas como punto de partida para su [!DNL Workfront Fusion] escenarios. Al crear un escenario a partir de una plantilla, puede modificarlo sin modificar la plantilla. Los valores de campo no se guardan en plantillas.

Para obtener más información sobre la creación y el uso de plantillas, consulte [Plantillas de escenario](../../workfront-fusion/scenarios/templates/fusion-templates.md).

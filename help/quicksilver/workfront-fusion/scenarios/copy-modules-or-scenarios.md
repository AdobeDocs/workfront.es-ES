---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copiar módulos o escenarios en  [!DNL Adobe Workfront Fusion]
description: Copiar módulos o escenarios en  [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# Copiar módulos o escenarios en [!DNL Adobe Workfront Fusion]

Puede copiar módulos, grupos de módulos o escenarios completos en [!DNL Adobe Workfront Fusion]. Esta capacidad le permite reutilizar escenarios o partes de escenarios sin tener que volver a crearlos

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
  </tr> 
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

## Requisitos previos

Debe agregar módulos a un escenario para poder copiarlos.

## Copiar un módulo o un grupo de módulos

Al copiar un módulo, la copia conserva todos los valores de campo y la configuración del módulo original.

Puede pegar el módulo o módulos en otra área del mismo escenario o en otro escenario diferente.

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
   >Para seleccionar más de un módulo, mantenga presionada la tecla [!UICONTROL mayús] y haga clic en los módulos que desee copiar. Al copiar un grupo de módulos también se copian las líneas de conexión, los filtros o la lógica de enrutamiento entre ellos.

1. Seleccione **[!UICONTROL Copiar módulo]**.
1. Mueva el cursor al área del escenario donde desee copiar el escenario.
1. Haga clic con el botón derecho y seleccione **[!UICONTROL Pegar]**.
1. Conecte los módulos pegados al escenario arrastrándolos a la ubicación adecuada en el escenario.

   También puede utilizar métodos abreviados del teclado para copiar y pegar.

## Copia de un escenario mediante clonación

Al clonar un escenario, se crea una copia del mismo que se puede editar a continuación.

1. Abra la página de detalles del escenario:

   1. Haga clic en la ficha **[!UICONTROL Escenario]** en el panel izquierdo y, a continuación, haga clic en un escenario sobre el que desee obtener detalles.

      O

      Si está trabajando en el escenario en [El editor de escenarios en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), haga clic en la flecha izquierda ![](assets/exit-editing-arrow.png) cerca de la esquina superior izquierda de la ventana.

1. Haga clic con el botón derecho en **[!UICONTROL Opciones]** en la parte superior derecha de la página.
1. Seleccionar **[!UICONTROL clonar]**.
1. (Opcional) Escriba un nombre para el nuevo escenario.
1. (Opcional) Habilite **[!UICONTROL Mantenga los estados de cualquier módulo nuevo igual que los que se están duplicando]** para asegurarse de que el escenario copiado también incluya información sobre los registros más recientes procesados por el escenario original.
1. Haga clic en **[!UICONTROL Guardar]** para crear el escenario.

## Copiar un escenario mediante modelos

Los modelos de escenario representan la organización, la asignación y los valores de campo de un escenario determinado en un momento determinado. Puede exportar un modelo de escenario a un archivo JSON de su equipo y, a continuación, importarlo al crear un nuevo escenario. Los escenarios importados de un modelo de escenario se pueden editar.

Un modelo de escenario representa todo el escenario. Si desea copiar solamente ciertos módulos de un escenario, consulte [Copiar un módulo o un grupo de módulos](#copy-a-module-or-a-group-of-modules) en este artículo.

>[!NOTE]
>
>Para obtener información acerca de los modelos en el contexto de [!DNL Adobe Workfront], vea [Información general sobre modelos](../../administration-and-setup/blueprints/blueprints-overview.md).

### Exportar un modelo de escenario

1. En el escenario, haga clic en el menú **[!UICONTROL Más]** del área de configuración del escenario.
1. Haga clic en **[!UICONTROL Exportar modelo]**.

   Se crea un archivo JSON y se descarga en el equipo. Puede ubicar este archivo en la carpeta [!DNL Downloads].

### Importar un modelo

>[!IMPORTANT]
>
>Si importa un modelo a un escenario existente, el modelo de escenario reemplazará al escenario existente. No se puede anexar un modelo a un escenario existente.

1. Empiece a crear un nuevo escenario.
1. En el escenario, haga clic en el menú **[!UICONTROL Más]** del área de configuración del escenario.
1. Haga clic en **[!UICONTROL Importar modelo]**.
1. En el diálogo que aparece, haga clic en **[!UICONTROL Examinar]**
1. Vaya al modelo que desee importar y haga clic en **[!UICONTROL Abrir]**.
1. Haga clic en **[!UICONTROL Guardar]**.

   Se crea un archivo JSON y se descarga en el equipo. Puedes encontrar este archivo en tu carpeta [!UICONTROL Descargas].

## Copiar y reutilizar escenarios mediante plantillas

Puede crear plantillas como punto de partida para sus [!DNL Workfront Fusion] escenarios. Cuando crea un escenario a partir de una plantilla, puede modificarlo sin modificarla. Los valores de campo no se guardan en las plantillas.

Para obtener más información sobre cómo crear y usar plantillas, consulte [Plantillas de escenarios](../../workfront-fusion/scenarios/templates/fusion-templates.md).

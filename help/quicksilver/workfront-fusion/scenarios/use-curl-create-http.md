---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Utilice cURL para agregar un módulo HTTP
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 31%

---

# Utilice cURL para agregar un módulo HTTP

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Use cURL para agregar un módulo HTTP](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/use-curl-create-http.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Puede pegar una solicitud cURL en su escenario y Fusion creará un módulo HTTP configurado a partir de la solicitud cURL.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Plan de Adobe Workfront</td>  
      <td>Cualquiera</td>  
    </tr>  
    <tr>  
      <td>Licencia de Adobe Workfront</td>  
      <td>
        Nuevo: Estándar<br>
        O<br>
        Actual: Trabajo o superior
      </td>  
    </tr>  
    <tr>  
      <td>Licencia de Adobe Workfront Fusion</td>  
      <td> 
        Actual: no se requiere licencia de Workfront Fusion.<br>
        O<br>
        Heredado: cualquiera
      </td>  
    </tr>  
    <tr>  
      <td>Producto</td>  
      <td> 
        Nuevo: Plan Select or Prime Workfront: su organización debe adquirir Adobe Workfront Fusion.<br>
        Plan Ultimate Workfront: Workfront Fusion está incluido.<br>
        O<br>
        Actual: su organización debe adquirir Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Creación de un módulo HTTP a partir de una solicitud cURL


Para crear un módulo HTTP mediante cURL:

1. Cree el texto de la solicitud cURL fuera de Fusion, como en un editor de texto.
1. Copie la solicitud cURL en el portapapeles.
1. Haga clic en la ficha **[!UICONTROL Escenario]** en el panel izquierdo.
1. Seleccione el escenario en el que desea crear el módulo.
1. Haga clic en cualquier lugar del escenario para introducir el Editor de escenarios.
1. Haga clic con el botón derecho en cualquier espacio en blanco del editor de escenarios y seleccione **Pegar**.

   O

   Presione Ctrl + V (Windows) o Cmd + V (Mac).


   Se crea un módulo de HTML.
1. Arrastre el módulo para conectarlo a su escenario.

## Resolución de problemas

Si la cURL no se pega en el escenario, compruebe la configuración del explorador para asegurarse de que está habilitado el pegado desde el portapapeles.



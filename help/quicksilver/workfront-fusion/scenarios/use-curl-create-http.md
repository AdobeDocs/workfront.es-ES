---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Utilice cURL para agregar un módulo HTTP
description: Puede pegar una solicitud cURL en su escenario y Fusion creará un módulo HTTP configurado a partir de la solicitud cURL.
author: Becky
feature: Workfront Fusion
source-git-commit: 4cc881f4f5a28bd105e6898ad7ffb57c1dafb563
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 33%

---

# Utilice cURL para agregar un módulo HTTP

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

   >[!IMPORTANT]
   >
   >Si utiliza Fusion en un equipo con Windows, la solicitud de cURL no debe incluir saltos de línea.
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

Si la cURL no se pega en el escenario, compruebe lo siguiente:

* Compruebe la configuración de su navegador para asegurarse de que está activado pegar desde el portapapeles.
* Si está ejecutando Windows, compruebe la solicitud cURL para asegurarse de que no incluye saltos de línea.




---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Cambiar la resolución de prueba interactiva en el visor de pruebas
description: Puede obtener una vista previa del aspecto de una prueba interactiva en varios dispositivos, lo que le permite ver cómo se muestra y responde el contenido en función de distintas resoluciones.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 1%

---

# Cambiar la resolución de prueba interactiva en el visor de pruebas

Puede obtener una vista previa del aspecto de una prueba interactiva en varios dispositivos, lo que le permite ver cómo se muestra y responde el contenido en función de distintas resoluciones.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Vistas de dispositivo y resolución en el visor de pruebas de escritorio frente al visor de pruebas web

El administrador de Adobe Workfront ha configurado el sistema para que pueda revisar el contenido interactivo en el Visor de pruebas de escritorio o, como contenido agrupado en un archivo ZIP, en el Visor de pruebas web:

* En el Visor de prueba de escritorio, puede ver cómo aparece y responde el contenido en varias resoluciones y en varios dispositivos. Cuando un revisor especifica un dispositivo determinado, el contenido aparece tal como aparecería en ese dispositivo, con las especificaciones de la interfaz de usuario del dispositivo. Por ejemplo, un botón rojo en una marca de smartphones puede ser azul en una marca diferente.

* En el visor de pruebas web, puede ver el contenido interactivo tal como aparece en las resoluciones de los distintos dispositivos. Sin embargo, el visor de prueba web no emula el contenido utilizando especificaciones de interfaz en estos dispositivos, como el color del botón.

   >[!NOTE]
   >
   >El administrador de Workfront puede configurar dispositivos personalizados para los usuarios de su organización, tal como se describe en Configuración de dispositivos personalizados para pruebas interactivas en el artículo .

## Ver una prueba con un dispositivo preestablecido o una configuración de resolución

1. Vaya a la lista de documentos que contiene la prueba que desea abrir.
1. Pase el ratón sobre el documento y haga clic en **Abrir prueba**.
1. Haga clic en **Interactivo** en la parte central inferior del visor de pruebas.

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. En el Visor de prueba de escritorio, en la lista de dispositivos y resoluciones que aparecen, haga clic en el que desee.

   O

   En el visor de pruebas web, en la lista de resoluciones que aparecen, haga clic en la que desee.

   Si necesita información sobre las diferencias entre estos dos visores, consulte [Diferencias entre el visor de pruebas web y el visor de pruebas de escritorio](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   La prueba interactiva se procesa en la resolución seleccionada.

## Ver una prueba con una configuración de resolución personalizada

1. Vaya a la lista de documentos que contiene la prueba que desea abrir.
1. Pase el ratón sobre el documento y haga clic en **Abrir prueba**.
1. Haga clic en **Interactivo** en la parte central inferior del visor de pruebas.
1. Escriba un **Interactivo** resolución.

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   O

   Pase el cursor sobre el contenido interactivo y arrastre el borde azul de la esquina inferior derecha, o el borde derecho o inferior, a la resolución que desee.

   ![Arrastrar_bordes_azules_para_resolución.png](assets/drag-blue-edges-for-resolution-350x251.png)

   La resolución personalizada se muestra en las siguientes ubicaciones:

   * En el **Resolución** en la parte inferior central del visualizador.\
      ![Captura de pantalla de 2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * En cualquier comentario, los revisores añaden a la prueba. Cada comentario incluye la resolución de pantalla que se seleccionó cuando el revisor creó el comentario.

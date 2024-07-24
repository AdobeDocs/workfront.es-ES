---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Cambiar la resolución de prueba interactiva en el visor de pruebas
description: Puede obtener una vista previa del aspecto de una prueba interactiva en varios dispositivos, lo que le permite ver cómo se muestra el contenido y cómo responde en función de diferentes resoluciones.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 1%

---

# Cambiar la resolución de prueba interactiva en el visor de pruebas

Puede obtener una vista previa del aspecto de una prueba interactiva en varios dispositivos, lo que le permite ver cómo se muestra el contenido y cómo responde en función de diferentes resoluciones.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Vistas de dispositivo y resolución en el Visor de pruebas de escritorio frente al Visor de pruebas web

El administrador de Adobe Workfront ha configurado el sistema para que revise el contenido interactivo en el Visor de pruebas de escritorio o, como contenido agrupado en un archivo ZIP, en el Visor de pruebas web:

* En el Visor de pruebas de escritorio, puede ver cómo aparece el contenido y cómo responde en varias resoluciones y en varios dispositivos. Cuando un revisor especifica un dispositivo determinado, el contenido aparece como lo haría en ese dispositivo, con las especificaciones de interfaz de usuario para el dispositivo. Por ejemplo, un botón rojo en una marca de smartphone puede ser azul en una marca diferente.

* En el Visor de revisión web, puede ver el contenido interactivo tal como aparece en las resoluciones de los distintos dispositivos. Sin embargo, el Visor de revisión web no emula el contenido mediante especificaciones de interfaz en estos dispositivos, como el color del botón.

  >[!NOTE]
  >
  >El administrador de Workfront puede configurar dispositivos personalizados para los usuarios de su organización, tal como se describe en [Configuración de dispositivos personalizados para pruebas](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#configure-custom-devices-for-proofs) en el artículo [Configuración de pruebas para su organización](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

## Visualización de una prueba con un dispositivo preestablecido o un ajuste de resolución

1. Vaya a la lista de documentos que contiene la prueba que desea abrir.
1. Pase el ratón sobre el documento y luego haga clic en **Abrir revisión**.
1. Haga clic en **Adaptable** en la parte inferior central del visor de revisión.

   ![Opción_de_resolución_en_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. En el Visor de corrección de escritorio, en la lista de dispositivos y resoluciones que aparece, haga clic en el que desee.

   O

   En el Visor de revisión Web, en la lista de resoluciones que aparece, haga clic en la que desee.

   Si necesita información sobre cómo difieren estos dos visores, vea [Diferencias entre el Visor de revisión web y la descripción general del Visor de revisión de escritorio](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   La prueba interactiva se procesa en la resolución que seleccione.

## Visualización de una prueba con una configuración de resolución personalizada

1. Vaya a la lista de documentos que contiene la prueba que desea abrir.
1. Pase el ratón sobre el documento y luego haga clic en **Abrir revisión**.
1. Haga clic en **Adaptable** en la parte inferior central del Visor de pruebas.
1. Escriba una resolución **adaptable** personalizada.

   ![Tipo_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   O

   Pase el ratón sobre el contenido interactivo y arrastre el borde azul de la esquina inferior derecha, o el borde derecho o inferior, a la resolución que desee.

   ![Arrastrar_bordes_azules_para_resolución.png](assets/drag-blue-edges-for-resolution-350x251.png)

   La resolución personalizada se muestra en las siguientes ubicaciones:

   * En el panel **Resolución** en la parte inferior central del visor.\
     ![Captura de pantalla_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * En cualquier comentario, los revisores añaden a la prueba. Cada comentario incluye la resolución de pantalla seleccionada cuando el revisor creó el comentario.

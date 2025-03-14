---
product-area: documents
navigation-topic: approvals
title: Cargar una nueva versión del documento y solicitar una aprobación
description: Puede cargar una nueva versión del documento y solicitar la aprobación de otros usuarios en Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 30%

---

# Cargar una nueva versión del documento y solicitar una aprobación

Si un documento está marcado necesita trabajar en una revisión anterior, puede cargar una nueva versión en el documento original e iniciar otra ronda de aprobaciones. Una vez cargada una nueva versión del documento, las versiones anteriores se bloquean.

Si el nombre de archivo de la nueva versión es diferente del nombre de archivo de la versión anterior, Workfront muestra el documento con el nombre de archivo más reciente.

Cuando se añade una nueva versión a un documento con aprobaciones pendientes, la aprobación de la versión anterior se muestra como Retirada. El proceso de aprobación previo se cierra, incluso si algunos participantes aún no han tomado una decisión.

Si se elimina la versión más reciente del documento, las versiones anteriores permanecerán bloqueadas. Si necesita editar una versión anterior, debe desbloquearla manualmente.


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Actual: solicitud o superior</p>
   o
   <p>Nuevo: colaborador o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso al objeto asociado con el documento</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Utilice arrastrar y soltar para agregar una nueva versión

>[!NOTE]
>
>Arrastrar y soltar no funciona con Internet Explorer.

1. Vaya al área Documentos donde se ha cargado el documento.
1. Desde el escritorio o desde una ficha de explorador independiente, arrastre la nueva versión del documento sobre la versión existente en Workfront.

   A medida que arrastra la nueva versión, puede situarse sobre una carpeta de documentos de Workfront para abrirla. A continuación, puede desplazarse hacia arriba y hacia abajo arrastrando los archivos a la parte superior o inferior de la pantalla.

1. Coloque la nueva versión sobre el archivo existente en la ficha **Documentos**.

1. Una vez cargado el documento, haga clic en él y abra el panel Resumen del documento.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del panel Resumen del documento y haga clic en **Añadir**.

![Agregar aprobadores en el resumen del documento](assets/doc-summary-add-approvers.png)

1. (Opcional) Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas antes y 24 horas antes del plazo especificado.

1. Para agregar rápidamente revisores y aprobadores de la versión anterior, haga clic en el botón Agregar situado junto a sus nombres en la lista siguiente.
   <!--need screenshot when working-->

1. (Opcional) Cambiar la función de aprobador/revisor.

1. Para agregar nuevos aprobadores y revisores, haga clic en **Revisor** o **Aprobador** y empiece a escribir el usuario o equipo.

   ![Agregar aprobador y fecha límite](assets/add-approver-and-deadline.png)

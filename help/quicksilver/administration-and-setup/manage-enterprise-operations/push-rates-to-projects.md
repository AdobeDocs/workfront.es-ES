---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Cambios de tasa push en proyectos
description: Una tarjeta de tarifas representa el acuerdo contractual con su cliente en el que se definen las tarifas por hora para los roles que completarán el trabajo. En una tarjeta de tarifas, puede definir varias tarifas de facturación por rol, según los atributos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
source-git-commit: 7686cd33a5c761dc57cb488ea49a4139665949d9
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 20%

---

# Cambios en la tasa push de los proyectos

Cuando se adjunta una tarjeta de tarifas a un proyecto <!--or a staffing plan-->, las tarifas de la tarjeta de tarifas aún se pueden ajustar. A continuación, si lo desea, puede insertar esas tasas en los proyectos a los que está adjunta la tarjeta de tasas. Si no inserta las nuevas tasas, las tasas originales permanecerán en el proyecto.
<!-- and staffing plans -->
<!-- or staffing plan -->

Para obtener información acerca de cómo adjuntar una tarjeta de tarifa a un proyecto, vea [Adjuntar una tarjeta de tarifa a un proyecto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Editar acceso a [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Para editar una tarjeta de tarifas compartida con usted, debe tener permisos de administración en la tarjeta de tarifas.</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cambios en la tasa push de los proyectos

{{step-1-to-setup}}

1. El panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Haga clic en el nombre de la tarjeta de tarifa en la lista Tarjetas de tarifa.
1. En la pantalla Tarjeta de tarifas > Funciones del puesto y tarifas, compruebe que las tarifas son correctas y edite las tarifas según sea necesario.
1. Haga clic en [!UICONTROL **Cambios push**].
1. En el cuadro de diálogo [!UICONTROL **Aplicar a todos los proyectos**], todos los proyectos que usan esta tarjeta de tarifa se seleccionan de manera predeterminada. Si no desea que un proyecto aplique los cambios de tasa, debe deseleccionarlo.

   <!--/staffing plans-->
   <!--and staffing plans -->
   <!--or staffing plan -->

1. Haga clic en [!UICONTROL **Guardar**].

   Las nuevas tarifas ahora se reflejan en los proyectos <!--and staffing plans --> que usan la tarjeta de tarifas.

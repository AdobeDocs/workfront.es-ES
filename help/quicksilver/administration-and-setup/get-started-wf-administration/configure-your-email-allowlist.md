---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar la lista de permitidos de correo electrónico
description: Si su organización utiliza el plan Workfront Enterprise, puede crear una lista de permitidos de correo electrónico de Workfront para controlar qué dominios de correo electrónico pueden aceptar correos electrónicos de Workfront y qué dominios de correo electrónico pueden estar en la dirección de correo electrónico que los usuarios especifiquen en su perfil de usuario. Esto resulta útil si la política de seguridad de su organización impide que los usuarios envíen datos almacenados en Workfront a direcciones de correo electrónico externas; puede incluir solo los dominios internos de la compañía en la lista de permitidos para asegurarse de que se sigue esta política.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 99%

---

# Configurar la lista de permitidos de correo electrónico

Si su organización utiliza el plan para empresas de Workfront, puede crear una lista de permitidos de correo electrónico de Workfront para controlar lo siguiente:

* Los dominios de correo electrónico que pueden aceptar correos electrónicos de Workfront.
* Los dominios de correo electrónico que pueden estar en la dirección de correo electrónico que los usuarios especifiquen en su perfil de usuario.

Esto resulta útil si la directiva de seguridad de su organización impide que los usuarios envíen datos almacenados en Workfront a direcciones de correo electrónico externas; puede incluir solo los dominios internos de la compañía en la lista de permitidos para asegurarse de que se sigue esta directiva.

>[!IMPORTANT]
>
>Su equipo de TI debe asegurarse de que el correo electrónico entrante de `notifications@my.workfront.com` no esté bloqueado en el sistema de su organización.
>
>Todo el correo electrónico de Workfront se envía desde esa dirección para aumentar el éxito de la entrega de correo electrónico y para eliminar la suplantación de correos electrónicos. Esto incluye tanto alertas automatizadas como la comunicación de usuario a usuario.
>
>Por ejemplo, la línea “De” en un correo electrónico de Workfront que recibe de un usuario llamado Joan Harris tendría este aspecto:
>>`Joan Harris <notifications@my.workfront.com>`

Para obtener información sobre la configuración del cortafuegos de su organización para abrir la comunicación entre su entorno y los servidores de Adobe Workfront, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Otras listas de permitidos

Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a determinados proveedores, debe añadir determinadas direcciones IP a su lista de permitidos. Se abre la comunicación entre su entorno y los servidores de Adobe Workfront. Para obtener información al respecto, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar la lista de permitidos de correo electrónico

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Información del cliente**.
1. En la sección **Lista de permitidos de correo electrónico**, seleccione **Habilitar lista de permitidos de dominio** y luego haga clic en **Añadir dominio**.
1. En el cuadro que se muestra, escriba un dominio que desea que se permita, como `ourcompany.com`, y haga clic en **Añadir dominio**.
1. Repita el paso anterior para añadir cualquier otro dominio que desee permitir.
1. Cuando termine, haga clic en **Guardar**.

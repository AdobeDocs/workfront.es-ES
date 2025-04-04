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
source-git-commit: 937965ad495453e185504d53f9d9c88c3cd7e201
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 100%

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
>`Joan Harris <notifications@my.workfront.com>`

Para obtener información sobre la configuración del cortafuegos de su organización para abrir la comunicación entre su entorno y los servidores de Adobe Workfront, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Otras listas de permitidos

Si su organización tiene el plan para empresas, puede configurar una lista de permitidos IP de Adobe Workfront que limite el acceso a Workfront a 75 direcciones IP o rangos de direcciones IP que especifique. Esto proporciona un nivel adicional de seguridad para la aplicación de Workfront. Para obtener más información, consulte [Restringir el acceso a Adobe Workfront por la dirección IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Además, si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a determinados proveedores, debe añadir determinadas direcciones IP a su lista de permitidos. Se abre la comunicación entre su entorno y los servidores de Adobe Workfront. Para obtener información al respecto, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar la lista de permitidos de correo electrónico

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Información del cliente**.
1. En la sección **Lista de permitidos de correo electrónico**, seleccione **Habilitar lista de permitidos de dominio** y luego haga clic en **Añadir dominio**.
1. En el cuadro que se muestra, escriba un dominio que desea que se permita, como `ourcompany.com`, y haga clic en **Añadir dominio**.
1. Repita el paso anterior para añadir cualquier otro dominio que desee permitir.
1. Cuando termine, haga clic en **Guardar**.

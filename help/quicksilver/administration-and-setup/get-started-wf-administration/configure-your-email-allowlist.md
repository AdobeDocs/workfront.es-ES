---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar la lista de permitidos de correo electrónico
description: Si su organización utiliza el plan WorkfrontEnterprise, puede crear una lista de permitidos de correo electrónico de Workfront para controlar qué dominios de correo electrónico pueden aceptar correos electrónicos de Workfront y qué dominios de correo electrónico pueden estar en la dirección de correo electrónico que especifican los usuarios en su perfil de usuario. Esto resulta útil si la política de seguridad de su organización restringe el envío de datos almacenados en Workfront a direcciones de correo electrónico externas; puede incluir solo los dominios de empresa internos en la lista de permitidos para garantizar que se sigue esta política.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Configurar la lista de permitidos de correo electrónico

Si su organización utiliza el plan WorkfrontEnterprise, puede crear una lista de permitidos de correo electrónico de Workfront para controlar:

* Qué dominios de correo electrónico pueden aceptar correos electrónicos de Workfront.
* Qué dominios de correo electrónico pueden estar en la dirección de correo electrónico que los usuarios especifican en su perfil de usuario.

Esto resulta útil si la política de seguridad de su organización restringe el envío de datos almacenados en Workfront a direcciones de correo electrónico externas; puede incluir solo los dominios de empresa internos en la lista de permitidos para garantizar que se sigue esta política.

>[!IMPORTANT]
>
>Su equipo de TI debe asegurarse de que el correo electrónico entrante `notifications@my.workfront.com` no está bloqueado en el sistema de su organización.
>
>Todo el correo electrónico de Workfront se envía desde esa dirección para aumentar el envío correcto de correos electrónicos y eliminar la suplantación de correos electrónicos. Esto incluye tanto alertas automatizadas como comunicación de usuario a usuario.
>
>Por ejemplo, la línea Desde de un correo electrónico de Workfront que recibe de un usuario llamado Joan Harris tendría este aspecto:
>
```
>Joan Harris <notifications@my.workfront.com>
>```

Para obtener información sobre la configuración del cortafuegos de su organización para abrir la comunicación entre su entorno y los servidores de Adobe Workfront, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Otras listas de permitidos

Si su organización tiene el plan Enterprise , puede configurar una lista de permitidos IP de Adobe Workfront que limite el acceso a Workfront a 45 direcciones IP o intervalos de direcciones IP que especifique. Esto proporciona una capa adicional de seguridad para la aplicación Workfront. Para obtener más información, consulte [Restringir el acceso a Adobe Workfront por dirección IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Además, si el servidor de seguridad o de correo está configurado para permitir el acceso solo a determinados proveedores, debe añadir ciertas direcciones IP a su lista de permitidos. Esto abre la comunicación entre su entorno y los servidores de Adobe Workfront. Para obtener información al respecto, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar la lista de permitidos de correo electrónico

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Información del cliente**.

1. En el **Lista de permitidos de correo electrónico** , seleccione **Habilitar Lista de permitidos de dominio** y haga clic en **Agregar dominio**.
1. En el cuadro que aparece, escriba un dominio que desee permitir, como `ourcompany.com`y haga clic en **Agregar dominio**.

1. Repita el paso anterior para agregar cualquier otro dominio que desee permitir.
1. Cuando haya terminado, haga clic en **Guardar**.

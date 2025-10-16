---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Impedir usuarios duplicados
description: Al crear un nuevo usuario en Adobe Workfront, ya no puede utilizar una dirección de correo electrónico que ya esté utilizando otro usuario, aunque la dirección de correo electrónico varíe según las mayúsculas y minúsculas (por ejemplo, JohnDoe@example.com y johndoe@example.com). Además, para prepararse para futuras mejoras de autenticación, asegúrese de que todos los usuarios tengan direcciones de correo electrónico únicas en una instancia de Workfront.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 7%

---

# Impedir usuarios duplicados

Al crear un nuevo usuario en Adobe Workfront, ya no puede utilizar una dirección de correo electrónico que ya esté utilizando otro usuario, aunque la dirección de correo electrónico varíe según las mayúsculas y minúsculas (por ejemplo, JohnDoe@example.com y johndoe@example.com). Además, para prepararse para futuras mejoras de autenticación, asegúrese de que todos los usuarios tengan direcciones de correo electrónico únicas en una instancia de Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear usuarios con direcciones de correo electrónico únicas

A partir de la versión 2019.4, al crear un nuevo usuario en Workfront, ya no puede utilizar una dirección de correo electrónico que ya esté siendo utilizada por otro usuario, aunque la dirección de correo electrónico varíe según el caso. Por ejemplo, no se puede crear un usuario con la dirección de correo electrónico JohnDoe@example.com si otro usuario tiene la dirección de correo electrónico johndoe@example.com.

## Actualizar las direcciones de correo electrónico de los usuarios existentes en la instancia de Workfront

Como administrador de Workfront, debe actualizar los usuarios existentes que tengan direcciones de correo electrónico coincidentes que solo difieran en función del caso.
Para corregir direcciones de correo electrónico duplicadas dentro de una instancia de Workfront:

1. Examine los usuarios duplicados y decida qué usuario ya no es necesario.

   {{step-1-to-users}}

   1. En el menú **Filtro**, seleccione **Todos**.

   1. En el menú **Ver**, seleccione **Inicio de sesión de usuario**.

   1. En el menú **Agrupación**, seleccione **Nada**.

   1. Personalice la vista Inicio de sesión de usuario.

      1. Haga clic en **Vista** > **Personalizar vista**.

      1. Reemplace la columna **ID** con la columna **Dirección de correo electrónico**.

      1. Cambie el nombre de la vista y guárdela.

   1. Crear nueva agrupación.

      1. Haga clic en **Agrupación** > **Nueva agrupación**.

      1. Haga clic en **Cambiar al modo de texto** en la esquina superior derecha de la página.
      1. Pegue el siguiente código de modo de texto:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. Cambie el nombre de la agrupación y guárdela.

1. Realice una de las siguientes acciones:

   * (Método preferido) Agregue una dirección + a la dirección de correo electrónico del usuario para cada cuenta adicional.

     Elija esta opción si un solo usuario de su organización necesita acceder a más de una cuenta de usuario. Si su proveedor de correo electrónico no admite el direccionamiento plus, debe proporcionar una cuenta de correo electrónico independiente para cada cuenta de Workfront.

     Por ejemplo, John Doe puede tener una cuenta de usuario para su cuenta de uso diario y otra para utilizarla con fines de prueba:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Cambie el dominio para utilizar un dominio falso añadiendo el siguiente texto a la dirección de correo electrónico:

     `.inactive`

     Por ejemplo, Juan García podría tener los siguientes dominios: (Estos deben ser únicos).

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     Ya no puede iniciar sesión en estas cuentas porque los restablecimientos de contraseña requieren una dirección de correo electrónico válida. Solo se puede acceder a estas cuentas mediante la función Iniciar sesión como.

   * Eliminar usuarios innecesarios

     >[!IMPORTANT]
     >
     >Elija esta opción solo para las cuentas que se crearon por error o para las cuentas de prueba. Esta opción solo se suele aplicar a cuentas con cero o un inicio de sesión erróneo. Las cuentas que se han utilizado con regularidad nunca deben eliminarse.

Si tiene usuarios en una instancia de Workfront con direcciones de correo electrónico coincidentes que solo difieren según el caso, Workfront se pondrá en contacto con usted para proporcionarle información adicional y una cronología cuando sea necesario actualizarlas.

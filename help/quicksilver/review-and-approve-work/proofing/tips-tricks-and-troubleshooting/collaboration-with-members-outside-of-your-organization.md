---
title: Prueba de las limitaciones de colaboración con personas fuera de la organización
description: Prueba de las limitaciones de colaboración con personas fuera de la organización
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Prueba de las limitaciones de colaboración con personas fuera de la organización

Existen algunas limitaciones que deben tenerse en cuenta al comunicarse con personas ajenas a la organización cuando se añaden a una prueba, específicamente si la persona fuera de la organización tiene acceso de prueba en un entorno independiente.

## Contactos con distinción de Miembro

Existen tres tipos de contactos en un entorno de prueba:

* **Usuarios**: Los usuarios tienen un inicio de sesión de prueba de Workfront en el entorno de su organización.
* **Miembros**: Los miembros tienen su propio inicio de sesión de Workfront Proof en el entorno de otra organización (no el suyo propio). No puede convertir miembros a usuarios en su entorno.
* **Invitados**: Los clientes no tienen su propio inicio de sesión de prueba de Workfront en el entorno de su organización, pero ha añadido sus detalles a su cuenta (por ejemplo, revisores invitados en pruebas). Puede convertir invitados en usuarios.

Debido a que los miembros no se pueden convertir en usuarios, su capacidad para etiquetar a las personas en comentarios de prueba está limitada a los usuarios de *su organización original*.

**Ejemplo:** La empresa A invita a un usuario externo a revisar una prueba. Este usuario ya existe en un entorno de prueba independiente, Empresa B.

 

Cuando la empresa A invita al usuario externo a la prueba, el usuario externo se agrega a la lista de contactos de la empresa A como miembro. Los revisores del flujo de trabajo de prueba de la empresa A pueden etiquetar al usuario externo en comentarios de prueba porque ahora están en el directorio de contacto de la empresa A.

 

El usuario externo no puede etiquetar a los usuarios de la empresa A, aunque estén en el mismo flujo de trabajo de prueba, ya que los usuarios de la empresa A no se han agregado como contactos a la empresa B.

 

El usuario externo de la Empresa B puede etiquetar a otros usuarios de la Empresa B si están en el flujo de trabajo de prueba o si tienen permiso para compartir la prueba con nuevos usuarios porque esos usuarios existen como contactos en la Empresa B.

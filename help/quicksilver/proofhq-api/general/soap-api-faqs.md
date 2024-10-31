---
title: SOAP Preguntas frecuentes sobre API de
description: SOAP Preguntas frecuentes sobre API de
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 79b6370ec3283922a16435e8eb8069f7f9560c55
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# SOAP Preguntas frecuentes sobre API de

## ¿Cómo creo mi primera revisión de archivo?

Realiza 3 sencillos pasos:

**Paso 1**: Cargue el archivo en Workfront Proof enviándolo mediante una petición Post a  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Le devolveremos el hash del archivo. ¡Esto es muy importante! Tenga en cuenta que en este momento no verá nada en su cuenta, todo lo que ha hecho hasta ahora es enviarnos el archivo, pero no nos dijo qué hacer con él.

**Paso 2**: Si aún no tiene un ID de sesión, consiga uno mediante los métodos doLogin() o getSessionID(). Utilice la primera para &quot;iniciar sesión&quot; con la dirección de correo electrónico y la contraseña de un usuario o el segundo método si tiene la dirección de correo electrónico y el token de autenticación del usuario.

**Paso 3:** Ahora es el momento de crear su revisión. Utilice el método createProof() y envíenos al menos los campos obligatorios (actualmente solo hay 5). Asegúrese de establecer el parámetro Hash en el hash de archivo devuelto durante el &quot;Paso 1&quot;, ya que esto nos permite determinar qué archivo utilizar al crear la prueba.

Si ahora inicia sesión en su cuenta, verá la prueba.

## ¿Cómo creo mi primera revisión de instantánea web?

Realiza dos sencillos pasos:

**Paso 1**: Si aún no tiene un ID de sesión, consiga uno mediante los métodos doLogin() o getSessionID(). Utilice la primera para &quot;iniciar sesión&quot; con la dirección de correo electrónico y la contraseña de un usuario o el segundo método si tiene la dirección de correo electrónico y el token de autenticación del usuario.

**Paso 2:**Ahora es el momento de crear la prueba. Utilice el método createProof() y envíenos al menos los campos obligatorios (actualmente solo hay 5). Asegúrese de establecer el parámetro Hash en &quot;web&quot; y el parámetro SourceName como URL de la página web que desea capturar.

Si ahora inicia sesión en su cuenta, verá la prueba.

## ¿Cuál es la diferencia entre una prueba y una versión?

En Workfront Proof, las versiones se muestran como una sola Prueba. Al hacer clic en una versión específica en la interfaz de usuario web se muestran los detalles de esa versión. En realidad, cada versión es una prueba independiente y la interfaz de usuario web las muestra juntas.

Desde la perspectiva de la API, cada versión es una prueba independiente y las pruebas están vinculadas entre sí por sus ID.

**createProof()** siempre creará **versión 1** de la revisión. Supongamos que para nuestro ejemplo el ID devuelto para esta prueba es &quot;100&quot;.

Al usar **createProofVersion()**, envíe siempre el ID de la versión anterior. Si queremos crear **versión 2** en la prueba &quot;100&quot;, **pasamos &quot;100&quot; para el parámetro ParentFileID**. Esto indica al sistema que esta prueba debe ser la versión 2 del conjunto. El método devolverá un ID de prueba único, por ejemplo, supongamos que es &quot;101&quot;.

Si se requiere una tercera versión, por ejemplo **versión 3**, llamará a **createProofVersion()** de nuevo y esta vez **pasará &quot;101&quot; para ParentFileID**, lo que garantizará que la lista de versiones vinculada se haya creado correctamente.

## ¿Necesito obtener un nuevo ID de sesión antes de cada llamada a?

Es importante señalar que, en esencia, cada ID de sesión es un usuario que realiza las acciones. 

No es necesario obtener un nuevo ID de sesión antes de cada llamada a la API, por lo que seguirá siendo válido durante 24 horas. La hora de caducidad se restablece cada vez que realiza una llamada a la API.

## ¿Qué es una prueba o una URL personal?

**Equipo/Público**: Cada versión de revisión tiene una dirección URL de equipo (pública) única. Si está activada, se abrirá la prueba en modo de solo lectura. Puede obtener la dirección URL del equipo mediante el método [getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html).

**Personal**: Una dirección URL personal es única para cada versión de revisión y revisión. Si un conjunto de pruebas contiene 3 versiones y un revisor está en todas las versiones, el revisor tendrá 3 URL personales únicas. Una dirección URL personal abre la versión de prueba con el revisor ya identificado y, por lo tanto, debe mantenerse a salvo y no compartirse. Las direcciones URL personales se pueden obtener llamando al método [getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html) y luego iterando cada una  [SOAPReceptientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html) y obteniendo el parámetro &quot;proof_url&quot;.

## >¿Cómo se incluyen los parámetros personalizados al abrir la prueba mínima?

La prueba mínima le permite incrustar la herramienta de prueba en su propia página. Se puede incluir un parámetro &quot;referer&quot; como parte de la prueba mínima para proporcionar una URL de redireccionamiento cuando un usuario haga clic en el botón cerrar de la prueba mínima. Puede incluir cualquier número de parámetros personalizados como parte de esta dirección URL de redireccionamiento anexándolos con el carácter &quot;&amp;&quot; de escape, por ejemplo: %26.

Por ejemplo, la URL de prueba mínima
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` debe codificarse como 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` para que se pasen los parámetros personalizados.



---
title: Aviso de privacidad
permalink: /privacidad/
lang: es
---

# Aviso de privacidad de PlatinoHunter

**Última actualización:** 9 de octubre de 2026 · [Read in English](../privacy/)

PlatinoHunter es una aplicación para Android que te ayuda a seguir tus trofeos de PlayStation Network, encontrar guías y descubrir qué platinar después. Este aviso explica qué datos usa la app, para qué, dónde se guardan y con quién se comparten.

**En resumen:** la app no tiene servidores propios. Tus datos se guardan solo en tu teléfono y no los vendemos ni los recopilamos. La app solo se conecta a los servicios de terceros que necesita para funcionar (Sony, la tienda de Steam y webs de guías) y a Google AdMob para mostrar **como mucho un anuncio al día** (ver la sección 5).

> PlatinoHunter es una app independiente. **No está afiliada, patrocinada ni aprobada por Sony Interactive Entertainment.** «PlayStation», «PSN» y los nombres e imágenes de los juegos pertenecen a sus respectivos propietarios.

---

## 1. Responsable

PlatinoHunter es un proyecto independiente. Para cualquier consulta sobre privacidad puedes escribir a **[chrisrg1303@gmail.com]**.

## 2. Qué datos usa la app y para qué

### 2.1 Tu cuenta de PlayStation Network

- **Inicio de sesión.** Inicias sesión en la página oficial de Sony, que se abre en tu navegador (Chrome) o en un navegador integrado. **La app nunca ve tu contraseña ni tu passkey.** Sony le entrega un código de acceso que la app cambia por un token de sesión. También puedes pegar a mano un token de sesión (NPSSO) obtenido de la web de Sony.
- **Datos que la app obtiene de Sony:**
  - Tu nombre de usuario (Online ID), tu avatar y tu nivel de trofeos.
  - Tu lista de juegos, el progreso de trofeos y los trofeos de cada juego (nombres, descripciones, fecha en que los conseguiste y rareza).
  - La lista de tus amigos de PSN.
- **Para qué:** mostrarte tu biblioteca y tu progreso, crear tus recomendaciones, tu collage de platinos y tus tarjetas de reseña.

### 2.2 Datos de tus amigos de PSN

Para mejorar las recomendaciones, la app consulta qué platinos han conseguido tus amigos con **perfil público** y en qué orden. Los perfiles privados se saltan.

- Su identificador de cuenta **no se guarda en claro**: se guarda un resumen irreversible (hash SHA-256 truncado), que no permite saber quién es.
- De cada amigo solo se guarda qué juegos ha platinado y cuándo. No se guardan ni su nombre de usuario ni su avatar.
- Estos datos se quedan en tu teléfono y no se envían a ningún sitio.

### 2.3 Tus reseñas

Las reseñas que escribes (nota, «me gusta» y texto) se guardan **solo en tu teléfono**. Solo salen de él si tú decides compartir la imagen de la reseña.

### 2.4 Lo que la app no recopila

- No usa herramientas de analítica propias. La única excepción es la publicidad de Google AdMob, que se explica en la sección 5.
- No usa sistemas de informes de errores de terceros.
- No accede a tu ubicación, contactos, cámara ni micrófono.
- No pide permisos de almacenamiento: las imágenes se guardan en tu galería con el sistema de Android (MediaStore), sin permisos adicionales.

**Permisos de Android:**

- `INTERNET` y `ACCESS_NETWORK_STATE`: para conectarse a los servicios descritos y saber si hay conexión.
- `WAKE_LOCK` y `FOREGROUND_SERVICE`: los añade el sistema de tareas de Android (WorkManager) para la actualización diaria en segundo plano.
- `AD_ID` y los permisos de *Privacy Sandbox* (`ACCESS_ADSERVICES_*`): los añade Google AdMob para los anuncios (ver la sección 5).

## 3. Dónde se guardan los datos

Todo se guarda **en tu teléfono**:

- **Token de sesión de PSN:** cifrado con una clave del almacén seguro de Android (Android Keystore).
- **El resto** (tu biblioteca, trofeos, reseñas, fichas de juegos, índice de guías y datos de amigos): en una base de datos local de la app.
- **Anuncios:** la app guarda el día en que viste el último anuncio, para no mostrarte más de uno al día. Tu elección de consentimiento la guarda en el teléfono la herramienta de consentimiento de Google.
- **Copias de seguridad:** la app tiene desactivada la copia de seguridad automática de Android, así que estos datos no se suben a tu cuenta de Google.

## 4. Servicios de terceros a los que se conecta la app

La app se conecta directamente, siempre por HTTPS, a estos servicios. Cada uno tiene su propia política de privacidad y recibe la información técnica habitual de una conexión, como la dirección IP o el idioma del dispositivo.

| Servicio | Para qué | Qué recibe |
|---|---|---|
| **Sony (PlayStation Network)** · `ca.account.sony.com`, `m.np.playstation.com` | Inicio de sesión y datos de trofeos, perfil y amigos | Tu token de sesión y las peticiones de tus datos |
| **Tienda de Steam (Valve)** · `store.steampowered.com`, `api.steampowered.com` | Completar fichas de juegos (género, dificultad estimada) | **Solo el nombre de juegos**, sin ningún dato tuyo |
| **PlayStationTrophies.org** | Descargar su índice público de guías (una vez por semana) | Una petición anónima |
| **PSNProfiles, PlayStationTrophies.org** | Abrir guías, solo cuando tú lo eliges | Se abren en Chrome; lo que hagas allí se rige por esas webs y por Google |
| **Servidores de imágenes** de Sony y Steam | Cargar portadas, iconos y avatares | Peticiones de las imágenes |
| **Google AdMob** | Mostrar como mucho un anuncio al día y pedir tu consentimiento | Los datos del dispositivo descritos en la sección 5; **nunca** tus datos de PSN |

Políticas de privacidad: [Sony](https://www.playstation.com/legal/privacy-policy/) · [Valve/Steam](https://store.steampowered.com/privacy_agreement/) · [Google (Chrome y AdMob)](https://policies.google.com/privacy).

## 5. Publicidad

La app muestra **como mucho un anuncio al día**, servido por **Google AdMob**. Es un anuncio a pantalla completa (puede ser un vídeo) que aparece al cambiar de sección, nunca al abrir la app, y que puedes cerrar. Google puede recopilar y usar datos del dispositivo, como el identificador de publicidad, la dirección IP y datos técnicos y de interacción con el anuncio, para mostrar anuncios, medirlos y evitar fraudes. Lo hace según su propia política: [cómo usa Google los datos](https://policies.google.com/technologies/partner-sites).

- En el **Espacio Económico Europeo, el Reino Unido y Suiza** (y donde la ley lo exija), la app te pide **consentimiento** antes de mostrar anuncios personalizados. Puedes cambiar tu elección cuando quieras en *Ajustes → Opciones de privacidad de anuncios*.
- Puedes restablecer o desactivar tu identificador de publicidad en *Ajustes de Android → Google → Anuncios*.
- PlatinoHunter **no comparte con AdMob** tus trofeos, tus reseñas ni ningún dato de tu cuenta de PSN.

## 6. Compartir imágenes

El collage de platinos y las tarjetas de reseña se crean **en tu teléfono**. Solo salen de él cuando pulsas **Compartir** (las envías tú a la app que elijas) o **Guardar** (se guardan en tu galería). Ten en cuenta que estas imágenes incluyen tu nombre de usuario de PSN, tu avatar y tus trofeos.

## 7. Cuánto tiempo se guardan y cómo borrarlos

Los datos se guardan en tu teléfono hasta que los borras:

- **Cerrar sesión** (en *Ajustes*) borra tu token de sesión, tu biblioteca, tus trofeos y tu historial de platinos. **Se conservan** tus reseñas, las fichas de juegos, el índice de guías y los datos anónimos de amigos.
- **Para borrarlo todo**, desinstala la app o usa *Ajustes de Android → Aplicaciones → PlatinoHunter → Almacenamiento → Borrar datos*.

Como no tenemos servidores, **no guardamos copia de nada** que podamos consultar o borrar por ti.

## 8. Tus derechos

Como todos tus datos están en tu dispositivo, tienes el control total: puedes consultarlos en la app y borrarlos como se explica arriba. Si vives en un lugar con leyes de protección de datos (por ejemplo, el RGPD en la UE o la LFPDPPP en México) y tienes cualquier duda, escríbenos a la dirección de contacto.

Para los datos que gestionan Sony, Valve o Google, ejerce tus derechos directamente ante ellos.

## 9. Menores

La app no está dirigida a menores de 13 años (o de la edad mínima que fije tu país) y no recopila a sabiendas datos de menores. Para usarla necesitas una cuenta de PlayStation Network, que tiene sus propios requisitos de edad.

## 10. Seguridad

- Todas las conexiones usan HTTPS.
- El token de sesión se guarda cifrado.
- La app nunca maneja tu contraseña de PSN.

Aun así, ningún sistema es infalible: protege tu teléfono con bloqueo de pantalla.

## 11. Cambios en este aviso

Si cambia lo que hace la app con tus datos, actualizaremos este aviso y la fecha de arriba. Los cambios importantes se anunciarán en la propia app.

## 12. Contacto

**[chrisrg1303@gmail.com]**

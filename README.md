# 🚤 BASE DE DATOS PATERAS

Aplicación web para cargar las **tablas de combinar** de cada patera, buscar cualquier dato (NIE, nombre, diligencias…), marcar **triaje**, **protección / decreto**, **desistimientos**, **citaciones de notificación de acuerdo** y **letrado**, y guardar por patera un **mensaje inicial**, un **mensaje final** y unas **observaciones**. Funciona en el ordenador y en el móvil, se instala como una app y **no necesita servidor**. Los datos se guardan en el propio dispositivo o, si lo conectas, en un archivo de la **carpeta compartida** para que varios ordenadores vean los mismos datos.

> **Archivo de la app:** `index.html` (un único archivo).

---

## 📑 Índice

1. [Instalar la app en el móvil](#1-instalar-la-app-en-el-móvil)
2. [Pantalla principal](#2-pantalla-principal)
3. [Cargar tablas de combinar](#3-cargar-tablas-de-combinar)
4. [Año y búsqueda](#4-año-y-búsqueda)
5. [Personas: triaje, protección, desistimiento, citación y letrado](#5-personas-triaje-protección-desistimiento-citación-y-letrado)
6. [Mensaje inicial, mensaje final y observaciones](#6-mensaje-inicial-mensaje-final-y-observaciones)
7. [Cambiar varias pateras de golpe](#7-cambiar-varias-pateras-de-golpe)
8. [Borrar pateras](#8-borrar-pateras)
9. [Varios ordenadores: base de datos en la carpeta compartida](#9-varios-ordenadores-base-de-datos-en-la-carpeta-compartida)
10. [Exportar e importar la base de datos](#10-exportar-e-importar-la-base-de-datos)
11. [Copias de seguridad](#11-copias-de-seguridad)
12. [Problemas frecuentes](#12-problemas-frecuentes)
13. [Publicar la app en GitHub Pages](#13-publicar-la-app-en-github-pages)

---

## 1. Instalar la app en el móvil

Así tendrás un icono junto a tus demás apps, sin abrir el navegador cada vez.

### 🤖 Android (Chrome)

| Paso | Qué hacer |
|---|---|
| 1️⃣ | Abre el enlace en **Chrome**. No lo abras desde WhatsApp ni otra app: copia el enlace y pégalo en Chrome. |
| 2️⃣ | Pulsa los **3 puntos** (⋮) arriba a la derecha. |
| 3️⃣ | Elige **"Añadir a pantalla de inicio"** (en algunos móviles: **"Instalar aplicación"**). |
| 4️⃣ | Pulsa **Añadir / Instalar**. |

### 🍎 iPhone (Safari)

| Paso | Qué hacer |
|---|---|
| 1️⃣ | Abre el enlace en **Safari**. |
| 2️⃣ | Pulsa **Compartir** (cuadrado con flecha hacia arriba). |
| 3️⃣ | Elige **"Añadir a pantalla de inicio"**. |
| 4️⃣ | Pulsa **Añadir**. |

> ⚠️ Los datos se guardan **en cada dispositivo por separado**: lo que hagas en el móvil no aparece solo en el ordenador. Para pasar los datos de uno a otro usa **Exportar / importar** (sección 10). En los ordenadores de la oficina puedes usar la **carpeta compartida** (sección 9). Si borras los datos del navegador, también se borran: exporta la base de datos de vez en cuando.

---

## 2. Pantalla principal

| Zona | Para qué sirve |
|---|---|
| ☰ (arriba a la izquierda) | Menú: Pateras y personas, Cargar tablas, Exportar / importar, Borrar pateras, Copias de seguridad, Guía y Manual. |
| 🟨 **GUÍA DE USO** | Abre la guía rápida en PDF. |
| **Cargar tablas de combinar** | Elige (o arrastra, en el ordenador) las tablas .ods, .xlsx, .xls o .csv. |
| Resumen | Totales del año elegido: pateras, personas, triajes, protecciones, decretos, desistimientos y citaciones. |
| Año / Buscar | Elige el año y busca cualquier dato. |
| **Pateras** | Una tarjeta por patera, con sus botones **Mensaje inicial**, **Mensaje final** y **Observaciones**. |
| **Personas** | En el ordenador, una tabla; en el móvil, una ficha por persona. |
| 📖 **Manual detallado** | Este manual (abajo, siempre visible). |

---

## 3. Cargar tablas de combinar

1. Pulsa **Elegir archivos…** (o ☰ → **Cargar tablas**). En el ordenador también puedes **arrastrar** los archivos a la página.
2. El nombre de la patera sale **del número del nombre del archivo**: `Patera 121.ods` → **Patera 121**. Si el nombre no lleva número, la app lo pregunta.
3. El **año** de cada persona sale de la columna **fecha de detención**.
4. Si la patera **ya estaba cargada**, la app pregunta:
   - **Añadir solo las personas nuevas** (las que ya estaban no se tocan).
   - **Reemplazar todo**: se carga la tabla de nuevo, pero se **conserva** lo marcado (triaje, protección, desistimiento, citación y letrado) de las personas que sigan en la tabla.
5. Al terminar aparece un resumen con las personas añadidas.

> 💡 Los `.xls` antiguos necesitan **conexión a internet** la primera vez (se descarga el lector). Los `.ods`, `.xlsx` y `.csv` funcionan sin conexión.

---

## 4. Año y búsqueda

- **Año:** muestra solo las pateras y personas de ese año (o **Todos los años**).
- **Buscar:** escribe cualquier dato (NIE, nombre, diligencias, nacionalidad, letrado…). Debajo aparece **en qué pateras está** lo buscado; toca una para ver solo esa.
- **Toca una tarjeta de patera** para ver solo sus personas. Vuelve a tocarla (o pulsa la **✕** del filtro) para verlas todas.
- **Todas las columnas** (ordenador): muestra también las columnas extra de las tablas.
- **Limpiar** borra la búsqueda y el filtro de patera.

---

## 5. Personas: triaje, protección, desistimiento, citación y letrado

Todo se **guarda solo** al cambiarlo.

| Campo | Tipo | Cómo se rellena |
|---|---|---|
| **Triaje** | Lista | Con Triaje (azul) · Sin triaje (naranja) |
| **Protección/Decreto** | Lista | Protección (verde) · Decreto (rojo) |
| **Fecha notificación desistimiento** | Fecha + ✔ | La fecha y el círculo verde cuando ya se ha realizado |
| **Citación noti acuerdo** | Fecha | Fecha de la citación |
| **Hora noti acuerdo** | Hora | Hora de la citación |
| **Letrado y tlf** | Texto libre | Nombre del letrado y teléfono |

- Toca el **nombre de la patera** o el **N.º** (ordenador), o **ver ficha** (móvil), para ver la **ficha completa** de la persona.

---

## 6. Mensaje inicial, mensaje final y observaciones

Cada tarjeta de patera tiene tres botones: **Mensaje inicial**, **Mensaje final** y **Observaciones**.

1. Pulsa el botón: se abre un cuadro grande de texto libre.
2. Escribe o pega el texto.
3. Pulsa **💾 Guardar mensaje**. El texto queda **asociado al número de la patera**.
4. Cuando el botón tiene texto guardado se ve **relleno y con ✔**.
5. **📋 Copiar** copia el texto; **📤 Compartir** abre el menú de compartir del móvil (WhatsApp, correo…).

> ⚠️ Si cierras sin pulsar **Guardar mensaje**, la app avisa de que hay cambios sin guardar. Si borras todo el texto y guardas, el mensaje se elimina.
>
> 💡 Si eliminas una patera, sus mensajes **se conservan** y vuelven a aparecer si la cargas de nuevo.

---

## 7. Cambiar varias pateras de golpe

1. Marca la casilla de las **pateras** (o de **personas** sueltas) que quieras. **Marcar todas** marca todas las del año.
2. Abajo aparece una barra: elige **Triaje** y/o **Protección/Decreto** (o **Dejar vacío**).
3. Pulsa **Aplicar** y confirma. Antes se guarda una copia de seguridad.

---

## 8. Borrar pateras

Hay dos formas:

- **Una sola:** la papelera 🗑 de su tarjeta (solo se ven las pateras del año elegido).
- **Varias a la vez, de cualquier año:** ☰ → **Borrar pateras**.

1. En la lista salen **todas las pateras**, con su año, número de personas y mensajes. Puedes filtrar por número o año.
2. **Marca** las que quieras borrar (o **Marcar todas**).
3. Si quieres, activa **Borrar también sus mensajes**. Si no, los mensajes se conservan y vuelven a aparecer si cargas esa patera otra vez.
4. Pulsa **Borrar seleccionadas**. El botón cambia a *"Pulsa otra vez para confirmar el borrado"*: púlsalo otra vez.

> 🛡 Antes de borrar se guarda una **copia de seguridad**. Si te equivocas: ☰ → **Copias de seguridad** → **Restaurar**.

---

## 9. Varios ordenadores: base de datos en la carpeta compartida

Si abres la app en dos ordenadores, **cada uno guarda sus datos en su propio navegador**. Para que todos trabajen con **los mismos datos**, la app usa un archivo de base de datos en la carpeta compartida: **`BASE DE DATOS\pateras_datos.js`**, en la misma carpeta donde está el HTML.

> Abre siempre la app desde la carpeta compartida: `\\10.45.17.73\CarpetaCompartida\00 PROGRAMAS EXTRANJERÍA\00. BASE DE DATOS.html`.

### Ponerlo en marcha (una vez en cada ordenador)

1. ☰ → **Carpeta compartida** → **📁 Usar la base de datos de la carpeta compartida**.
2. **Si todavía no existe** (solo el primer ordenador, el que tiene los datos): pulsa **➕ Crear la base de datos compartida**. Se abre la ventana «Guardar como»: si no está ya en la carpeta `BASE DE DATOS`, pega con **Ctrl+V** en «Nombre:» (la ruta completa ya está copiada) y pulsa **Guardar**.
3. **Si ya existe**: la app la lee directamente, sin ventanas. Si ese ordenador tiene datos que no están en ella, pregunta si **añadirlos** (recomendado).

### Día a día

| Qué | Cómo |
|---|---|
| **Ver los datos** | Automático: al abrir la app se lee la base de datos compartida y se actualiza sola cada pocos segundos con lo que hagan los demás. |
| **Guardar cambios** | Una vez cada vez que abras la app: pulsa **💾 Activar guardado** (arriba, o sale solo al hacer el primer cambio) → en la ventana «Guardar como» pulsa **Guardar** → **Sí** para reemplazar. A partir de ahí, todo se guarda solo hasta que cierres la app. |

- Arriba se ve el estado: naranja **«Viendo la base de datos compartida… Activar guardado»** o verde **«Conectado… guardado activado»**.
- Antes de guardar, la app trae lo último que hayan hecho los demás: **no se pisan los cambios** aunque dos personas trabajen a la vez.
- Si en la ventana «Guardar» se elige otra carpeta o nombre, la app lo detecta y avisa: hay que guardarlo exactamente en `BASE DE DATOS\pateras_datos.js`.

> 🔐 Por seguridad, Edge no deja que una página guarde en una carpeta de red sin que la persona lo confirme en la ventana «Guardar», y no recuerda ese permiso al cerrar la app. Por eso hace falta **Activar guardado** una vez por sesión.
>
> 📄 El archivo antiguo `pateras_datos.json` ya no se usa. Si tiene datos que no estén en ningún ordenador, impórtalo con **Exportar / importar → Importar solo datos nuevos**.
>
> 🔌 **Desconectar** (☰ → Carpeta compartida) deja de usar la base de datos compartida; el ordenador se queda con una copia y el archivo no se borra.
>
> 🛡 Las copias de seguridad automáticas se guardan en cada ordenador. Exporta la base de datos de vez en cuando para tener otra copia.

---

## 10. Exportar e importar la base de datos

Abre **☰ → Exportar / importar base de datos**.

### Exportar

| Botón | Qué genera |
|---|---|
| **⬇ Exportar base de datos** | Un archivo `.json` con **todo** (pateras, personas, marcas, citaciones, letrados y mensajes). Es el que sirve para importar en otro dispositivo o guardar una copia. En el móvil puedes **Compartir / enviar**. |
| Lo que veo ahora (.csv) | La tabla con el año y la búsqueda actuales, para Excel / LibreOffice. |
| Todas las personas (.csv) | Todas las personas y todas las columnas, para Excel / LibreOffice. |

### Importar

| Botón | Qué hace |
|---|---|
| **➕ Importar solo datos nuevos** | Añade las pateras, personas y mensajes que **no tengas**. No borra ni cambia nada de lo que ya hay; solo **rellena los campos vacíos** (por ejemplo, un letrado o una citación que pusiste en otro dispositivo). |
| **♻ Importar y reemplazar todo** | Sustituye **toda** la base de datos por la del archivo. Antes se guarda una copia de seguridad. |

> 💡 También se puede importar el archivo **`pateras.db`** del programa antiguo (carpeta `BASE DE DATOS`), con cualquiera de los dos botones. Necesita conexión a internet.
>
> 🔁 **Para trabajar en el ordenador y en el móvil:** exporta en uno y usa **Importar solo datos nuevos** en el otro.
>
> 🔒 El archivo exportado contiene **datos personales**. Guárdalo en un sitio seguro y **no lo subas nunca a GitHub**.

---

## 11. Copias de seguridad

La app guarda **copias automáticas** dentro del navegador: al abrirla (cada pocas horas), antes de cargar tablas, de eliminar una patera, de un cambio en bloque, de importar o de restaurar, y cada rato mientras editas. Se guardan las **30 últimas**.

1. ☰ → **Copias de seguridad**.
2. **＋ Crear copia ahora** para hacer una en el momento.
3. **Restaurar** vuelve a los datos de esa copia (antes se guarda una copia de lo actual, por si te arrepientes).

> ⚠️ Estas copias están **en el mismo navegador**. Si se borran los datos del navegador, se pierden también. Para una copia segura, **exporta la base de datos** (sección 10).

---

## 12. Problemas frecuentes

| Problema | Solución |
|---|---|
| En otro ordenador no salen los datos | Cada navegador guarda sus datos. Conecta todos los ordenadores a la **carpeta compartida** (sección 9). |
| En el móvil no veo lo que hice en el ordenador | Es normal: cada dispositivo guarda sus datos. Exporta en uno e importa (solo datos nuevos) en el otro. |
| Sale *Activar guardado* al abrir la app | Es normal: Edge pide confirmar la ventana «Guardar» una vez por sesión para poder guardar en la red. Ver los datos no necesita nada. |
| *Not allowed to request permissions…*, *Hace falta permiso…* o *No se puede abrir esta carpeta porque contiene archivos del sistema* | Eran fallos de versiones anteriores con Edge. Usa la **versión 4** (sale abajo, junto a «Manual detallado»). |
| *Se ha guardado en otro sitio* | En la ventana «Guardar» se eligió otra carpeta. Vuelve a pulsar **Activar guardado** y pega la ruta con **Ctrl+V** en «Nombre:». |
| *No se puede leer la base de datos compartida* | La carpeta compartida no está disponible (red, servidor apagado o el archivo se ha movido). Pulsa **Reintentar**. |
| No lee un `.xls` | Necesita internet la primera vez. O guarda la tabla como `.xlsx` u `.ods`. |
| No lee el `pateras.db` antiguo | Necesita internet para cargar el lector de bases de datos. |
| Una tabla sale sin año | La tabla no tiene una columna de **fecha de detención** reconocible. Revisa el título de esa columna. |
| He borrado algo sin querer | ☰ → **Copias de seguridad** → **Restaurar** la copia anterior. |
| Se han perdido los datos | Pasa si se borran los datos del navegador o se desinstala la app. Importa tu último `.json` exportado. |

---

## 13. Publicar la app en GitHub Pages

1. En [github.com](https://github.com) crea un **repositorio nuevo** (por ejemplo `gestor-pateras`), público.
2. Sube a la raíz del repositorio los archivos **`index.html`**, **`README.md`**, **`Guia_de_uso_Gestor_de_pateras.pdf`** y **`.gitignore`** (opción *Add file → Upload files*). El `.gitignore` evita que se suban por error archivos con datos.
3. Ve a **Settings → Pages**.
4. En *Source* elige **Deploy from a branch**, rama **main** y carpeta **/ (root)**. Pulsa **Save**.
5. Espera uno o dos minutos. La dirección será normalmente `https://TU-USUARIO.github.io/gestor-pateras/`.
6. Abre esa dirección en el ordenador o en el móvil y sigue el apartado 1 para instalarla.

> 📁 **Versión web y carpeta compartida.** La base de datos compartida (sección 9) solo funciona abriendo la app **desde la carpeta compartida** (`00. BASE DE DATOS.html`). Desde la dirección de GitHub (por ejemplo, en el móvil), cada dispositivo guarda sus propios datos; para pasarlos usa **Exportar / importar** (sección 10). En la carpeta compartida podéis poner el mismo `index.html` renombrado como `00. BASE DE DATOS.html`.
>
> 🔓 Una web de GitHub Pages es pública para quien tenga el enlace, pero **la app no lleva datos**: los datos de cada usuario se guardan solo en su dispositivo.
>
> 🚫 **No subas nunca** al repositorio las tablas de combinar, el `pateras.db`, el `pateras_datos.js` de la carpeta compartida ni los `.json` exportados: contienen datos personales.
>
> 🔄 Para actualizar la app, sube el nuevo `index.html` sustituyendo el anterior. Los datos guardados no se pierden.

---

## 🧱 Notas técnicas

- App de un solo archivo HTML, sin servidor.
- Datos guardados localmente en el navegador (IndexedDB) y, opcionalmente, en `BASE DE DATOS/pateras_datos.js` de la carpeta compartida: se lee como script (sin permisos) y se escribe con la File System Access API (ventana «Guardar»).
- Lee `.xlsx`, `.ods` y `.csv` sin librerías externas. Los `.xls` usan [SheetJS](https://sheetjs.com/) y el `pateras.db` antiguo usa [sql.js](https://sql.js.org/), cargados desde internet solo cuando hacen falta.
- Reconoce a las mismas personas que el programa antiguo, así que importar su base de datos y seguir cargando tablas no duplica a nadie.

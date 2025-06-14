# 🖥️ Radiopatito 42

Un userscript para mejorar la visualización de usuarios en los clústeres de la intranet de 42.

## 📋 Descripción

**Radiopatito 42** es un userscript que mejora la experiencia de visualización en la sección de clústeres de la intranet de 42 (`meta.intra.42.fr/clusters`). Permite ver de forma ampliada las imágenes de perfil de todos los estudiantes conectados en los clústeres, junto con información útil como su login y el ordenador que están utilizando.

## ⚠️ Disclaimer

**Este userscript contiene bromas internas, emojis excesivos y algunas faltas de ortografía intencionales** que forman parte del humor entre mi grupo de amigos de 42. Lo comparto porque funciona bastante bien y puede ser útil para otros estudiantes.

**¿Quieres eliminarlo?** Si prefieres una versión más seria, sin bromas o en otro idioma, ve directamente a la sección **[🌍 Personalización e internacionalización](#-personalización-e-internacionalización)** donde se explica cómo cambiar todos los textos de la interfaz.

**Créditos**: Este userscript empezó un día de aburrimiento con Claude Sonnet 4 de Claude.ai y poco a poco se ha ido puliendo y mejorando. El readme también lo he hecho yo, la Claude; tu IA de confianza 😘😘😘

---

### ✨ Características

- 🔍 **Imágenes ampliadas**: Visualiza las fotos de perfil 15 veces más grandes que el tamaño original
- 👥 **Vista de cuadrícula**: Organiza todas las imágenes en una cuadrícula responsive
- 🏢 **Filtros por clúster**: Filtra usuarios por Clúster A (car*) o Clúster B (cbr*)
- ❤️‍🔥 **Sistema de favoritos**: Añade y gestiona una lista de tus "panas" favoritos
- 💤 **Usuarios offline**: Ve el estado de tus favoritos aunque no estén conectados
- 🔎 **Buscador de usuarios**: Busca patitos específicos por username
- 📊 **Información detallada**: Muestra el login del usuario y el ID del ordenador
- 🔗 **Enlaces directos**: Click en cualquier imagen para ir al perfil del usuario
- 🌍 **Textos configurables**: Sistema de internacionalización fácil de modificar
- 🎨 **Interfaz moderna**: Diseño dark con bordes redondeados y sombras
- 📱 **Responsive**: Se adapta a diferentes tamaños de pantalla
- ⚡ **Gestión de errores**: Manejo elegante de imágenes que no cargan
- 🎲 **Imagen aleatoria**: Si un usuario no existe, muestra una imagen consoladora
- 💾 **Persistencia**: Los favoritos se guardan permanentemente

## 🚀 Instalación

### Paso 1: Instalar un gestor de userscripts

### 🖥️ Compatibilidad PC
- ✅ **Violentmonkey** (Recomendado para escritorio)
- ✅ **Tampermonkey** (Solo firefox en escritorio)
- ❓ **Greasemonkey** (No probado)

### Paso 2: Instalar el script

Tienes dos opciones para instalar **Radiopatito 42**:

#### 🌟 Opción A: Copiar y pegar el código (Recomendado)

1. Instala [Violentmonkey](https://violentmonkey.github.io/) en tu navegador
2. Copia el código completo del userscript desde GitHub:
   - Ve al archivo <a href="./Radiopatito_42" target="_blank" rel="noopener noreferrer">`Radiopatito_42`</a> en este repositorio
   - Haz click en **"Copy raw file"** para copiar el código sin formato

3. Abre el dashboard de Violentmonkey
4. Haz click en **"+ Nuevo"** o **"New Script"**
5. **Borra todo** el contenido que aparece por defecto
6. **Pega el código** del userscript (`Ctrl+V`)
7. Guarda el script (`Ctrl+S`)

#### 📁 Opción B: Arrastrar archivo

1. Instala [Violentmonkey](https://violentmonkey.github.io/) en tu navegador
2. Descarga el archivo <a href="./Radiopatito_42" target="_blank" rel="noopener noreferrer">`Radiopatito_42`</a> desde este repositorio
3. Arrastra el archivo al dashboard de Violentmonkey o haz click en "Install" cuando se abra automáticamente

### Paso 3: Activar el script

1. **Ve a la página de clústeres**: Navega a `https://meta.intra.42.fr/clusters`
2. **Refresca la página** si ya estabas en esa URL antes de instalar el script
3. **¡Listo!** Deberías ver el botón **"Lo mismo pero grande"** en la esquina inferior derecha

**⚠️ Permisos requeridos**: El script ahora requiere permisos de almacenamiento (`GM_setValue` y `GM_getValue`) para guardar favoritos.

### 📱 Compatibilidad móvil

**Radiopatito_42_Movil** es la versión móvil probada en Firefox usando **Tampermonkey**.

Compatibilidad adicional:
- ❓ **Greasemonkey** (No probado)
- ❓ **Violentmonkey** (No probado)
<img src="radiopatito_mobile.jpg" alt="Vista móvil de Radiopatito 42" width="200">
*Radiopatito 42 funcionando en Firerox móvil con Tampermonkey*

## 🎯 Uso

1. Navega a la sección de clústeres en la intranet: `https://meta.intra.42.fr/clusters*`
2. Verás un botón en la esquina inferior derecha que dice **"Lo mismo pero grande"**
3. Haz click en el botón para abrir la vista ampliada
4. Disfruta de ver todos los "patitos" 🦆 conectados en una vista mejorada

### 🖱️ Controles principales

- **Botón principal**: Abre/actualiza la vista de imágenes ampliadas
- **Botón × (superior derecho)**: Cierra la vista ampliada
- **Botón 🔍 (superior izquierdo)**: Abre el buscador de usuarios
- **Click en imagen**: Va al perfil del usuario en una nueva pestaña
- **Scroll**: El título se desvanece automáticamente al hacer scroll

### 🏢 Filtros por clúster

Una vez abierta la vista ampliada, encontrarás **cuatro botones** de filtro en la parte superior:

- **Todo 42**: Muestra todos los usuarios conectados (por defecto)
- **Clúster A**: Filtra solo usuarios en estaciones que empiecen por "car" (ej: car1s1)
- **Clúster B**: Filtra solo usuarios en estaciones que empiecen por "cbr" (ej: cbr1s1)
- **❤️‍🔥 Los panas ❤️‍🔥**: **NUEVO** - Muestra tu lista de favoritos

El título se actualiza automáticamente para mostrar cuántos patitos hay en cada clúster.

### ❤️‍🔥 Sistema de favoritos - ¡NUEVA FUNCIONALIDAD!

#### Gestión de favoritos

Al hacer click en "❤️‍🔥 Los panas ❤️‍🔥", accedes a tu lista personal de favoritos con dos botones de gestión:

- **➕ Añadir pana**: Añade nuevos usuarios a tu lista de favoritos
- **💔 Divorcio**: Elimina usuarios de tu lista de favoritos

#### Estados de favoritos

Los usuarios favoritos pueden aparecer en dos estados:

1. **🟢 Online (Conectado)**:
   - Imagen normal del perfil
   - ID del ordenador donde están conectados
   - Enlace directo al perfil

2. **💤 Offline (Desconectado)**:
   - Imagen aleatoria de [Picsum](https://picsum.photos/)
   - Estilo visual diferenciado (bordes rosas, opacidad reducida)
   - Texto "🔌 Offline" en lugar del ID del ordenador
   - Mensaje "❤️‍🔥 Tu pana está offline ❤️‍🔥"
   - **✨ NUEVA MEJORA**: También puedes hacer click para ir a su perfil

#### ➕ Añadir favoritos

1. **Acceso**: Click en "❤️‍🔥 Los panas ❤️‍🔥" → "➕ Añadir pana"
2. **Formulario**: Escribe el username exacto del usuario
3. **Métodos de añadir**:
   - Click en "❤️ Añadir a los panas ❤️"
   - Presiona Enter
4. **Validaciones**:
   - Previene duplicados automáticamente
   - Valida campos vacíos
   - Feedback visual inmediato

#### 💔 Gestión de divorcios - **¡MEJORADO!**

1. **Acceso**: Click en "❤️‍🔥 Los panas ❤️‍🔥" → "💔 Divorcio"
2. **Interfaz**: Lista con checkboxes de todos tus favoritos
3. **✨ NUEVA LÓGICA**: 
   - **Todas las casillas aparecen desmarcadas por defecto**
   - **Marca las casillas** de los panas de los que te quieres divorciar
   - **Mucho más seguro**: No hay riesgo de divorciarte accidentalmente de todos
4. **Confirmación**: Mensaje de confirmación antes de eliminar
5. **Resultado**: Feedback con usuarios eliminados

#### 🎯 Ordenación inteligente de favoritos

Los favoritos ahora se muestran en orden de prioridad:
- **Primero**: Panas conectados (online) 💚
- **Después**: Panas desconectados (offline) 💤

Esto hace que sea más fácil ver de un vistazo quiénes de tus panas están disponibles.

#### Características técnicas de favoritos

- **💾 Persistencia**: Los favoritos se guardan permanentemente usando `GM_setValue`/`GM_getValue`
- **🔄 Auto-refresh**: La vista se actualiza automáticamente tras cambios
- **🛡️ Gestión de errores**: Manejo robusto de datos corruptos
- **📱 Responsive**: Interfaz adaptada a móviles
- **⌨️ Atajos de teclado**: Escape para cerrar modales, Enter para confirmar
- **🔗 Enlaces universales**: Click en cualquier pana (online u offline) va a su perfil

### 🔎 Buscador de usuarios

El buscador te permite encontrar patitos específicos:

1. **Acceso**: Click en el botón 🔍 en la esquina superior izquierda
2. **Búsqueda**: Escribe el username exacto del usuario
3. **Métodos de búsqueda**:
   - Click en el botón "Buscar"
   - Presiona Enter
4. **Resultados**:
   - **Usuario encontrado**: Muestra "🎉 ¡Patito encontrado! 🎉" con la tarjeta del usuario
   - **Usuario no encontrado**: Muestra "❌ Patito no encontrado ❌" con una imagen aleatoria consoladora de [Picsum](https://picsum.photos/)

#### Características del buscador:
- **Búsqueda case-insensitive**: No importa si escribes en mayúsculas o minúsculas
- **Validación**: Avisa si el campo está vacío
- **Imágenes aleatorias**: Cada búsqueda fallida muestra una imagen diferente
- **Atajos de teclado**: 
  - `Enter` para buscar
  - `Escape` para cerrar
- **Auto-focus**: El campo de búsqueda se selecciona automáticamente

## 🌍 Personalización e internacionalización

### Sistema de textos configurables

**Radiopatito 42** v42.4.2 incluye un sistema completo de textos configurables que permite:

- **🔧 Personalización fácil**: Cambia cualquier texto del script
- **🌍 Traducción simple**: Adapta el script a cualquier idioma
- **📝 Mantenimiento**: Todos los textos están organizados en un solo lugar

### Cambiar idioma

Para cambiar el idioma, simplemente modifica el objeto `TEXTS` al principio del script:

```javascript
// Ejemplo: Cambio a inglés
const TEXTS = {
    FAVORITES_BUTTON: '❤️‍🔥 My Buddies ❤️‍🔥',
    ADD_FAVORITE: '➕ Add Buddy',
    REMOVE_FAVORITES: '💔 Remove Friends',
    ADD_MODAL_TITLE: '❤️‍🔥 Add New Buddy ❤️‍🔥',
    SEARCH_MODAL_TITLE: '🔍 Find User 🔍',
    REMOVE_MODAL_SUBTITLE: 'Mark the buddies you want to remove',
    // ... resto de textos
};
```

### Categorías de textos configurables

- **🔘 Botones principales**: Filtros y acciones principales
- **📋 Títulos dinámicos**: Contadores y encabezados
- **❤️ Favoritos**: Toda la interfaz del sistema de favoritos
- **🔍 Búsqueda**: Modal y mensajes de búsqueda
- **👤 Estados de usuario**: Mensajes de online/offline
- **⚠️ Errores**: Mensajes de validación y errores

## 🛠️ Detalles técnicos

### Características del código

- **Namespace**: `Violentmonkey Scripts`
- **Versión**: 42.4.2
- **Permisos requeridos**: 
  - `GM_setValue` (para guardar favoritos)
  - `GM_getValue` (para cargar favoritos)
- **Dominio**: Solo funciona en `https://meta.intra.42.fr/clusters*`

### Funcionalidades implementadas

- Detección automática de imágenes SVG con atributos `xlink:href` o `href`
- Extracción de metadatos de tooltips y atributos de elementos
- Amplificación inteligente de imágenes (15x el tamaño original)
- Grid CSS responsive con `minmax(300px, 1fr)`
- Filtrado dinámico por clústeres basado en IDs de estaciones
- **NUEVO**: Sistema completo de favoritos con persistencia
- **NUEVO**: Gestión de usuarios offline en favoritos
- **NUEVO**: Sistema de internacionalización con textos configurables
- **MEJORADO**: Lógica de divorcio más segura y intuitiva
- **MEJORADO**: Ordenación inteligente de favoritos (online primero)
- **MEJORADO**: Enlaces universales a perfiles (online y offline)
- Sistema de búsqueda con validación y feedback visual
- Gestión de estados de scroll para UX mejorada
- Manejo de errores de carga de imágenes
- Optimizaciones de rendimiento (lazy loading, document fragments)
- Gestión de memoria y cleanup de event listeners

### Nuevas optimizaciones v42.4.2

- **🏗️ Arquitectura mejorada**: Código reorganizado y más mantenible
- **💾 Gestión de almacenamiento**: Sistema robusto de persistencia de datos
- **🎨 Efectos visuales**: Hover effects y transiciones suaves
- **🧩 Interpolación de strings**: Sistema de templates para mensajes dinámicos
- **🔒 Validación mejorada**: Manejo de casos edge y datos corruptos
- **✅ UX mejorada**: Lógica de divorcio más intuitiva y segura
- **📊 Ordenación inteligente**: Favoritos organizados por estado de conexión

### Optimizaciones de rendimiento

- **Lazy loading**: Las imágenes se cargan bajo demanda
- **Document fragments**: Operaciones DOM por lotes para mejor rendimiento
- **Throttled scrolling**: Eventos de scroll optimizados
- **Memory cleanup**: Limpieza automática de event listeners y elementos DOM
- **Event delegation**: Manejo eficiente de eventos para favoritos

## 🎨 Interfaz de usuario

El script proporciona:

### Vista principal
- **Contador dinámico**: "Habemos X 👨‍💻 patitos 👩‍💻 [en Clúster A/B]" o "Habemos X ❤️‍🔥 panas ❤️‍🔥"
- **Grid responsive**: Se adapta automáticamente al tamaño de pantalla
- **Información de usuario**: Login y ID de estación claramente visible
- **Estados visuales**: Diferenciación clara entre usuarios online y offline
- **Ordenación inteligente**: Favoritos online aparecen primero

### Controles de navegación
- **Botones de filtro**: Interfaz intuitiva con feedback visual y estados especiales
- **Controles de favoritos**: Botones dedicados para gestión de favoritos
- **Modal de búsqueda**: Diseño limpio y funcional
- **Botones de acción**: Posicionamiento fijo para fácil acceso

### Nuevos elementos de UI v42.4.2
- **🎨 Hover effects**: Botones con animaciones al pasar el mouse
- **🌈 Estados especiales**: Botón de favoritos con color distintivo
- **📋 Modales mejorados**: Diseño consistente y accesible
- **✨ Transiciones**: Animaciones suaves en todas las interacciones
- **🔒 Interfaz de divorcio mejorada**: Lógica más segura e intuitiva

## 🤝 Contribuir

¿Tienes ideas para mejorar Radiopatito 42? ¡Las contribuciones son bienvenidas!

1. Fork este repositorio
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -am 'Añade nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

### Ideas para futuras mejoras 

- [x] ~~Sección de usuarios favoritos~~ ✅ **¡Implementado en v42.4.2!**
- [x] ~~Mejorar UX del sistema de divorcio~~ ✅ **¡Implementado en v42.4.2!**
- [x] ~~Ordenación de favoritos por estado~~ ✅ **¡Implementado en v42.4.2!**
- [x] ~~Enlaces a perfiles para usuarios offline~~ ✅ **¡Implementado en v42.4.2!**
- [ ] Exportar/importar lista de favoritos
- [x] ~~Notificaciones cuando favoritos se conectan~~ ❌ **Limitado y coñazo, no mola**
- [ ] Estadísticas de tiempo de conexión
- [ ] Temas de colores personalizables
- [ ] Integración con la API de 42 para más información
- [ ] Sistema de grupos/categorías de favoritos

## 📝 Notas

- El script se ejecuta automáticamente después de 1 segundo de cargar la página
- Las imágenes se redimensionan manteniendo la proporción (`object-fit: contain`)
- Compatible con el sistema de tooltips de la intranet de 42
- Incluye logging en consola para debugging
- El buscador solo busca entre usuarios actualmente conectados en los clústeres
- Los filtros por clúster funcionan con el patrón estándar de IDs de 42
- **NUEVO**: Los favoritos se almacenan localmente usando la API de Tampermonkey/Violentmonkey
- **NUEVO**: Los usuarios offline en favoritos muestran imágenes aleatorias únicas
- **MEJORADO**: Los favoritos se ordenan automáticamente (conectados primero)
- **MEJORADO**: Cualquier pana (online u offline) permite click para ir al perfil

## 🔧 Solución de problemas

### El script no funciona
- Verifica que Violentmonkey/Tampermonkey esté instalado y habilitado
- **NUEVO**: Asegúrate de que el script tenga permisos de almacenamiento habilitados
- Asegúrate de estar en la URL correcta: `https://meta.intra.42.fr/clusters*`
- **Refresca la página** si acabas de instalar o modificar el script
- Comprueba la consola del navegador para errores

### No aparecen usuarios
- Verifica que haya usuarios conectados en los clústeres
- Comprueba que la página haya cargado completamente
- **Intenta refrescar la página** (`F5` o `Ctrl+R`)

### El buscador no encuentra usuarios
- Asegúrate de escribir el username exacto
- Recuerda que solo busca entre usuarios actualmente conectados
- Verifica que el usuario esté realmente en algún clúster

### Problemas con favoritos
- **No se guardan los favoritos**: Verifica que el script tenga permisos `GM_setValue` habilitados
- **Favoritos perdidos**: Comprueba si Tampermonkey/Violentmonkey tiene suficiente espacio de almacenamiento
- **Error al añadir**: Asegúrate de escribir usernames válidos sin espacios
- **No aparecen botones**: Verifica que estés en la sección "❤️‍🔥 Los panas ❤️‍🔥"
- **Problema con divorcio**: Si marcaste por error, simplemente desmarca las casillas

### Problemas en móvil
- Asegúrate de usar Chrome con Tampermonkey instalado
- Verifica que el script esté habilitado en Tampermonkey
- Comprueba que estés accediendo desde la URL correcta de la intranet
- **NUEVO**: Los modales de favoritos están optimizados para pantallas pequeñas

### Después de instalar o modificar el script
- **Siempre refresca la página** de clústeres (`https://meta.intra.42.fr/clusters`)
- Si ya estás en la página, presiona `F5` o `Ctrl+R`
- El script necesita ejecutarse desde cero después de cualquier cambio

## 📄 Licencia

Este proyecto está bajo una licencia abierta. Siéntete libre de usar, modificar y distribuir el código.

## 🏫 Sobre 42

Este script está diseñado específicamente para la red de escuelas 42. Si eres estudiante de 42, ¡esperamos que encuentres útil esta herramienta para visualizar mejor a tus compañeros en los clústeres!

---

## 📈 Changelog

### v42.4.2 - Sistema de Favoritos y Mejoras de UX
- ✅ **NUEVO**: Sistema completo de favoritos "❤️‍🔥 Los panas ❤️‍🔥"
- ✅ **NUEVO**: Gestión de usuarios offline en favoritos
- ✅ **NUEVO**: Sistema de textos configurables para internacionalización
- ✅ **NUEVO**: Interfaz de añadir/eliminar favoritos con validaciones
- ✅ **NUEVO**: Persistencia de datos usando GM_setValue/GM_getValue
- ✅ **NUEVO**: Efectos hover y transiciones mejoradas
- ✅ **MEJORADO**: Lógica de divorcio más segura (desmarcado por defecto)
- ✅ **MEJORADO**: Ordenación inteligente de favoritos (online primero)
- ✅ **MEJORADO**: Enlaces universales (panas offline también clickeables)
- ✅ **MEJORADO**: Arquitectura de código reorganizada y más mantenible
- ✅ **MEJORADO**: Gestión de errores más robusta
- ✅ **MEJORADO**: Interfaz responsive optimizada para móviles

### v42 - Versión Base
- ✅ Vista ampliada de imágenes de perfil
- ✅ Filtros por Clúster A y B
- ✅ Buscador de usuarios
- ✅ Interfaz responsive
- ✅ Gestión de errores básica

---

*Hecho con ❤️ para la comunidad de 42*

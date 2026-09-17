🏊‍♂️ Gestor de Cuadrantes y Control de Horas - Piscina y Centro Deportivo

Aplicación web interactiva, moderna y ligera (en un único archivo) diseñada para
la gestión semanal de actividades dirigidas, asignación de monitores y cómputo
automático de horas trabajadas en piscinas, gimnasios o centros deportivos.

Funciona de forma 100% local y offline en el navegador a través de localStorage,
sin necesidad de servidores, bases de datos complejas ni instalaciones.

🚀 Características Principales

  - 📊 Cuadrícula Estilo Hoja de Cálculo (Lunes a Sábado):
      - Visualización clara, compacta y profesional de toda la semana.
      - Filas con contraste alterno acentuado para facilitar la lectura tanto en
        pantalla como en papel.
  - ⏱️ Franjas Horarias con Cálculo Automático:
      - Definición libre de horas de inicio y fin con selector nativo.
      - Cómputo instantáneo de la duración exacta en horas decimales (ej. 0.75 h
        para 45 minutos).
  - 🔀 Reestructuración e Intercalado de Filas a la Izquierda:
      - Botón (+) verde: Intercala una nueva franja horaria justo debajo
        heredando los horarios.
      - Flechas (▲ / ▼): Sube o baja franjas completas de posición sin tener que
        retocar las horas de las filas siguientes.
      - Papelera (🗑): Elimina la franja horaria completa con confirmación.
  - 🏋️ Múltiples Actividades y Salas por Franja:
      - Espacio amplio para el nombre de la actividad.
      - Casilla compacta para la sala/vaso (máx. 3 caracteres: ej. S7, VP, SC,
        S2).
      - Botón integrado en cabecera (+) para añadir actividades simultáneas en
        distintas salas dentro de la misma hora.
  - 👥 Asignación Rápida de Monitores:
      - Modal inteligente con búsqueda rápida por clic, números (ej. 1, 3) o
        nombres separados por comas.
      - Alta sobre la marcha: Si escribes un monitor que no existe, se añade
        automáticamente a la base de datos general.
      - Botón compacto +👤 en línea para no aumentar la altura de las filas.
  - ✅ Control Real de Asistencia (Cómputo de Horas):
      - Cada monitor asignado cuenta con una casilla de verificación (checkbox).
      - Si el monitor no imparte la clase o causa baja, basta con desmarcar su
        casilla: el nombre se tacha y sus horas dejan de sumarse automáticamente
        en el total semanal.
  - 🧮 Pie de Tabla con Totales Semanales:
      - Suma en tiempo real el cómputo exacto de horas realizadas por cada
        monitor durante la semana seleccionada, mostrando tanto el formato
        decimal (14.50h) como el desglose exacto (14h 30m).
  - 📅 Gestión de Semanas y Clonación:
      - Selector y navegación fluida entre distintas semanas del año.
      - Clonador inteligente: Duplica toda la estructura actual (clases, salas y
        monitores) para la siguiente semana, reactivando todas las casillas de
        asistencia por defecto.
      - Creación de calendarios limpios en blanco en un clic.
  - 💾 Copias de Seguridad (Backup) y Portabilidad:
      - Descarga manual en 1 clic: Guarda el archivo backup_piscina.json (nombre
        fijo sin fecha para sobrescribir y no duplicar archivos en el
        Escritorio).
      - Restauración inmediata: Importa el archivo en cualquier otro ordenador o
        tras limpiar la caché.
      - Copia de seguridad automática diaria: Opción configurable para descargar
        un respaldo al abrir la app cada día.
  - 🖨️ Impresión Optimizada en 1 Hoja A4 Horizontal:
      - Estilos dedicados (@media print): oculta botones y controles de edición,
        ajusta tipografías y márgenes para que todo el cuadrante encaje limpio
        en un único folio apaisado o PDF.
  - 🧭 Tour de Ayuda Interactivo Integrado:
      - Guía dinámica paso a paso que resalta visualmente cada herramienta con
        un halo luminoso y explica su funcionamiento con consejos prácticos.

🛠️ Tecnologías Utilizadas

  - HTML5 Semántico: Estructura limpia y accesible.
  - Tailwind CSS (CDN): Diseño moderno, adaptable y responsivo.
  - FontAwesome (CDN): Iconografía vectorial.
  - Vanilla JavaScript (ES6+): Lógica reactiva sin dependencias ni frameworks
    pesados.
  - Web Storage API (localStorage): Persistencia de datos en el cliente.

📦 Puesta en Marcha

No requiere Node.js, PHP, Python ni ningún servidor web:

1.  Descarga el proyecto:
    git clone https://github.com/tu-usuario/cuadrante-piscina.git
2.  Abre la aplicación: Haz doble clic sobre el archivo index.html en tu
    explorador de archivos para abrirlo en cualquier navegador moderno (Google
    Chrome, Microsoft Edge, Mozilla Firefox, Safari, Brave, etc.).

📖 Guía Rápida de Uso

1. Asignar Monitores a una Clase

1.  Haz clic en el botón + Monitor (o +👤 si ya hay uno).
2.  Haz clic sobre el nombre del monitor en la lista rápida, o escribe varios
    nombres/números separados por comas (ej. Julia, Diego o 1, 3).
3.  Pulsa Guardar o la tecla Enter.

2. Controlar la Asistencia

  - Por defecto, el monitor asignado tiene su casilla marcada y computa sus
    horas.
  - Si el monitor no acudió o fue sustituido, desmarca la casilla junto a su
    nombre. El nombre aparecerá tachado y sus horas se descontarán al instante
    del sumatorio al pie de la tabla.

3. Reestructurar el Horario

  - Para insertar una clase intermedia sin reescribir las demás, pulsa el botón
    verde (+) situado en la columna izquierda.
  - Para cambiar de orden una franja completa, usa las flechas ▲ y ▼.

4. Pasar a la Siguiente Semana

1.  Pulsa Clonar Semana en la barra superior.
2.  Escribe el nuevo rango de fechas (ej. Semana del 19 al 24 de Septiembre).
3.  Se generará un nuevo cuadrante idéntico con todas las casillas de asistencia
    activadas de nuevo.

5. Copias de Seguridad y Traslado de Datos

  - Pulsa en Copia / Backup > Descargar backup_piscina.json para guardar tu
    copia en el Escritorio o en un pendrive.
  - Para abrir tus datos en otro equipo, pulsa Copia / Backup > Seleccionar
    backup_piscina.json.

🔒 Privacidad y Almacenamiento

  - 100% Privado: Los datos se procesan y almacenan exclusivamente en el
    navegador local (localStorage).
  - Sin Rastreo: Ningún dato es transmitido por internet ni enviado a servidores
    externos.
  - Modo Avión / Offline: Funciona con total normalidad sin conexión a internet
    (una vez cargadas las hojas de estilo en caché).

📄 Licencia

Este proyecto está bajo la Licencia MIT - puedes utilizarlo, modificarlo y
adaptarlo libremente para tus instalaciones o proyectos personales/comerciales.

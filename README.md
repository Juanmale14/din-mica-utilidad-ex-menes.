📝 DINÁMICA: ¿PARA QUÉ SIRVEN LOS EXÁMENES?

Una aplicación web interactiva, moderna y ligera diseñada para la reflexión en tiempo real en aulas, talleres y conferencias sobre la función y utilidad de las evaluaciones.

Está configurada para conectar directamente con Google Sheets a través de Google Apps Script, permitiendo a los docentes y dinamizadores proyectar en directo las respuestas enviadas por los participantes mediante un Formulario de Google.

🚀 Características Principales

Pizarra Digital Compartida:

Muestra las aportaciones recopiladas en la base de datos de manera limpia y visual.

Formato en tarjetas con colores pastel diferenciados de forma dinámica para facilitar la lectura.

Selección de diseño flexible (de 1 a 4 columnas).

Botón de carga/refresco instantáneo de datos.

Modo Proyección:

Diseñado para proyectores y pantallas grandes de aula.

Visualización por bloques de columnas a pantalla completa con alta legibilidad.

Navegación táctil, con botones o mediante teclado (flechas ← y →).

Panel de Administración (Protegido por Clave):

Acceso restringido para el docente o moderador.

Enlaces directos al Formulario de Google y a la Hoja de Cálculo (para revisión o limpieza de datos).

Exportación de respuestas a archivos Excel (.xlsx) y PDF.

Configuración y prueba de la URL de Google Apps Script en caliente.

Sin Dependencias Pesadas:

Desarrollado en CSS3 nativo (sin Tailwind CSS) para evitar incompatibilidades o problemas de renderizado.

Utiliza FontAwesome para iconografía y SheetJS para exportación a Excel.

🛠️ Estructura del Proyecto

.
├── index.html                       # Aplicación web completa (Single File App)
├── guia_conexion_apps_script.md     # Guía paso a paso para configurar Google Sheets y Apps Script
└── README.md                        # Documentación general del proyecto


📊 Estructura de la Hoja de Cálculo (Google Sheet)

Para que la aplicación procese correctamente la información, la hoja debe estructurarse así:

Columna A

Columna B

Marca temporal

¿PARA QUÉ SIRVEN LOS EXÁMENES?

(Ignorada automáticamente)

(Texto reflejado en la pizarra)

⚙️ Configuración e Integración

Configurar Google Apps Script:

Sigue los pasos descritos en el archivo guia_conexion_apps_script.md adjunto en este proyecto.

Publica la secuencia de comandos de tu hoja como Aplicación Web permitiendo el acceso a "Cualquiera".

Grabar la URL en la Aplicación Web:

Abre index.html en tu editor de código.

Busca la constante URL_APPS_SCRIPT_FIJA al inicio de la etiqueta <script>:

const URL_APPS_SCRIPT_FIJA = "PEGA_AQUÍ_TU_URL_DE_APPS_SCRIPT";


Reemplaza "PEGA_AQUÍ_TU_URL_DE_APPS_SCRIPT" con la URL de tu Web App (terminada en /exec).

Acceso al Panel de Administración:

Para acceder al panel de control, haz clic en la pestaña Administración e introduce la contraseña establecida para el docente/administrador.

📄 Licencia y Créditos

Elaborada por El loco de la mochila en 2026.

Saber más y consultar otros recursos docentes en: [blogsaverroes.juntadeandalucia.es/ellocodelamochila](https://blogsaverroes.juntadeandalucia.es/ellocodelamochila/)

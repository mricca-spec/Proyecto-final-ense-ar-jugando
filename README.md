Rescate Geométrico — Juego para enseñar Matemática
Descripción del proyecto
Rescate Geométrico es un juego digital educativo para trabajar contenidos de geometría, especialmente triángulos, áreas y perímetros. Está dirigido a estudiantes de 8.º grado de Educación Básica Integrada (aproximadamente 13–14 años) y propone aprender mediante desafíos matemáticos de dificultad progresiva.

La propuesta busca promover la participación activa, la resolución de problemas y la revisión de los errores a través de una experiencia interactiva.
Acceso al juego
El repositorio está publicado mediante GitHub Pages. Por eso, el proyecto se puede utilizar desde un navegador web, sin descargar los archivos.
Página publicada: https://mricca-spec.github.io/Proyecto-final-jugar-para-ensenar/

El archivo index.html funciona como página de inicio y permite elegir el perfil de acceso. Si se selecciona “Soy Estudiante”, se abre el juego. La opción “Soy Docente” permite acceder a la planilla de resultados mediante el panel correspondiente.
Archivos del repositorio
- index.html: pantalla de inicio del sitio y selección del perfil de acceso.
- Juego.html: juego interactivo con 12 niveles progresivos, instrucciones, pistas, retroalimentación, registro de intentos y errores y calificación final de 1 a 100.
- Documento .pdf: memoria de la propuesta didáctica, descripción del diseño, funcionamiento, puntuación, integración con Google Sheets y reflexión pedagógica.
¿Cómo funciona?
1. El estudiante ingresa a la página publicada con GitHub Pages.
2. En index.html, selecciona el acceso de estudiante.
3. Escribe su nombre y comienza la misión.
4. Resuelve los 12 niveles en orden. Si se equivoca, recibe una devolución y puede volver a intentarlo; también puede solicitar pistas.
5. Al finalizar, obtiene una calificación de 1 a 100 y un resumen de su desempeño.
6. Los resultados se envían a una hoja de cálculo de Google mediante Google Apps Script.
7. El docente puede consultar los resultados desde la opción correspondiente de la pantalla de inicio.
Contenidos matemáticos
- Condición de existencia de un triángulo y desigualdad triangular.
- Perímetro como suma de longitudes.
- Área de un triángulo: A = (base × altura perpendicular) / 2.
- Cálculo inverso de una medida y despeje de fórmulas.
- Diferencia entre unidades lineales y cuadradas.
- Revisión de procedimientos y detección de errores.
Puntuación
El juego diferencia los puntos de progreso de la calificación final:
- Cada nivel superado suma 10 puntos de juego, hasta un máximo de 120.
- Cada respuesta incorrecta descuenta 4 puntos de la calificación.
- Cada intento posterior al primero dentro de un nivel descuenta 2 puntos adicionales.
- Solicitar una pista no descuenta puntos.
- La calificación final se calcula como 100 − (4 × errores) − (2 × intentos adicionales), con un mínimo de 1 y un máximo de 100.
La calificación automática representa el recorrido registrado en la partida y no sustituye por sí sola la evaluación docente.
Tecnologías utilizadas
- HTML, CSS y JavaScript para la estructura, el diseño y la lógica del juego.
- GitHub Pages para publicar el proyecto como página web.
- Google Sheets para registrar los resultados.
- Google Apps Script para gestionar el envío de datos a la hoja de cálculo.
Consideraciones técnicas
La integración con Google Sheets depende de que el servicio de Google Apps Script esté correctamente configurado y disponible. Conviene realizar una partida de prueba y comprobar que los datos se guarden efectivamente en la planilla.

La contraseña del panel docente está escrita en el código del lado del navegador. Por eso, funciona como una barrera básica, pero no como un sistema de autenticación seguro. Si se usan datos personales reales o el sitio queda disponible públicamente, se recomienda implementar la validación del acceso del lado del servidor y revisar los permisos de la hoja de cálculo.
Propósito educativo
El juego puede utilizarse como instancia de práctica y evaluación formativa después de trabajar los conceptos geométricos. El registro de resultados ayuda a identificar niveles que generan dificultades y a preparar una puesta en común sobre las estrategias, los errores y los procedimientos utilizados.

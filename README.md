# ProyectoPracticas
<h2>Mi proyecto de prácticas profesionales de Ingeniería de Sistemas</h2>
<p>Me complace presentar mi proyecto de practicas profesionales del programa de ingeniería de sistemas de la universidad Simón Bolívar de Barranquilla, Colombia. 
El nombre del proyecto es “Desarrollo del soporte gráfico y analítico para los documentos de autoevaluación de la Maestría en Salud Pública”, el cual consistió en representar gráficamente las respuestas de estudiantes, profesores y administrativos a las encuestas de autoevaluación de dicho programa. Para esto tuve que llevar a cabo varias acciones explicadas a continuación.</p>
<h3>Parte 1: Agrupación de preguntas por componentes</h3>
<p>En un archivo Excel, se elaboró una matriz con cuatro columnas: Componentes (los temas a los que van enfocadas las preguntas, ej: infraestructura, recursos humanos), Estudiantes, Profesores, Administrativos. En las filas iban las preguntas para cada uno de los actores.<br>
<b>NOTA:</b> A pesar de que cada actor tenía su encuesta, había muchas preguntas que todos o solo dos de los actores tenían en común.</p>


![](https://github.com/user-attachments/assets/b30993f5-3fa7-4e2a-b083-6ba868a03c02)

<h3>Parte 2: Creación de base de datos</h3>
<p>Se creó una base de datos preliminar en Excel, siete hojas, equivalente a siete tablas: actores, componentes, preguntas, resp_estudiantes, resp_profesores, resp_admin, respuestas_todos. Esto con el fin de revisar si no había errores. 
Después de verificar que todo estaba bien, se creó la base de datos oficial en MySQL con PHPMyAdmin convirtiendo el Excel a CSV y migrándolo a MySQL.
</p>

![image](https://github.com/user-attachments/assets/033cc824-72da-4567-96af-9cbf1edb6c7f)

<h3>Parte 3: Creación de Dashboard</h3>
<p>Se conectó la base de datos con Power BI, y se realizó el siguiente dashboard que se compone de varias páginas:
</p>
<h4>Preguntas (primera parte)</h4>

![image](https://github.com/user-attachments/assets/84714215-faec-414a-87cf-02ce81754bb4)

<h4>Preguntas (segunda parte)</h4>

![image](https://github.com/user-attachments/assets/c8696d92-4047-420b-9556-4bec6318e5d4)

Se identificó un total de 315 preguntas (1) entre los tres actores involucrados en este proceso (2) y 29 componentes para todos los cuestionarios (3). De estos 29, a los profesores se les pregunta por 26, a los estudiantes por 22 y a los administrativos por 21 (4).
Los componentes con mayor cantidad de preguntas para todos los actores son Sistema de Información Universidad, Infraestructura, Currículo, Bienestar Institucional y Recursos Tecnológicos (5). Las preguntas pueden visualizarse en (6).
Por otra parte, se identificaron tres categorías para estos componentes: Componentes compartidos por todos los actores (7), Componentes compartidos por dos de los actores y Componentes individuales para cada actor (8).
<h4>Respuestas de Actores</h4>
Se adjuntan los dashboards de las respuestas a las preguntas de los cuestionarios del proceso de autoevaluación de la Maestría en Salud Pública para cada actor involucrado.

<h5>Profesores</h5>

![image](https://github.com/user-attachments/assets/dd39a7c5-dfad-45b9-8fee-5196508226d4)

En 2024-2, en la Maestría en Salud Pública había 11 profesores (9), su encuesta de autoevaluación constaba de 122 preguntas (10), por ende las respuestas fueron 1342 en total, producto de 11 por 122 (11). Los componentes a evaluar por los profesores fueron 26 (12). Se cuenta con un gráfico circular el cual ayuda a reflejar los resultados por cada opción (Totalmente de acuerdo, De acuerdo, No sabe / no tiene información, En desacuerdo, Totalmente en desacuerdo) (13). A su lado hay una tarjeta la cual ayuda a la mejor visualización de la pregunta actualmente seleccionada (14) de las que están en la tabla inferior (15).
Nota: para Estudiantes y Administrativos se continúa con la misma guía de los numerales anteriores.

<h5>Estudiantes</h5>

![image](https://github.com/user-attachments/assets/0758a6bb-d9da-40ab-90cd-01de0b872a08)

En 2024-2, en la Maestría en Salud Pública había 11 estudiantes (9), su encuesta de autoevaluación constaba de 102 preguntas (10), por ende las respuestas fueron 1122 en total, producto de 11 por 102 (11). Los componentes a evaluar por los estudiantes fueron 22 (12). Se cuenta con un gráfico circular el cual ayuda a reflejar los resultados por cada opción (Totalmente de acuerdo, De acuerdo, No sabe / no tiene información, En desacuerdo, Totalmente en desacuerdo) (13). A su lado hay una tarjeta la cual ayuda a la mejor visualización de la pregunta actualmente seleccionada (14) de las que están en la tabla inferior (15).
<h5>Administrativos</h5>

![image](https://github.com/user-attachments/assets/ed38ec70-f633-402a-a7e7-0689545a0932)

En la Maestría en Salud Pública hay 1 administrativo, quien es la directora (9), su encuesta de autoevaluación constaba de 91 preguntas (10), por ende las respuestas fueron 91 en total, producto de 91 por 1 (11). Los componentes a evaluar por la directora fueron 21 (12). Se cuenta con un gráfico circular el cual ayuda a reflejar los resultados por cada opción (Totalmente de acuerdo, De acuerdo, No sabe / no tiene información, En desacuerdo, Totalmente en desacuerdo) (13). A su lado hay una tarjeta la cual ayuda a la mejor visualización de la pregunta actualmente seleccionada (14) de las que están en la tabla inferior (15).

<h5>Respuestas (común)</h5>

![image](https://github.com/user-attachments/assets/74a2c2ba-f662-4900-a1e2-53a40d548d63)

Esta es una vista común para las respuestas de todos los actores. Se muestra el número total de actores, para efectos de este ejemplo, los profesores (16), de acuerdo con el seleccionado en el filtro (17). Se listan los componentes de todos los actores (18) y seleccionado uno de ellos, se puede escoger una pregunta de ese componente en la tabla inferior (19). Para mejor visualización de la pregunta seleccionada, esta se mostrará en la tarjeta al lado del gráfico circular (20) y en este, aparecerán los resultados de cada una de las opciones del cuestionario de autoevaluación (21).

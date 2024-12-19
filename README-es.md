- # Literalura - Desafío Back-end del Programa ONE

  ## Descripción del proyecto

  Literalura es una implementación de un catálogo de libros basada en datos de la API Gutendex. El objetivo es practicar el consumo de APIs en proyectos Spring, junto con la persistencia de datos en una base de datos relacional.

  Nos centramos en la creación y consulta de libros y autores, parte esencial del CRUD (*Create, Read, Update and Delete*) en proyectos de *backend*.

  Decidimos no enfocarnos en la actualización/eliminación de datos, ya que este desafío representa el primer contacto práctico de los estudiantes con Spring en la especialización de *backend*.

  ### Curso del desafío

  Para más información sobre el Foro Hub, accede al [curso del desafío](https://app.aluracursos.com/course/challenge-spring-boot-literalura), que también incluye el tablero de Trello del desafío.

  ## Estructura del proyecto

  Este proyecto se enfoca en la implementación de entidades relacionadas con libros y autores, recibidas mediante solicitudes a la API.

  La API Gutendex es gratuita, no es necesario crear una cuenta ni generar una clave API, solo usar las URL disponibles para las solicitudes. Más información en el sitio oficial de Gutendex: https://gutendex.com/

  Esta aplicación consume la API Gutendex y utiliza una base de datos local PostgreSQL, con algunas funcionalidades vistas en la formación de Java y Spring Boot, especialmente en los dos primeros cursos de la especialización.

  En esta implementación, también trabajamos la persistencia de datos en una base de datos relacional llamada PostgreSQL, centrándonos únicamente en la construcción de dos entidades relacionadas: libros y autores.

  ## Tecnologías utilizadas

  - Java - versión 17: https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html
  - Maven - versión 4.0.0
  - Spring - versión 3.2.5: https://start.spring.io/
  - PostgreSQL- versión 17.2: https://www.postgresql.org/download/
  - Intellij Community (opcional): https://www.jetbrains.com/idea/download

  ### Dependencias de Spring usadas:

  - Lombok
  - Spring Web
  - Spring Boot DevTools
  - Spring Data JPA
  - PostgreSQL Driver

  ## Cómo ejecutar el proyecto

  Para ejecutar este proyecto localmente, basta con crear el archivo .jar del proyecto Java. A continuación se detallan métodos comunes para generar un archivo JAR (Java Archive), según las herramientas y entornos de desarrollo utilizados.

  ### **Usando la Línea de Comandos (javac y jar)**

  1. **Compila tu código:** Navega al directorio donde se encuentra tu código fuente y compila los archivos .java a .class usando el comando `javac`:

  ```bash
  javac -d out src/com/tuProyecto/*.java  
  ```

  En este ejemplo, los archivos .java están en la carpeta `src/com/tuProyecto`, y los archivos .class generados se colocarán en la carpeta `out`.

  1. **Crea el archivo JAR:** Utiliza el comando `jar` para crear el archivo JAR a partir de los archivos .class compilados:

  ```bash
  jar cvf miProyecto.jar -C out .  
  ```

  Este comando crea un archivo JAR llamado `miProyecto.jar`, que contiene todos los archivos .class del directorio `out`.

  ### **Usando Eclipse**

  1. Exportar como JAR:
     - Haz clic derecho en el proyecto en la pestaña **Project Explorer**.
     - Selecciona **Export** y luego **Java > JAR file**.
     - Elige los recursos a exportar y la ubicación donde guardar el archivo JAR.
     - Configura las opciones de exportación según sea necesario y haz clic en **Finish**.

  ### **Usando IntelliJ IDEA**

  1. **Crear Artefacto:**
     - Ve a **File > Project Structure**.
     - En la pestaña **Artifacts**, haz clic en **+** y selecciona **JAR > From modules with dependencies**.
     - Elige el módulo principal de tu proyecto y configura las opciones según sea necesario.
     - Haz clic en **OK** y luego en **Apply**.
  2. **Construir el Artefacto:**
     - Ve a **Build > Build Artifacts** y selecciona el artefacto creado.
     - Haz clic en **Build** para generar el archivo JAR.

  También puedes agregar herramientas de construcción como **Maven** y **Gradle** al proyecto para generar el archivo .jar usando estas herramientas.

  ## Autores

  - **Instructor Eric Monné:** https://www.linkedin.com/in/ericmonnefo/
  - **Monitora Brenda Souza:** https://www.linkedin.com/in/breudes/

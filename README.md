# G7 Alura Proyecto

**G7 Alura Proyecto** es una aplicación desarrollada con **Spring Boot** que permite gestionar información sobre libros y facilitar su administración a través de una API REST. Este proyecto está diseñado como una solución escalable y moderna utilizando tecnologías robustas como **Spring Boot**, **JPA/Hibernate** y **PostgreSQL**.

---

## Características

- **Gestión de Libros**: Crear, leer, actualizar y eliminar información de libros.
- **API REST**: Endpoints organizados y optimizados para el manejo de datos.
- **Base de Datos Relacional**: Persistencia de datos utilizando PostgreSQL.
- **Arquitectura Modular**: Organización clara en controladores, servicios, repositorios y modelos.
- **Escalabilidad**: Preparado para integrar nuevas funcionalidades.

---

## Tecnologías Utilizadas

- **Java 17**
- **Spring Boot 3.x**
- **JPA/Hibernate**
- **PostgreSQL**
- **Maven**

---

## Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

1. [Java 17 o superior](https://www.oracle.com/java/technologies/javase-downloads.html)
2. [PostgreSQL](https://www.postgresql.org/download/)
3. [Maven](https://maven.apache.org/download.cgi)
4. [Git](https://git-scm.com/)

---

## Configuración Inicial

### Clonar el Repositorio

```bash
git clone https://github.com/tu-usuario/g7-alura-proyecto.git
cd g7-alura-proyecto

Configurar Base de Datos

    Crear una base de datos en PostgreSQL:

CREATE DATABASE g7_alura;

Configurar las credenciales en el archivo application.properties:

    spring.datasource.url=jdbc:postgresql://localhost:5432/g7_alura
    spring.datasource.username=tu_usuario
    spring.datasource.password=tu_contraseña
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

Ejecutar la Aplicación

    Compilar y ejecutar:

    mvn spring-boot:run

    La aplicación estará disponible en http://localhost:8080.

Estructura del Proyecto

src/
├── main/
│   ├── java/com/alura/literalura/
│   │   ├── controller/    # Controladores REST
│   │   ├── model/         # Entidades JPA
│   │   ├── repository/    # Interfaces de acceso a la base de datos
│   │   └── service/       # Lógica de negocio
│   ├── resources/
│       ├── application.properties  # Configuración de la aplicación
│       └── static/                 # Archivos estáticos (si aplica)
└── test/
    └── java/com/alura/literalura/  # Pruebas unitarias

Endpoints Disponibles
Libros
Método	Endpoint	Descripción
GET	/api/libros	Listar todos los libros
POST	/api/libros	Crear un nuevo libro
GET	/api/libros/{id}	Obtener un libro por ID
PUT	/api/libros/{id}	Actualizar un libro existente
DELETE	/api/libros/{id}	Eliminar un libro por ID
Contribución

¡Contribuciones son bienvenidas! Por favor sigue estos pasos:

    Haz un fork del proyecto.
    Crea una rama nueva para tus cambios:

git checkout -b feature/nueva-funcionalidad

Realiza tus cambios y haz commit:

git commit -m "Añadida nueva funcionalidad"

Envía los cambios:

    git push origin feature/nueva-funcionalidad

    Abre un Pull Request en el repositorio original.

Autor

Atsotomayor
Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo LICENSE para más detalles.



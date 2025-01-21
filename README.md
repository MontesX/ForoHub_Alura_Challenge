# ForoHub - Creación y manipulación de tópicos

ForoHub es una plataforma  diseñada para crear, gestionar y participar en foros de temas educativos. El proyecto tiene 
la implementacion de registro de usuarios, tópicos y respuestas. Así como la manipulación
de dichos datos. Almacena ésta información en una base de datos y tienes acceso a ella mediante plataformas como Insomnia.

---

## **Contenido**
1. [Capacidades](#capacidades)
2. [Estructura del Sistema](#estructura)
3. [Tecnologías](#tecnologías)
4. [Configuración y Uso](#configuración-e-instalación)
5. [Endpoints](#endpoints-principales)
6. [Agradecimientos y créditos](#agradecimientos-y-créditos)
7. [Autor](#autor)

---

## **Capacidades**
- **Gestión de Usuarios**: Autenticación y autorización con JWT.
- **Gestión de Foros**: Creación y visualización de temas y respuestas.
- **Gestión de Cursos**: Asociación de cursos con temas y categorías.
- **Documentación de la API**: Generada con Swagger.
- **Seguridad**: Implementación de roles y permisos con Spring Security.

---

## **Estructura**
El proyecto está diseñado con una arquitectura por capas:
- **Capa API**: Contiene los controladores REST y configuraciones de seguridad.
- **Capa de Dominio**: Define las entidades, repositorios y DTOs.
- **Capa de Infraestructura**: Incluye configuración de base de datos, manejo de errores y documentación de API.


---

## **Tecnologías**
- **Lenguaje**: Java 17
- **Framework Principal**: Spring Boot
- **Seguridad**: Spring Security, JWT
- **Acceso a Datos**: Spring Data JPA, Hibernate
- **Base de Datos**: MySQL
- **Documentación**: SpringDoc OpenAPI (Swagger)

---

## **Configuración e Instalación**

### **Prerrequisitos**
- JDK 17
- Maven 3.8+
- MySQL Workbench 8.0+

### **Pasos**
1. Clonar el repositorio:
   ```bash
   git clone https://github.com/MontesX/ForoHub_Alura_Challenge.git
   cd forohub
   ```
2. Configuración de base de datos:
   - Crear una base de datos en MySQL Workbench.
   - Actualizar las credenciales en el archivo `application.properties`:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/forohub
     spring.datasource.username=tu_usuario
     spring.datasource.password=tu_contraseña
     ```
3. Compilar y ejecutar la aplicación:
   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

## **Algunos de los endpoints**

| Método | Endpoint         | Descripción                        |
|--------|------------------|------------------------------------|
| POST   | `/login`         | Loguear un usuario.                |
| GET    | `/usuarios`      | Obtener lista de usuarios.         |
| GET    | `/topicos`       | Listar todos los temas.            |
| POST   | `/topicos`       | Crear un nuevo tema.               |
| GET    | `/cursos`        | Listar todos los cursos.           |
| POST   | `/respuestas`    | Publicar una respuesta en un tema. |
| DEL    | `/usuarios`      | Desactiva a un usuario.            |
| PUT    | `/respuestas/id` | Actualiza una respuesta            |

---

## **Agradecimientos y créditos**

Con total agradecimiento a mis tutores:
Por brindarnos su tiempo, su atención, y hacer posible ésta formación en progreso. ¡Muchas gracias!
- [Oracle](https://www.oracle.com/ar/education/oracle-next-education/)
- [Alura Latam](https://app.aluracursos.com/form-one/registro/latam-general)

---
## **Autor**

Desarrollado por Paul Montes.

Contacto:

- [LinkedIn](https://www.linkedin.com/in/montessx/)


# Recursos Humanos - Spring Boot + Frontend

Este proyecto implementa un **sistema de gestión de empleados** con un backend en **Java Spring Boot** y un frontend en **JavaScript (React)**.  
El sistema permite administrar empleados con operaciones CRUD (crear, listar, actualizar y eliminar).

---

## 🚀 Tecnologías utilizadas

### Backend (Java - Spring Boot)
- **Java 24+**
- **Spring Boot** (framework principal)
- **Spring Web** (exposición de APIs REST)
- **Spring Data JPA + Hibernate** (persistencia de datos)
- **Maven** (gestión de dependencias y build)
- **Logback** (logging y manejo de logs)
- **Arquitectura MVC**
  - **Controladores (Controller)** → reciben peticiones HTTP.
  - **Servicios (Service Layer)** → contienen la lógica de negocio.
  - **Repositorios (Repository Pattern)** → acceso a base de datos.
  - **Modelos (Entities)** → representación de las tablas en BD.
- **Excepciones personalizadas** → manejo de errores claros y centralizados.

### Frontend
- **JavaScript / React**
- **Axios / Fetch** para consumo de la API
- **Bootstrap** 
- **Node.js + npm** para gestión de dependencias

- 1. Abrir el proyecto en **IntelliJ IDEA**.
2. Compilar con Maven:
   mvn clean install

3. Ejecutar la aplicación: mvn spring-boot:run
4. El backend se levanta en: http://localhost:8080
5. Ir a la carpeta del frontend: cd recursos-humanos-app
6. Instalar dependencias: npm install
7. Correr el servidor de desarrollo: npm start
8. El frontend estará disponible en: http://localhost:3000

⚠️ Nota: El frontend consume el backend en http://localhost:8080/rh-app/empleados

🌐 Endpoints principales (Backend)

GET /rh-app/empleados → Listar empleados

GET /rh-app/empleados/{id} → Obtener empleado por ID

POST /rh-app/empleados → Crear empleado

PUT /rh-app/empleados/{id} → Actualizar empleado

DELETE /rh-app/empleados/{id} → Eliminar empleado

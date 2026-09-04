# Microservicio Evaluación DevOps (Spring Boot)

## 1. Estrategia de Ramificación
Utilizamos **GitFlow**. Esta estrategia nos permite mantener un código estable en la rama `main`, mientras integramos continuamente nuevas características en `develop`. Las ramas `feature/` nos permiten trabajar de forma aislada sin afectar el entorno de pruebas, y las ramas `hotfix/` garantizan una respuesta rápida ante incidentes en producción.

## 2. Convenciones y Buenas Prácticas
* **Ramas:** 
  * `main` (Producción)
  * `develop` (Integración)
  * `feature/<nombre>` (Nuevas funcionalidades)
  * `hotfix/<nombre>` (Parches críticos)
* **Commits:** Uso de Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`).
* **Flujo:** Todo código llega a `main` o `develop` exclusivamente a través de Pull Requests.

## 3. Comandos Locales (Maven)
```bash
# Ejecutar pruebas
mvn clean test

# Levantar microservicio
mvn spring-boot:run
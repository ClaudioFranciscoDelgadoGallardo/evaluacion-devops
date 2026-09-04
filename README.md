# Microservicio Evaluación DevOps (Spring Boot)

## 1. Estrategia de Ramificación
Utilizamos **GitFlow**. Esta estrategia nos permite mantener un código estable en la rama main, mientras integramos continuamente nuevas características en develop. Las ramas feature/ nos permiten trabajar de forma aislada, y las ramas hotfix/ garantizan una respuesta rápida ante incidentes en producción.

## 2. Convenciones y Buenas Prácticas
* **Ramas:** 
  * main (Producción)
  * develop (Integración)
  * feature/<nombre> (Nuevas funcionalidades)
  * hotfix/<nombre> (Parches críticos)
* **Commits:** Uso de Conventional Commits (feat:, fix:, docs:, chore:).
* **Flujo:** Todo código llega a main o develop exclusivamente a través de Pull Requests.

## 3. Reflexión Individual
- **Claudio Delgado:** (Aquí redactarás tu aprendizaje sobre la implementación de GitFlow y CI/CD en la nube para automatizar procesos).

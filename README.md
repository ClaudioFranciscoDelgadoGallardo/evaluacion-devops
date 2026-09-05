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
* **Integración Continua:** El pipeline automatizado ejecuta pruebas en cada push a develop y PR a main.

## 3. Reflexión Individual
- **Claudio Delgado:** Durante el desarrollo de este encargo, comprobé que gestionar código en la nube requiere protocolos tan estrictos como los que se aplican al mantener una red de incendios en terreno. La implementación de GitFlow me enseñó la importancia de nunca alterar la rama de producción (main) de forma directa. Aislar cada parche urgente en ramas como hotfix actúa como una medida de contención. Además, la automatización mediante GitHub Actions cambió mi perspectiva sobre el control de calidad: el pipeline funciona como un panel de detección temprana. Así como un módulo alerta de un cortocircuito antes de que escale, el flujo CI/CD nos advirtió de errores de compilación al instante, reduciendo el riesgo y asegurando la estabilidad.
"@

# **Capítulo VII: DevOps Practices**
## 7.1. Continuous Integration
### 7.1.1. Tools and Practices.
La integración continua es una estrategia en el desarrollo de software la cuallos desarrolladores utilizan para fusionar sus cambios de código con la ramamain muchas veces al día. Esto desencadena una secuencia automatizadade compilación y pruebas que se completa de manera muy rápida. Este enfoque busca asegurar un proceso de desarrollo predecible y confiable, conequipos capaces de detectar y solucionar rápidamente cualquier problema decompilación. En la competencia tecnológica, las empresas utilizan laintegración continua para agilizar la introducción de nuevas características,acelerar la corrección de errores y reducir el tiempo de lanzamiento al mercado de sus productos. Es crucial que todos los desarrolladores involucrados en el proyecto se comprometan con esta práctica, tomando medidas inmediatas para solucionar cualquier inconveniente que surja.
### 7.1.2. Build & Test Suite Pipeline Components.

![Build & Test Suite Pipeline Components](assets/img/BuildTestPipelineComponents.png)

## 7.2 Continuous Delivery

### 7.2.1 Tools and Practices
La entrega continua (CD) se refiere al proceso de garantizar que los cambios en el código estén listos para ser lanzados a producción después de pasar por una serie de pruebas automatizadas.

- **Herramientas principales:**
  - **GitHub Actions, Jenkins y GitLab CI/CD:** Utilizados para construir pipelines que gestionen las pruebas, despliegues, y aprobaciones manuales necesarias antes de la implementación en producción.
  - **Spinnaker:** Herramienta de entrega continua desarrollada por Netflix, que facilita la creación y gestión de pipelines de despliegue.
  - **Argo CD:** Herramienta de despliegue continuo para Kubernetes.
  
- **Prácticas comunes:**
  - **Branching Strategy:** Usar estrategias de ramificación como GitFlow para gestionar cambios.
  - **Test Automatizados en Múltiples Entornos:** Ejecutar pruebas en entornos de staging y producción para validar el comportamiento del sistema.
  - **Aprobaciones Manuales:** Contar con una última fase de aprobación manual antes del despliegue en producción.

### 7.2.2 Stages Deployment Pipeline Components
Un pipeline de entrega continua suele incluir las siguientes etapas:

- **Test Stage:** 
  - **Pruebas Unitarias:** Valida cada componente del código.
  - **Pruebas de Aceptación:** Ejecutadas mediante herramientas como **Selenium** para simular el comportamiento del usuario.
- **Staging Environment:** Un entorno lo más parecido a producción. Herramientas como **Docker** y **Kubernetes** ayudan a orquestar contenedores y asegurar la portabilidad de las aplicaciones.
- **Deployment Stage:** Automatización del despliegue usando **GitHub Actions** o **GitLab CI/CD**.
- **Release Stage:** Monitorización continua usando herramientas como **New Relic** o **Prometheus** para identificar problemas en tiempo real.
- **Rollback and Recovery:** **MySQL** se utiliza para hacer respaldos de datos, y Git maneja las versiones de código.
- **Release Management:** Herramientas de control de versiones como **Git** o **GitHub** gestionan versiones y revisiones.

## 7.3 Continuous Deployment

### 7.3.1 Tools and Practices
La implementación continua lleva la entrega continua un paso más allá, desplegando automáticamente cada cambio aprobado en producción.

- **Herramientas principales:**
  - **Jenkins y GitLab CI/CD:** Para automatizar todo el pipeline de despliegue en producción.
  - **AWS CodePipeline y Google Cloud Build:** Herramientas específicas de CI/CD de proveedores de la nube.
  - **Octopus Deploy:** Para gestionar despliegues en múltiples entornos.
  
- **Prácticas comunes:**
  - **Branching Strategy:** GitFlow u otras estrategias de branching que faciliten la integración y despliegue de código.
  - **Canary Releases y Blue-Green Deployments:** Técnicas de despliegue que minimizan el impacto de cambios en el entorno de producción.
  - **Rollbacks Automáticos:** Configurar la capacidad de revertir despliegues en caso de fallos críticos.

### 7.3.2 Production Deployment Pipeline Components
El pipeline de despliegue en producción incluye:

- **Source Control Management:** Git permite gestionar cambios y versiones de manera organizada.
- **Build and Compilation:** Usando herramientas como **builder de Angular** para frontend o **Gradle** y **Maven** para backend.
- **Artifact Repository:** Repositorios como **Nexus** o **Artifactory** guardan artefactos compilados y aseguran la trazabilidad del código en producción.

## 7.4 Continuous Monitoring

### 7.4.1 Tools and Practices
El monitoreo continuo permite analizar el comportamiento de los sistemas en producción en tiempo real, lo cual ayuda a identificar y resolver problemas rápidamente.

- **Herramientas principales:**
  - **Prometheus y Grafana:** Prometheus se utiliza para recopilar métricas y Grafana para visualizarlas.
  - **New Relic y Dynatrace:** Herramientas avanzadas para monitorear rendimiento y detectar anomalías.
  - **ELK Stack (Elasticsearch, Logstash, Kibana):** Solución de administración de registros que ayuda a visualizar y analizar logs de aplicaciones.
  
- **Prácticas comunes:**
  - **Log Aggregation:** Centralizar los registros de aplicación y sistema.
  - **Alert Thresholds:** Configuración de umbrales para detectar cuando el rendimiento se ve afectado.
  - **Response Time Monitoring:** Monitorear el tiempo de respuesta de los servicios críticos.

### 7.4.2 Monitoring Pipeline Components
El pipeline de monitoreo incluye:

- **Metric Collection:** Recopilación de métricas de CPU, memoria, y otras estadísticas de recursos con herramientas como **Prometheus**.
- **Logs Management:** Uso de **ELK Stack** para centralizar y analizar logs, permitiendo la detección rápida de problemas.
- **Dashboarding:** Visualización de datos en **Grafana** o **Kibana** para monitorear en tiempo real.

### 7.4.3 Alerting Pipeline Components
- **Alerting:** Configuración de alertas con herramientas como **Grafana** o **PagerDuty**. Estas alertas notifican al equipo sobre eventos críticos basados en métricas predeterminadas, como el uso excesivo de CPU o caídas de servicio.
- **Alert Escalation Policies:** Configurar políticas de escalación para que si un problema no es atendido rápidamente, se alerte a los niveles superiores del equipo.

### 7.4.4 Notification Pipeline Components
- **Notification:** Integración con plataformas de comunicación como **Slack**, **Microsoft Teams** o **email** para enviar notificaciones a los equipos de desarrollo cuando ocurren eventos críticos. Esto garantiza que las alertas lleguen a las personas adecuadas.
- **Automated Incident Tracking:** Registro automatizado de incidentes en herramientas de gestión de proyectos como **Jira** para facilitar el seguimiento y resolución de problemas.

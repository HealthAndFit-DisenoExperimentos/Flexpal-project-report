# **Capítulo VII: DevOps Practices**
## 7.1. Continuous Integration
### 7.1.1. Tools and Practices.
La integración continua es una estrategia en el desarrollo de software la cuallos desarrolladores utilizan para fusionar sus cambios de código con la ramamain muchas veces al día. Esto desencadena una secuencia automatizadade compilación y pruebas que se completa de manera muy rápida. Este enfoque busca asegurar un proceso de desarrollo predecible y confiable, conequipos capaces de detectar y solucionar rápidamente cualquier problema decompilación. En la competencia tecnológica, las empresas utilizan laintegración continua para agilizar la introducción de nuevas características,acelerar la corrección de errores y reducir el tiempo de lanzamiento al mercado de sus productos. Es crucial que todos los desarrolladores involucrados en el proyecto se comprometan con esta práctica, tomando medidas inmediatas para solucionar cualquier inconveniente que surja.
### 7.1.2. Build & Test Suite Pipeline Components.

![Build & Test Suite Pipeline Components](assets/img/BuildTestPipelineComponents.png)

## 7.2 Continuous Delivery

### 7.2.1 Tools and Practices
En la entrega continua, el código pasa por un pipeline de pruebas, y una vez aprobado, está listo para ser lanzado a producción bajo aprobación manual. Las herramientas incluyen **GitHub Actions, Jenkins, GitLab CI**, y **Spinnaker** para automatizar los pipelines de entrega.

### 7.2.2 Stages Deployment Pipeline Components
- **Test Stage:** Pruebas de unidad (con **JUnit, Mockito**) y pruebas de aceptación automatizadas (ej. **Selenium**).
- **Staging Environment:** Con herramientas como **Docker** y **Kubernetes** para orquestar contenedores.
- **Deployment Stage:** Automatización mediante **GitHub Actions**.
- **Release Stage:** Monitoreo continuo de rendimiento usando **New Relic** o **Prometheus**.
- **Rollback and Recovery:** Sistema de backup y restauración con **MySQL** y gestión de versiones mediante **Git**.

## 7.3 Continuous Deployment

### 7.3.1 Tools and Practices
La implementación continua (CD) se realiza mediante herramientas que automatizan la entrega de código en producción. **Jenkins** o **GitLab CI/CD** son útiles aquí, junto con prácticas como el uso de ramas de Git (ej. **Gitflow**) para gestionar cambios y evitar errores en producción.

### 7.3.2 Production Deployment Pipeline Components
- **Source Control Management:** Git para mantener el historial de cambios.
- **Build and Compilation:** Usa herramientas como el **builder de Angular**.
- **Artifact Repository:** Guarda artefactos compilados con **Maven Central**.

## 7.4 Continuous Monitoring

### 7.4.1 Tools and Practices
Herramientas de monitoreo como **Prometheus, Grafana** y **New Relic** permiten monitorear el rendimiento en tiempo real, capturando métricas de aplicaciones y sistemas. Estas herramientas identifican problemas de rendimiento y estabilidad antes de que afecten a los usuarios.

### 7.4.2 Monitoring Pipeline Components
Los componentes incluyen:
- **Metric Collection:** Recopilación de métricas en tiempo real mediante **Prometheus** o **Datadog**.
- **Logs Management:** **ELK Stack (ElasticSearch, Logstash, Kibana)** para gestionar y visualizar logs.

### 7.4.3 Alerting Pipeline Components
- **Alerting:** Configuración de alertas con **Grafana** o **PagerDuty** para notificar a los equipos de incidentes críticos. Las alertas se configuran con umbrales específicos para detectar anomalías en el rendimiento, errores del sistema y otros eventos críticos que requieren atención inmediata.

### 7.4.4 Notification Pipeline Components
- **Notification:** Integración con **Slack** o **email** para enviar notificaciones a los equipos de desarrollo en caso de errores críticos o caídas en el sistema. Este componente asegura que los mensajes de alerta lleguen de manera rápida y eficaz a los responsables, permitiendo una respuesta oportuna.

## Avance de Conclusiones, Bibliografía y Anexos.
### Conclusiones
- Durante el desarrollo de la Landing Page, el equipo de FlexPal ha logrado implementar con éxito las funcionalidades y características planificadas, proporcionando una experiencia de usuario sólida y coherente.
- La implementación de la Landing Page ha permitido al equipo demostrar su capacidad para traducir los requisitos y especificaciones en código funcional, desarrollando una estructura sólida y un diseño visual atractivo.
- La colaboración y el trabajo en equipo han sido fundamentales para el éxito del proyecto, permitiendo a los miembros del equipo compartir conocimientos, habilidades y recursos para lograr los objetivos establecidos.
- La implementación de la Landing Page ha sentado las bases para el desarrollo de la Web Application, que se espera completar en etapas posteriores del proyecto.
- El uso de herramientas de gestión de proyectos como Trello y GitHub ha facilitado la planificación, el seguimiento y la colaboración en el desarrollo del proyecto, permitiendo al equipo mantenerse organizado y enfocado en los objetivos.
- El proceso de desarrollo ágil ha demostrado ser efectivo para la implementación de la Landing Page, permitiendo al equipo adaptarse a los cambios y desafíos de manera eficiente y eficaz.

### Anexos
- Anexo 1: [Organización en GitHub](https://github.com/los-seniors-v2)
- Anexo 2: [Mockups - Wireframe](https://www.figma.com/file/91Ez19KOQpxgpmPEZ9NtIm/FlexPal?type=design&node-id=0%3A1&mode=design&t=vgM82K5YOfavEdYS-1)
- Anexo 3: [User-Flow - WireFlow Diagram](https://lucid.app/lucidspark/2c642c76-fe1b-41c2-a0e3-613a0b64f8f0/edit?viewport_loc=-1797%2C-1394%2C8704%2C4350%2C0_0&invitationId=inv_0f96f168-1b85-4920-a9fb-ce76f2b42015)
- Anexo 4: [Netlify](https://www.netlify.com/)
- Anexo 6: [Trello](https://trello.com/)
- Anexo 7: [SmarterAsp](https://www.smarterasp.net/)

### Bibliografía
- Ipsos. (16 de octubre de 2019). Alimentación y vida saludable en Lima. Ipsos. https://www.ipsos.com/es-pe/alimentacion-y-vida-saludable-en-lima
- Aproximadamente 15 millones de peruanos sufren de obesidad. (4 de marzo de 2024). Noticias - Ministerio De Salud - Plataforma Del Estado Peruano. https://www.gob.pe/institucion/minsa/noticias/915217-aproximadamente-15-millones-de-peruanos-sufren-de-obesidad
- Mena, F. G. (10 de junio de 2019). La realidad de los gimnasios: “80% de peruanos abandona su membresía en los primeros 3 meses.” Gestión. https://gestion.pe/tendencias/realidad-gimnasios-80-peruanos-abandona-membresia-primeros-3-meses-269519-noticia/
- Ruiz, A. M. (20 de mayo de 2020). El auge del coaching deportivo: Cómo los entrenadores personales están transformando la industria del fitness. ABC. https://abc.es/auge-coaching-deportivo-entrenadores-personales-transformando-industria-fitness
- Gómez, L. J. (12 de noviembre de 2019). La capacitación de profesionales en el ejercicio físico: Clave para el éxito de los gimnasios. El Mundo. https://elmundo.es/capacitacion-profesionales-ejercicio-fisico-exito-gimnasios
- Fernández, C. R. (7 de febrero de 2021). La importancia de la nutrición en el entrenamiento personal. El País. https://elpais.com/importancia-nutricion-entrenamiento-personal
- Sánchez, P. L. (3 de agosto de 2022). Tendencias en la industria del fitness: Del entrenamiento online a la personalización. La Vanguardia. https://lavanguardia.com/tendencias-industria-fitness-entrenamiento-online-personalizacion
- Navarro, E. F. (18 de abril de 2018). Formación y certificación de entrenadores personales: Estándares y mejores prácticas. Diario AS. https://as.com/formacion-certificacion-entrenadores-personales-estandares-mejores-practicas

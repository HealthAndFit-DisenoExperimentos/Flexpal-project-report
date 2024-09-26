# **Capítulo VII: DevOps Practices**
## 7.1. Continuous Integration
### 7.1.1. Tools and Practices.
La integración continua es una estrategia en el desarrollo de software la cuallos desarrolladores utilizan para fusionar sus cambios de código con la ramamain muchas veces al día. Esto desencadena una secuencia automatizadade compilación y pruebas que se completa de manera muy rápida. Este enfoque busca asegurar un proceso de desarrollo predecible y confiable, conequipos capaces de detectar y solucionar rápidamente cualquier problema decompilación. En la competencia tecnológica, las empresas utilizan laintegración continua para agilizar la introducción de nuevas características,acelerar la corrección de errores y reducir el tiempo de lanzamiento al mercado de sus productos. Es crucial que todos los desarrolladores involucrados en el proyecto se comprometan con esta práctica, tomando medidas inmediatas para solucionar cualquier inconveniente que surja.
### 7.1.2. Build & Test Suite Pipeline Components.
## 7.2. Continuous Delivery
### 7.2.1. Tools and Practices.
Utilizamos Github como repositorio del proyecto, cuando hacemos cambios alrepositorio, un código cypress corre en el servidor y se genera un log queseñala si hubo errores o conflictos viniendo de nuevos cambios.
### 7.2.2. Stages Deployment Pipeline Components.
Test Stage:
- Marco de pruebas unitarias: Mockito
- Pruebas de integración: Mockito
- Pruebas de aceptación automatizadas:Selenium
  
Staging Environment:
- Orquestación de contenedores: Docker, Kubernetes
- Aprovisionamiento de servidores: MySql
  
Deployment Stage:
- Herramientas de despliegue continuo: GitHub CI/CD
- Release Stage:Herramientas de monitoreo y registro: New Relic.
  
Rollback and Recovery:
- Copias de seguridad y restauración: MySql105
- Gestión de versiones de código: Git.
  
Release Management:
- Herramientas de gestión de versiones: Git, GitHub.
  
## 7.3. Continuous deployment
### 7.3.1. Tools and Practices.
Para llevar a cabo el proceso de gestión de versiones en Git, utilizamos laterminal de comandos. Para facilitar la automatización del proyecto, se haceuso de la herramienta “Gitflow” que brinda una guía detallada y automatizadapara seguir el flujo. Garantizandonos una gestión más eficiente.
### 7.3.2. Production Deployment Pipeline Components.
Source Control Management: Git

Build and compilation: Builder de Angular

Artifact repository: Maven Centra

# Avance de Conclusiones
# Bibliografía 
# Anexos

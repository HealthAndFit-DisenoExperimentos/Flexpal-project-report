# **Capítulo VIII: Experiment-Driven Development**
## 8.1 Experiment Planning

En esta fase, se definirán los objetivos, hipótesis y métricas clave para los experimentos, estableciendo un plan claro para evaluar el desempeño y los resultados de la plataforma antes del lanzamiento.

### 8.1.1 As-Is Summary: Redactar un resumen del estado actual del producto.
FlexPal es una plataforma integral diseñada para optimizar la gestión de ejercicios y actividades físicas. Su propósito principal es proporcionar a los entrenadores las herramientas necesarias para gestionar sus operaciones diarias de manera eficiente, mejorar su competitividad y facilitar su crecimiento en un mercado cada vez más globalizado.

Entre sus funcionalidades destacadas se encuentran la gestión de sesiones en línea, el control de horarios, el análisis de datos en tiempo real y la comunicación con clientes a través de múltiples canales.

### 8.1.2 Raw Material: Documentar asunciones, ideas y brechas de conocimiento.
**Assumptions**
- La plataforma FlexPal debe mostrar un seguimiento detallado de los horarios de las sesiones.

**Knowlegde Gaps**
- ¿Qué tan efectiva es la herramienta de análisis de datos para las personas en sus sesiones?

**Ideas**
- Integración de inteligencia artificial, de este modo esta herramienta puede ofrecer recomendaciones más precisas y personalizadas sobre ejercicios recomendados, horario de sesiones y dietas sugeridas, basadas en el análisis de datos en tiempo real.

**Claims**
- La plataforma necesita mejorar su capacidad para manejar grandes volúmenes de datos y usuarios mientras crecen.

### 8.1.3 Experiment-Ready Questions: Formular preguntas clave para los experimentos.
- ¿Qué estrategias de marketing digital son más efectivas para aumentar la visibilidad y atraer nuevos clientes a los entrenadores que utilizan FlexPal?

### 8.1.4 Question Backlog 
Las preguntas implantadas en el “Question Backlogs” son primordiales para mejorar
nuestros servicios y las incertidumbres que necesitan ser exploradas para mejorar la
plataforma y poder tomar decisiones informadas.

- ¿Qué formatos y visualizaciones de datos son más efectivos para los reportes de resultados por sesión?

### 8.1.5 Experiment Cards
| QUESTION | ¿Los clientes tienen miedo de realizar una subscripción online porque podría ser peor que una presencial? |
|----------|----|
| WHY      | Porque la inscripción por internet es más sencilla y directa |
| WHAT     | Implementamos un sistema de garantía de servicio |
| HYPOTHESIS | Si logramos que aumenten la cantidad de usuarios que deciden hacer una subscripción online en un 10%, entonces podemos incrementar las ventas en un 5% |

## 8.2 Experiment Design
### 8.2.1 Hypotheses
<table border="1" style="text-align: center;">
	<tbody>
		<tr>
			<td colspan="2">Hipótesis 1</td>
		</tr>
		<tr>
     			<td colspan="1">Pregunta</td>
      			<td colspan="1">¿Cuántos usuarios siguen utilizando el servicio después de la primera sesión?</td> 
    		</tr>
		<tr>
     			<td colspan="1">Creencia</td>
      			<td colspan="1">Después de la primera sesión mucha gente pierde el interés de seguir utilizando el servicio de la plataforma</td> 
    		</tr>
		<tr>
     			<td colspan="1">Hipotesis (alternativa)</td>
      			<td colspan="1">Al proveer incentivos tras la primera sesión, al igual que datos sobre el rendimiento estimado, lograremos aumentar la retención de usuarios en un 20%</td> 
    		</tr>
		<tr>
     			<td colspan="1">Hipotesis (nula)</td>
      			<td colspan="1">Al proveer incentivos tras la primera sesión, al igual que datos sobre el rendimiento estimado, no lograremos aumentar la retención de usuarios en un 10%</td> 
    		</tr>
	</tbody>
</table>

### 8.2.2 Measures
| Pregunta | ¿Cuántos usuarios siguen utilizando el servicio después de la primera sesión? |
|----------|----|
| Medida      | Cnatidad de usuarios que llegan a agendar una segunda sesión dentro de un mes |

### 8.2.3 Conditions
| Pregunta | ¿Cuántos usuarios siguen utilizando el servicio después de la primera sesión? |
|----------|----|
| Condición Experimental | La cantidad de ususarios que llega a agendar una segunda sesión aumenta en un 10% |
| Condición de Control   | La cantidad de ususarios que sigue utilizando el servicio tras la segunda sesión es igual o mayor|

### 8.2.4 Scale Calculations and Decisions: Establecer condiciones y cálculos de escala.
<table border="1" style="text-align: center;">
	<tbody>
		<tr>
			<td colspan="1">Scale calculation</td>
     			<td colspan="1">Decisión</td>
      			<td colspan="4">Factor</td> 
    		</tr>
		<tr>
			<td colspan="2"></td>
			<td>Desfavorables</td>
			<td>Aceptables</td>
			<td>Ideal</td>
			<td>Excelente</td>
		</tr>
		<tr>
			<td>Creemos que implementar un descuento del 20% en la segunda sesión, además de proveer estadísticas sobre posibles resultados futuros, aumentará la cantidad de usuarios que agenden una segunda sesión en un 10%</td>
			<td>Vamos a implementar una pestaña de logros futuros basada en los datos de la sesión</td>
			<td>1%<=x<2% </td>
			<td>>=2%</td>
			<td>>=5%</td>
			<td>>=9&</td>
		</tr>
	</tbody>
</table>

### 8.2.5 Methods Selection 
Para analizar la información y los datos propuesto en nuestro proyecto, decidimos optar comparativas con algunas de las herramientas que se usan para este tipo de casos:
<table border="1" style="text-align: center;">
	<tbody>
		<tr>
			<td colspan="3">Google Analitics</td>
		<tr>
			<td colspan="1">Descripción</td>
     			<td colspan="1">Ventajas</td>
      			<td colspan="1">Desventajas</td> 
    		</tr>
		<tr>
			<td colspan="1">Una herramienta de análisis web que ofrece capacidades avanzadas para rastrear, medir y analizar el comportamiento de los usuarios en sitios web, aplicaciones móviles y otras plataformas digitales.</td>
			<td>
                <ul>
                    <li>Ofrece capacidades avanzadas de análisis web y seguimiento de usuarios.</li>
                    <li> Integración con otras soluciones de Google, como Google Ads y Google Data Studio.</li>
                    <li>Personalización y creación de informes altamente flexibles.</li>
                </ul>
            </td>
      			<td>
                <ul>
                    <li>Algunas funcionalidades avanzadas pueden requerir una cuenta premium o de pago.</li>
                    <li>Requiere implementación de código en el sitio web para rastrear datos.</li>
                </ul>
            </td>
    		</tr>
	</tbody>
</table>

<table border="1" style="text-align: center;">
	<tbody>
		<tr>
			<td colspan="3">Tableau</td>
		<tr>
			<td colspan="1">Descripción</td>
     			<td colspan="1">Ventajas</td>
      			<td colspan="1">Desventajas</td> 
    		</tr>
		<tr>
			<td colspan="1">Una herramienta de visualización de datos que ayuda a las empresas a ver y entender sus datos a través de dashboards interactivos y altamente personalizables.</td>
			<td>
                <ul>
                    <li>Capacidad para conectar y analizar datos de múltiples fuentes.</li>
                    <li>Herramientas avanzadas de visualización de datos y creación de dashboards interactivos.</li>
                    <li>Fuerte comunidad de usuarios y recursos de aprendizaje</li>
                </ul>
            </td>
      			<td>
                <ul>
                    <li>Curva de aprendizaje pronunciada para usuarios no técnicos.</li>
                    <li>Requiere una licencia de pago para acceder a todas las funcionalidades.</li>
                </ul>
            </td>
    		</tr>
	</tbody>
</table>

<table border="1" style="text-align: center;">
	<tbody>
		<tr>
			<td colspan="3">Microsoft Power BI</td>
		<tr>
			<td colspan="1">Descripción</td>
     			<td colspan="1">Ventajas</td>
      			<td colspan="1">Desventajas</td> 
    		</tr>
		<tr>
			<td colspan="1">Una herramienta de análisis de negocios que permite a los usuarios crear informes interactivos y dashboards, facilitando la toma de decisiones basada en datos.</td>
			<td>
                <ul>
                    <li>Integración con otros productos de Microsoft, como Excel y Azure.</li>
                    <li>Interfaz intuitiva y fácil de usar para la creación de informes.</li>
                    <li> Opciones de análisis de datos en tiempo real.</li>
                </ul>
            </td>
      			<td>
                <ul>
                    <li>Algunas funcionalidades avanzadas pueden requerir una suscripción de pago.</li>
                    <li>Limitaciones en la personalización de ciertos tipos de gráficos y visualizaciones.</li>
                </ul>
            </td>
    		</tr>
	</tbody>
</table>

### 8.2.6 Data Analytics: Selección de métodos y métricas de análisis.
Esta sección explica lo que se pretende lograr con el análisis de datos, cuáles son los KPIs
más relevantes para monitorear y qué métricas se utilizarán para evaluar el rendimiento de
la plataforma.

- **1. Eventos de Uso de Funcionalidades:** Estos eventos rastrearán las acciones relacionadas con el uso de las funcionalidades de FlexPal. El principal objetivo será comprender mejor cómo los entrenadores utilizan diferentes funcionalidades para mejorar su eficiencia y eficacia.
- **2. Retención de usuarios:** Se tiene pensado la evaluación sobre la retención de usuarios a lo largo del tiempo, de esta manera se podrá conocer cuántos entrenadores regresan y usan FlexPal de manera recurrente, con el objetivo de medir la fidelidad de los usuarios y evaluar la efectividad de las estrategias de retención
- **3. Tasa de crecimiento de ventas:** Implementar un monitoreo sobre el incremento en las ventas generadas por los entrenadores utilizando FlexPal, con la finalidad de evaluar el impacto de FlexPal en el crecimiento de las subscripciones y ajustar estrategias en consecuencia.
- **4. Tiempo de respuesta del sistema:** Se medirá la velocidad con la que FlexPal procesa solicitudes de carga de datos, con el objetivo de asegurar una experiencia de usuario fluida y eficiente.

### 8.2.7 Web and Mobile Tracking Plan: Planificar el seguimiento en plataformas web y móvil.
**Etapa Final: Definición del Plan de Seguimiento de Experimentos para FlexPal**

Nos enfocaremos en optimizar y monitorear la aplicación web y móvil de FlexPal para mejorar la gestión de inventarios y ventas.
Para la etapa final estableceremos un plan de seguimiento detallado para evaluar las mejoras implementadas en la aplicación.

Control General de Experimentos en FlexPal:

El control de las funcionalidades experimentales se realizará en dos etapas clave:
1. Implementación Inicial:
- Recopilación de Datos: Después de la implementación inicial, se recopilarán datos de manera continua en intervalos diarios. Esto permitirá observar cómo evolucionan las conversiones, la precisión del inventario, las tasas de ventas y verificar si las hipótesis planteadas se confirman a lo largo del tiempo.
- Análisis Comparativo: Los datos recopilados se utilizarán para medir el rendimiento y la eficacia de las nuevas funcionalidades en comparación con las métricas existentes.

3. Seguimiento Continuo:
- Recopilación de Datos: Después de la implementación inicial, se recopilarán datos de manera continua en intervalos diarios. Esto permitirá observar cómo evolucionan las conversiones, la precisión del inventario, las tasas de ventas y verificar si las hipótesis planteadas se confirman a lo largo del tiempo.
- Análisis Comparativo: Los datos recopilados se utilizarán para medir el rendimiento y la eficacia de las nuevas funcionalidades en comparación con las métricas existentes.
Evaluación Subjetiva:
- Opiniones de los Usuarios: Para obtener una apreciación subjetiva, al finalizar la etapa de experimentación, se enviará un cuestionario a cada grupo de usuarios que participó en las pruebas de las funcionalidades específicas.

Objetivos del Cuestionario:
- Recopilar opiniones y comentarios de los usuarios sobre la funcionalidad en cuestión.
- Obtener información cualitativa sobre la experiencia del usuario, la usabilidad y la satisfacción.
- Identificar problemas y áreas de mejora a partir de las experiencias de los usuarios.

Indicadores Clave de Rendimiento:
- Tasa de Conversión: Medir el porcentaje de visitas que resultan en ventas.
- Precisión del Inventario: Verificar la exactitud entre el inventario registrado y el inventario real.
- Tiempo de Procesamiento de Pedidos: Medir el tiempo desde que se realiza un pedido hasta que se procesa.
- Satisfacción del Usuario: Evaluar la satisfacción general del usuario mediante encuestas.
- Retención de Usuarios: Medir la cantidad de usuarios que vuelven a utilizar la aplicación.

Proceso de Monitoreo y Análisis:
- **1. Configuración de Herramientas de Seguimiento:** Utilizar herramientas de análisis web y móvil (como Google Analytics, Tableau, etc.) para rastrear el comportamiento del usuario y las interacciones con las nuevas funcionalidades.
- **2. Recolección de Datos:** Capturar datos sobre cómo los usuarios interactúan con las nuevas funcionalidades (clics, tiempo en página, flujo de usuario, etc.).
- **3. Análisis de Datos:** Evaluar los datos recopilados para identificar patrones y tendencias. Comparar los resultados con los objetivos establecidos.
- **4. Feedback de Usuarios:** Revisar los comentarios y sugerencias de los cuestionarios enviados a los usuarios.
- **5. Iteración y Mejora:** Basado en el análisis de datos y feedback, realizar ajustes y mejoras en las funcionalidades experimentales.
## 8.3
## 8.4. Experiment Aftermath & Analysis

Esta sección se enfoca en los resultados y aprendizajes obtenidos tras realizar el experimento. El objetivo principal es interpretar los datos recolectados y priorizar ajustes o refinamientos basados en estos resultados.

### 8.4.1. Analysis and Interpretation of Results

El análisis de los resultados obtenidos permite interpretar los datos recolectados durante el experimento y evaluar su impacto en los objetivos establecidos. Este proceso responde preguntas clave sobre el desempeño, la efectividad y las áreas de mejora identificadas:

- Identificación de lo que funcionó según lo esperado.
- Detección de aspectos que no cumplieron con las expectativas y sus posibles causas.
- Propuestas de mejoras específicas basadas en la evidencia recolectada.

La interpretación de resultados combina tanto datos cuantitativos (métricas clave, tasas de éxito, tiempos, porcentajes) como cualitativos (retroalimentación de usuarios o participantes). Posteriormente, estos datos se comparan con los objetivos iniciales del experimento para determinar el nivel de cumplimiento y los ajustes necesarios.


### 8.4.2. Re-scored and Re-prioritized Question Backlog

Una vez obtenidos y analizados los resultados, se procederá a re-priorizar el backlog de preguntas, asegurando que esté alineado con los aprendizajes del experimento. Este proceso incluye:

- Reasignación de puntajes: Se revisa cada pregunta o problema pendiente y se ajusta su relevancia en función de los 
  nuevos hallazgos. Las preguntas resueltas se eliminan o archivan, mientras que las relacionadas con áreas críticas 
  identificadas ganan prioridad.

- Priorización basada en impacto: Las preguntas que demuestran un impacto directo en los resultados esperados se 
  priorizan. Esto asegura que las áreas con mayor influencia en la experiencia del usuario o los objetivos del 
  proyecto sean abordadas primero.

- Planificación de próximos pasos: Se establecen acciones para abordar las preguntas priorizadas, como el diseño de 
  nuevos experimentos, ajustes en las implementaciones actuales o reuniones de trabajo para definir estrategias.

Este proceso garantiza un ciclo iterativo de mejora continua, centrado en resolver las áreas críticas y maximizar los resultados.

## 8.5. Continous Learning 

En este punto, se implementará un flujo de aprendizaje continuo para identificar y abordar áreas de mejora en el desarrollo, la usabilidad, y la calidad del sistema, utilizando pruebas automatizadas y retroalimentación constante de usuarios. Esto asegurará la optimización y evolución de la aplicación.

### 8.5.1 Shareback Session Artifact: Learning Workflow
Arquitectura y Tecnologías Utilizadas
Arquitectura:
- Nuestra aplicación está basada y desplegada en la nube para escalabilidad.
  
Tecnologías:
- Base de datos SQL para almacenar información de los paquetes.
- Framework web para desarrollo rápido (Angular).

Funcionalidades Clave
- Registro y Autenticación de Usuarios: Proceso seguro y fácil.
- Buy: la función que te permite guardar tus datos y pagar el servicio.

Proceso de Desarrollo
- Enfoque: Usabilidad y seguridad.
- Pruebas: Sistema de prueba continuo para identificar y abordar problemas.

Experiencia del Usuario (UX)
- Interfaz de Usuario: Intuitiva y atractiva.
- Retroalimentación: Positiva de usuarios de prueba.

Testing y Calidad
- Pruebas: Rigurosas de seguridad y rendimiento realizadas con selenium y con jenkins.

## 8.6. To-Be Software Platform Pre-launch

En esta fase, se creará un video promocional que resuma el modelo de negocio, características y beneficios del producto.

### 8.6.1. Abouth-the-Product Intro Video
 
	youtube: https://youtu.be/dNG-wDpqw_Q

## Conclusiones

- FlexApp combina tecnología y fitness, ofreciendo planes de nutrición, rutinas adaptadas y entrenadores especializados, revolucionando la experiencia fitness.

- FlexApp fue sometida a pruebas exhaustivas de código y seguridad, asegurando una plataforma estable, confiable y protegida contra vulnerabilidades.

- El desarrollo de FlexApp utilizó principios de Domain-Driven Design (DDD), asegurando que la lógica de negocio refleje fielmente las necesidades del dominio fitness, facilitando escalabilidad y flexibilidad.

- Se realizaron pruebas exhaustivas, incluyendo validaciones unitarias y de integración, garantizando un sistema robusto y alineado con las reglas del dominio fitness.

- La personalización dinámica y la adaptabilidad de FlexApp fueron posibles gracias al enfoque en casos de uso específicos del dominio, asegurando una experiencia centrada en el cliente.

- Herramientas como User Personas, Empathy Mapping, y Journey Mapping aseguran que las soluciones desarrolladas estén profundamente conectadas con las expectativas y problemas de los usuarios.

- El uso de Experiment-Driven Development y la priorización basada en hipótesis fomentan la mejora iterativa y el aprendizaje continuo, adaptando el producto a escenarios reales.

- Durante el desarrollo de la Landing Page, el equipo de FlexPal ha logrado implementar con éxito las funcionalidades y características planificadas, proporcionando una experiencia de usuario sólida y coherente.
- La implementación de la Landing Page ha permitido al equipo demostrar su capacidad para traducir los requisitos y especificaciones en código funcional, desarrollando una estructura sólida y un diseño visual atractivo.
- La colaboración y el trabajo en equipo han sido fundamentales para el éxito del proyecto, permitiendo a los miembros del equipo compartir conocimientos, habilidades y recursos para lograr los objetivos establecidos.
- La implementación de la Landing Page ha sentado las bases para el desarrollo de la Web Application, que se espera completar en etapas posteriores del proyecto.
- El uso de herramientas de gestión de proyectos como Trello y GitHub ha facilitado la planificación, el seguimiento y la colaboración en el desarrollo del proyecto, permitiendo al equipo mantenerse organizado y enfocado en los objetivos.
- El proceso de desarrollo ágil ha demostrado ser efectivo para la implementación de la Landing Page, permitiendo al equipo adaptarse a los cambios y desafíos de manera eficiente y eficaz.


## Recomendaciones

- Consideramos clave refinar los contextos delimitados existentes para garantizar que cada módulo tenga un modelo de dominio bien definido y escalable. Esto facilitará la incorporación de nuevas funcionalidades sin comprometer la arquitectura actual.

- Creemos que integrar modelos de machine learning mejorará la personalización de planes de nutrición y rutinas, permitiendo ajustes dinámicos según el progreso y las preferencias individuales de los usuarios.

- Es fundamental incrementar la cobertura de nuestras pruebas automáticas, priorizando flujos end-to-end. Además, proponemos implementar monitoreo en tiempo real para identificar y resolver incidentes proactivamente.

- Para fortalecer nuestra comunidad, sugerimos crear foros o espacios dentro de la app donde los miembros puedan compartir logros, recetas o consejos. Esto aumentará el sentido de pertenencia y la fidelidad hacia la plataforma.

- Planeamos seguir utilizando el enfoque Experiment-Driven Development para validar y priorizar características basándonos en datos. Esto garantizará que cada nuevo desarrollo aporte valor tangible a nuestros usuarios.


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

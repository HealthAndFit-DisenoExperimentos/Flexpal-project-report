 # **Capítulo VI: Product Verification & Validation**
## 6.1. Testing Suites & Validation
### 6.1.1. Core Entities Unit Tests.
Para la elaboración de los principales test de nuestra Landing Page, hemostenido en cuenta las secciones más importantes, las cuales son el 
- About Us
- Subscription
- Testimonials
- Contact Us
Gracias a la herramienta de Selenium-IDE se ha logrado realizar los test que seejecutaron en la Landing Page que se muestra a continuación.

![FlexpalLandingPage](assets/img/FlexpalLanding.jpg)

### 6.1.2. Core Integration Tests.

![unitTest1](assets/img/unitTest_1.png)
![unitTest1](assets/img/unitTest_2.png)

### 6.1.3. Core Behavior-Driven Development
Estamos inmersos en el desarrollo de un sitio web que ofrece a los usuariosla capacidad de registrarse y acceder a una base de datos. En este proceso,podemos aprovechar los principios y prácticas del Behiavor-Driven-Development(BDD) para optimizar nuestra colaboración, definir y refinar los requisitos, yautomatizar las pruebas de aceptación. Una estrategia eficaz para estructurar estaspruebas es la técnica Given-When-Then. Por ejemplo, al considerar el escenario enel cual un usuario registrado accede a la base de datos, podemos seguir esteformato:
- Dado que soy un usuario del segmento coach en Flexpal y he iniciado sesión en la aplicación.
- Cuando el administrador haga clic en el botón de generar reporte.
- Entonces el administrador recibe un reporte detallado del inventario del sistema. Este enfoque nos permite clarificar las acciones previas, la acción en símisma y los resultados esperados, facilitando así la comprensión y ejecución de laspruebas de aceptación.
### 6.1.4. Core System Tests.
Para realizar los Core System tests, se ha seleccionado usar la herramienta“Lighthouse” en el cual se han realizado evaluaciones para nuestra Landing Pagedesplegada, las evaluaciones ejecutadas, se centran en el rendimiento principal denuestra Landing Page, accesibilidad y uso, a continuación se muestran mejoresdetalles.

![CoreSystemTest](assets/img/light1.jpg)

![CoreSystemTest](assets/img/light2.jpg)

El análisis realizado muestra que la página cumple con buenos niveles en accesibilidad y SEO, lo cual es positivo para la experiencia de usuario y el posicionamiento en buscadores. Sin embargo, el rendimiento general puede mejorarse significativamente. Las principales áreas de oportunidad están en la optimización de JavaScript, la carga diferida de recursos de terceros y la optimización de imágenes.

Siguientes Pasos Recomendados
- Revisar y Optimizar el Código JavaScript: Minimiza el código y aplica técnicas de carga diferida.
- Reducir el Impacto de Recursos de Terceros: Utiliza alternativas diferidas o carga condicional.
- Optimizar el Peso y Formato de Imágenes: Convierte las imágenes a formatos como WebP y ajusta el tamaño.
- Implementar Buenas Prácticas para Mejorar el LCP y el TBT.


## 6.2. Static Testing & Verification

### 6.2.1. Static Code Analysis:

### 6.2.1.1. Coding standard & Code conventions:

En esta sección, se documentarán los estándares de codificación y las convenciones de código utilizados para el proyecto FlexApp Landing Page. El objetivo es asegurar un código legible, mantenible y consistente.

1. Estructura General del Documento HTML
Estándar W3C HTML5: Se utiliza !DOCTYPE html para indicar que el documento cumple con HTML5, lo cual es importante para la correcta interpretación del HTML en todos los navegadores.
Uso de Etiquetas HTML estándar: La estructura principal del documento sigue las pautas de HTML5, manteniendo la claridad y organización del contenido dentro de etiquetas semánticas como html, head, body, header, main, section, y footer.
Ejemplo:
<!-- 
<!DOCTYPE html> 
<html lang="en"> 
... 
</html> 
-->

2. Declaración de Metadatos
Estándar de Accesibilidad y SEO: Las etiquetas meta de description, keywords, y author mejoran la optimización para motores de búsqueda (SEO) y ayudan a proporcionar información adicional sobre el sitio.
Compatibilidad con Dispositivos Móviles: La etiqueta meta name="viewport" content="width=device-width, initial-scale=1.0" garantiza que la página sea responsiva en dispositivos móviles.
Ejemplo:
<!-- <head> -->
<!--     <meta charset="UTF-8"> -->
<!--     <meta name="viewport" content="width=device-width, initial-scale=1.0"> -->
<!--     <meta name="description" content="Explora destinos nuevos y emocionantes con nuestra agencia de viajes."> -->
<!--     <meta name="keywords" content="viajes, destinos, agencia de viajes, turismo, aventura"> -->
<!--     <meta name="author" content="UniqueTrip App"> -->
<!-- </head> -->

3. Convenciones de Nombres
Estándar de Nomenclatura BEM: Se utilizan nombres en kebab-case para clases e IDs en el CSS, siguiendo el estándar BEM (Block Element Modifier), que facilita la lectura y organización del código CSS.
Nombres Claros y Descriptivos: Cada nombre de clase e ID se elige para que represente claramente su función o contenido, mejorando la mantenibilidad y comprensión del código.
Ejemplo:
<!-- <section class="about-us" id="about-us"> -->

4. Organización de CSS
Estándar de Organización de CSS: Los archivos CSS se cargan de forma modular (primero base.css para estilos generales y luego styles.css para estilos específicos) según la práctica recomendada de separación de responsabilidades en CSS.
Optimización de Recursos: La fuente externa se carga desde un CDN de Google Fonts, siguiendo las prácticas recomendadas para mejorar el rendimiento. El uso del atributo preload es opcional y se utiliza para reducir el tiempo de carga.
Ejemplo:
<!-- <link rel="stylesheet" href="assets/base.css"> -->
<!-- <link rel="stylesheet" href="assets/styles.css"> -->
<!-- <link href="https://fonts.googleapis.com/css?family=Poppins:400,700&display=swap" rel="stylesheet" preload> -->

5. Accesibilidad (A11Y)
Estándar de Accesibilidad WCAG: Todas las imágenes tienen un atributo alt que describe su contenido. Esto ayuda a los usuarios de lectores de pantalla y mejora la accesibilidad en línea con las pautas WCAG (Web Content Accessibility Guidelines).
Etiquetas ARIA: Para mejorar la accesibilidad, se utilizan atributos aria-label en elementos interactivos para describir su función. Esto asegura que todos los usuarios puedan comprender el propósito de los elementos.
Ejemplo:
<!-- <a href="#hero" class="nav-logo" aria-label="FlexApp Logo"> -->
<!--     <img src="assets/img/Flexapp.png" alt="FlexApp Logo" height="100px"> -->
<!-- </a> -->

6. Convenciones para CSS en Línea
Estándar de Separación de Estilos: Evitar CSS en línea (inline CSS) sigue la recomendación de mantener el HTML y CSS separados para mejorar la legibilidad y reutilización de código. El uso de estilos en línea está permitido solo para casos específicos como botones en a y se minimiza en lo posible.
Ejemplo:
<!-- <a href="http://flexpal-seniors.web.app" class="nav-btn-link"> -->
<!--     <button class="nav-btn">Log In</button> -->
<!-- </a> -->

7. Comentarios en el Código
Buenas Prácticas de Documentación: Agregar comentarios al inicio de cada sección HTML para documentar su propósito. Esto es esencial para la colaboración en equipo y facilita la comprensión y mantenimiento del código.
Ejemplo:
<!-- <!-- Header --> -->
<!-- <header> -->
<!--     ... -->
<!-- </header> -->

8. Buenas Prácticas para el SEO
SEO Friendly: El uso de etiquetas de encabezado en orden jerárquico (h1, h2, h3, etc.) ayuda tanto en accesibilidad como en optimización para motores de búsqueda.
URLs Descriptivos: Los enlaces internos son relativos y se evitan enlaces vacíos (href="#") excepto en prototipos, siguiendo prácticas de SEO y UX.
Ejemplo:
<!-- <h1>Welcome to FlexApp</h1> -->
<!-- <h2>About Us</h2> -->
<!-- <a href="#destinations" class="btn-2">Discover the plans we have for you</a> -->

9. Uso de Secciones Semánticas
HTML5 Semántico: Se utilizan etiquetas HTML5 como header, main, section, footer para definir las áreas principales de la página. Esto mejora tanto la accesibilidad como la claridad estructural del documento, cumpliendo con el estándar W3C.
Ejemplo:
<!-- <main class="main"> -->
<!--     <section class="hero" id="hero"> -->
<!--         ... -->
<!--     </section> -->
<!-- </main> -->



### 6.2.1.2. Code Quality & Code Security: 

### 6.2.2 Reviews: 







## 6.3. Validation Interviews
### 6.3.1. Diseño de Entrevistas.
### 6.3.2. Registro de Entrevistas.
### 6.3.3. Evaluaciones según heurísticas.

## 6.4. Auditoría de Experiencias de Usuario
### 6.4.1. Auditoría realizada.
### 6.4.2. Auditoría recibida.

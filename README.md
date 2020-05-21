# Ejercicio Final DIU20 ~ José Santos Salvador
* **Descripción:** Se va a realizar un (re)diseño de una web para una empresa de coworking, aplicando técnicas y metodologías de diseño centrado en un usuario y UX a un caso real.

* **Caso de estudio:** Este rediseño se va a hacer sobre Errant ya que en dicha página hay numerosos puntos de los que hablar y es la que más potencial de mejora tiene. El rediseño de UX se centrará en el analisis de sus problemas o desconexiones entre usuarios y su objetivo final y en la nueva solución a estos problemas mediante un rediseño.

## Problemas y analisis

Errant es empresa de coworking en Granada, el coworking se basa en una filosofía de trabajo por la cual se comparten espacios para desarrollar proyectos. Permiten generar espacios con afluencía de personas que puedan desembocar en nuevas relaciones , dando lugar a espacios no solo de trabajo, si no de gran creatividad y nuevas ideas.  
Errant además de proporcionar servicios de coworking, también proporciona la posiblidad de crear tu proyecto visual (la pecera comunicación).

### Analisis competitivo
En su ámbito de mercado nos encontramos propuestas como:
* *Cubitake* : Añade además la posibilidad de hablar con un bot para más información y obtener un servicio de oficina virtual respecto a Errant.
* *CoFamily Coworking*: Esta propuesta rompe un poco con las bases del coworking y amdeás añade a su objetivo, el trabajo cooperativo junto con el cuidado de tu bebé, todo en un mismo lugar.

### Usability-Review
Para el analisis de usabilidad, se ha centrado en la búsqueda de errores u objetivos que no se cumplen por parte de futuros usuarios. No se ha realizado la creación de personas ficticias para este proposito, ya que se consdiera más importante en un primer vistazo, identificar los posibles problemas y desarrollar soluciones a estos. Durante el analisis de usabilidad, se ha calificado la página con un 6 sobre 10.   
<br>
Los **principales problemas** de la página los encontramos es su corta funcionalidad y es que la página unicamente sirve como expositor de lo que se hace y publicidad, unicamente se puede consultar información (precios, localización, etc) y enviar formularios.   <br>  <br>
No te permite hacer ninguna reserva mediante la página, ni iniciar sesión si eres Errante o consultas relacionadas con la sesión del usuario y la gestión de errores es inexistente o nefasta (meter el erro directamente al html sin ningun tipo de formato con CSS).    <br>
La localización del sitio es una imagen añadidoa al html, sin hacer uso de ninguna API como la de GoogleMaps. Si cliclas en 'espacio coworking granada' del menú principal, sin seleccionar una subopción te genera un error dentro del HTML 
        
        ( Warning: Use of undefined constant PP_SETTINGS_TYPE - assumed 'PP_SETTINGS_TYPE' (this will throw an Error in a future version of PHP) in /homepages/12/d578519675/htdocs/wp-content/plugins/panopress/panopress.php on line 626) 
        
mostrando posible información sensible. La ayuda en linea se resume en formularios, no hay sección de preguntas frecuentes o uso de un bot en linea (como algunas de las empresas de su sector).       <br> <br>
También se reitira la parte de contacto, en la página de inicio al final y en la sección de contacto quizás hubiese sido mejor dejar en la sección principal, un area de información o que muestre algo ilustrativo de las instalaciones.   
Y uno de los principales problemas es lo confuso de su navegación por menús y su posicionamiento


[Usability Review ~ xlsx](https://github.com/thejosess/DIU20_EjercicioFinal/UX.xlsx)  <br>
[Usability Review ~ PDF](https://github.com/thejosess/DIU20_EjercicioFinal/UX.pdf) 


### Accesiblidad
Adicionalmente y para analizar los problemas de accesibilidad se ha hecho uso de extensiones como  accessibbility insights for web, WAVE Web Accesibility Evaluation Tool, Web Disability Simulator y AXE. 
La página no tiene ninguna sección de información sobre accesibilidad, tiene errores de contraste con los enlaces, los formulario no tienen etiquetas correspondientes, varios elementos tienen id iguales, el encabezado debe incrementarse para una mayor visibilidad para personas con discapacidades y no permite el zum y la aplicación ("maximum-scale en la etiqueta <meta> impide el zum en dispositivos móviles"). La aplicación obtiene un resultado pobre en cuanto a accesbilidad, impidiendo su uso normal por personas con discapacidades visuales.   
En cuanto al soporte de otros idiomas, al cambiar al inglés, ocurren algunos errores y las entradas del blog no están traducidas.

        formats not supported oir souces not found

 y no termina de ser una conversión correcta para su uso.


### Labeling que usan
El labeling de la página deja claro que no existe ningún footer (salvo lo que habla de WordPress y que es usado para la página) y hasta las redes sociales están dentro del body de la página.

![](img/labelingOld.png)



## Rediseño UX

### Feedback Captura Grid
Se ha llevado a cabo mediante el feedback obtenido por personas reales que han provado la página.

| Interesante/Relevante | Criticas constructivas|
| ------------- | ------------- |
| Información clara y esclarecedora | Añadir más información sobre la Pecera comunicación |
| Interfaz sencilla y concisa | Mejorar la información sobre que es el coworking |
|| Añadir un buen soporte para otros idiomas |

| Preguntas a raiz de la experiencia | Nuevas ideas |
| ------------- | ------------- |
| ¿Se pueden filtrar las búsquedas? | Añadir un mapa interaccitvo sobre el lugar de las oficinas |
| | Proporcionar una sección de FAQs |
| ¿Puede hacer reservas desde la página web? | Permitir las reservas online |
| ¿Puede gestionar mis cosas de Errante desde la web?|Añadir un area de errante|
| |Añadir un footer mejorado y con información de accesiblidad|
| |Ofrecer un bot para ayudar a los usuarios con sus preguntas |

**Propuesta de valor**   
La propuesta de valor que se va a diseñar a continuación trata de solucionar los problemas ya comentandos, mejorar la navegación por los menús, reorganización del labeling de la página, implementación de un area de clientes, permitiendo realizar reservas, adición de un bot, una sección FAQs y un footer para aummentar la información con los usuarios. Así como la creación de un mapa interactivo para localizar las oficinas.    
<br>
Todo ello con objeto de facilitar el uso a los clientes y permitiendo usar la página no solo como una forma de publicitar los servicios de la empresa, si no como una forma de interactuar con los clientes y los errantes.

### rediseño

explicar aqui los principales problemas que se van a abordar, que no se pierdan los menús cuando bajas la página, añadir un mapa interactivo haciendo uso de la API de google maps, mayor accesibilidad, comandos por voz, zona de usuuario, un bot para ayuda en linea, y meter funcionalidades en la página?, una aplicación? -> explicar que con este rediseño sería muy facil hacer una app, ya que se ha usado PAGINA WEB ->> PWAs

comando de voz para ayudar a personas con discapacidades, un icono que se te abra como un modo con voz todo.

añadir nuevo labeling, nuevos bocetos, nuevas funcionalides o cambio de orden de las cosas de la página (mirar páginas web) y notas.txt
añadir al labeling el bot?, añadirle seccióñn del faqs


HACER QUE EL MENÚ TENGA SENTIDO Y QUE LAS SECCIONES DEL MENÚ SI TE LLEVEN A COSAS INTERESANTE NO COMO TARIFA O ALQUILER DE SALAS QUE TE DAN LA MISMA INFORMACIÓN O COWORKER QUE CASI LO PONDRÍA EN MÁS INFORMACIÓN O CONTACTO.

meter mejores opciones de búsqueda con filtros y tal -> iria en el labeling?




Bibliografía
https://uxdesign.cc/the-new-york-times-timely-app-concept-27efe88e5d4b  
https://uxdesign.cc/redesigning-a-sleep-and-activity-trackers-e-commerce-page-a-ux-case-study-1f1c5b2a8955  
https://uxdesign.cc/ux-ui-case-study-atlanta-jugglers-association-site-redesign-90b422d9dba4   
https://uxdesign.cc/ux-case-studies/home  
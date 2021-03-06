# Frameworks-y-librerias-de-JavaScript

## Cuándo necesitas un framework de JavaScript

* __Websites__ (Sitios Web): Son estáticos (iguales para todos los usuarios), y se pueden hacer únicamente con HTML y CSS.
* __Webapps__ (Aplicaciones Web); Son dinámicas (interactivas con los usuarios) y para estas se necesita JS aparte de HTML y CSS, y algún framework para facilitar el desarrollo.
* __Framework__ (Entorno/Marco de trabajo​): Contiene librerías y herramientas que nos ayudarán a construir algo más rápido, garantizando la calidad gracias a una metodología y estructura de trabajo bien definida.
* __Librería__: Es un fragmento de código que nos ayuda a resolver un problema específico y que tiene un propósito concreto.


## Resumen de la historia de HTML

* 1993 Primera versión “formal” de HTML (NO fue estandar).
* 1995 HTML 2.0: Etiquetas implementadas de imágenes, mápas de imágenes, formularios, estilos…
* 1997 HTML 3.2: Tablas, textos alrededor de imágenes, applets de Java…
* 1999 HTML 4.01: Estandar desde el año 2000
* 2008 Primer borrador de HTML 5
* 2014 HTML 5 como estandar: Como lo conocemos hoy en día.

Referencia MDN: https://developer.mozilla.org/es/docs/Glossary/HTML


## ¿Qué son los componentes?

Partes de código reutilizables y modificables.


## ¿Qué es reactividad?

Reactividad: Es un paradigma, una forma de pensar nuestras aplicaciociones. Deben seguir 2 reglas:

1. Responsive, es decir, deben ser resilientes (siempre sabe qué hacer) y escalables (no importa con cuánta información debemos trabajar o cuántos usuarios entran a la aplicación, la aplicación debe poder seguir funcionando sin problemas).

2. Message Driven (Arquitectura basada en mensajes). Deben de haber emisores y receptores de mensajes. Los mensajes se entregan de manera asíncrona.


Recuerda: La arquitectura no es ajena a la programación.

Estado: Es el lugar donde vamos a guardar la información reactiva de nuestros componentes. Son variables a las que nos suscribimos para recibir una notificación cada vez que cambian sus valores.

Render: o renderizado, es el proceso por el cual nuestro HTML, pasan a ser información visual en el DOM.

Estrategias de render: Virtual DOM y No Virtual DOM. Ninguna es mejor, depende del caso en particular.

Componente -> Estado -> Render -> Usuario (y vuelve a “Estado”)


## Librerías vs. frameworks

__Framework__
Es un conjunto de piezas de codigo que se centra en la elaboración o construción todo un proyecto a través de un conjunto de herramientas que nos brinda el framework (puede incluir librerías) como si de una receta se tratase.

__Librería__
Es una porción o pieza de codigo que nos ayuda a resolver un problema en específico como trabajar con HTMLmediaElement (video o audio) por ejemplo.


## Ecosistema de frameworks y librerías JavaScript

Existen empaquetadores que nos ayudan a tener todos los archivos en produccion pero al momento de mandar al navegador sea lo mas ligero posible

* Webpack: Requiere que configuremos un archivo para especificar como queremos nuestro archivo.
* Parcel: Es evitarnos cualquier configuracion, trae todo listo para que construya toda su magia. No tenemos control de como empaqueta.
* Rollup: Se especializa en tener todo optimizado con una tecnica especial donde elimina el codigo inuti

Se dice que usemos webpack para paginas web y aplicaciones y Rollup para librerias.

Compiladores que transforman codigo Javascript que no es exactamente JS que los navegadores si pueden entender:

* Babel: Nos permite usar el codigo del futuro en proyectos que utilizan otra version, unificando todo en una version que entiendan los programadores
* TypeScript: Es un lenguaje de programacion con sus nuevas reglas que nos permiten entender mas facil los errores en JavaScript

Las herramientas para UI son para encargarse de las vistas e interaccion con los usuarios, puede ser JS solito pero si trabajamos en Frameworks se suelen usar:

* React
* Vue
* Svelt

Estan los estilos donde se pueden usar diferentes cosas, pero hay que tener en cuenta que a veces escribimos mas JS que CSS:

* CSS
* SASS
* LESS
* STYLUS

En CSS-in-JS normalmente el html, el css y el JS estaria en cada archivo individual pero esto nos permite desarrollar en los 3 lengaujes en un mismo componente, que necesariamente no es un mismo archivo.

* Styled Components
* Emotion

En los Routers son la forma en la que hacemos la navegacion de la aplicacion, muestra cierto contenido dependiendo de la URL

* React Router
* Vue Router
* Svelte Router
* LitElement Router
* Whatever Router

Los frameworks son elementos todos en uno, que se encargan de todos los apartados ya que todo lo contiene. Trabajar con un Framework acelera tu desarrollo.

* Angular: Es todo poderoso pero por ser tan grande es bastante dificil de integrar con otras herramientas que no sean especiales para ANGULAR.

Los entornos de desarrollo completos son un todo en uno, un grupo de librerias configuradas para trbajar con mas librerias. se llaman mas CLI y desde la consola podemos elegir lo que queremos y configurar todo por nuestro lado.

* Create React App
* Vue CLI
* Svelte CLI
* Polymer CLI
* Whatever CLI

En el manejo de estado son las librerias que podremos definir un estandar de flujo de datos constante y predecible dentro de la aplicacion, en vez de que todos sean diferentes podremos definir un patron comun

* Redux
* XState
* MobX

En la consulta de datos son formas o protocolos para comunicarnos con el backend para enviar y recibir informacion, hay herramientas para hacer peticiones que no hacen diferencia, pero estas herramientas si hacen diferencia:

* API REST
* GraphQL


## ¿Qué es React y cómo se construyó?

ECMAScript es estándar en el que se basa JavaScript, es la especificación del lenguaje de programación JavaScript; y lo que conocemos como Javascript es la implementación que hace cada navegador de esta especificación.

En 2005 surgió ECMAScript for XML, un estándar para agregar soporte nativo de ECMAScript a XML. Era una alternativa a la forma en la que se trabaja con el DOM.

En 2010, inspirados en ECMAScript for XML, Facebook estaba trabajando en XHP, una “mejora” a PHP con la que pretendían crear componentes personalizados y reutilizables de HTML y lo integraron a su Stack.

En 2011, bajo la influencia de XHP y los problemas que tenía Facebook, se creó el prototipo de React JS. Una herramienta para desarrollar aplicaciones con la que pudieran mejorar la eficiencia del los desarrolladores y seguir ofreciendo una buena UX.

En 2012 React se volvió Open Source.

En 2014 llegaron las React Developer Tools, un conjunto de herramientas para depurar componentes de React.

En 2015 apareció React Native, y con él muchas empresas grandes empezaron a utilizar React.

### Objetivos de React

* Declarativo: Se refiere a que sea fácil de leer.
* Basado en componentes: Que todo este formado por componentes.
* Multiplataforma: Significa que podremos utilizar React en cualquier plataforma con solo pequeños cambios.

Existe un gran ecosistema de herramientas relacionadas con React, algunas desarrolladas por Facebook y otras por creadas por la comunidad. Por ejemplo:

* React DOM: Se utiliza para renderizar los componentes de React en el navegador.
* React Native: Usado generalmente para crear aplicaciones móviles.

---
Hay dos formas de crear componentes con React: con una clase y con una función

Al crear componentes con una clase esta usa un función render y dentro una función return. Dentro de esta ultima se encuentra el código JSX para crear el componente. Además, React utiliza las llamadas props para presentar ciertas partes del componente de manera dinámica.

React también cuenta con el state, que nos sirve para cambiar el contenido de las variables dependiendo de la interacción del usuario. Este estado es un objeto donde podemos definir propiedades para después hacer uso de ellas. Cuando React detecta un cambio dentro del state automáticamente se vuelve a renderizar el componente mostrando los nuevos datos.


## Cómo usar React.js

Codigo en CodeSandbox: https://codesandbox.io/s/distracted-leakey-os80h?file=/src/form.js
El resultado: https://os80h.csb.app/?

## ¿Qué es Angular y cómo se construyó?

En el 2009 un grupo de amigos Desarrolladores inventaron una herramienta para que personas que no sabian programar pero si HTML pudieran hacer aplicaciones, esto no tuvo exito. Despues uno de ellos fue a trabajar a Google Feedback. Pero para esto necesitaron 17k lineas de codigo en frontend, usando un Google Web Toolkit, pero por esto apostaron que podian hacerlo en 2 semanas, pero logro hacerlo en 3 y con 1.5k lineas de codigo, y asi nacio Angular JS, que se volvio Open Source y patrocinado por google. Es como REACT pero FB depende totalmente de este, pero Google no depende de angular. Google solo lo patrocina.

Entre 2012 y 2014 Angular era bastante popular pero con el paso del tiempo empezo su decaida, y anunciaron que lo iban a hacer desde 0 y empezar a usar componente, pero los que iban a usar a angular no sabian que iba a pasar porque no iba a tener compatibilidad.

Es dificil convinar angualar con alguna libreria o algo que no se haya hecho especificamente para angular.

Angular tiene un sistema para crear componentes que se llaman Engine Modulos o Modulos de angular, que agrupan componentes y servicios a un mismo fin o a un mismo dominio. Los componentes son la logica y la interfaz de usuario para cada pedazo de la aplicacion.

Los componentes tienen dos partes, las logicas y las partes de UI, esto lo haremos con una clase en TS. Lo definimos con algo parecido a HTML.

Los servicios son agrupaciones de codigo. Agrupaciones de logica que podemos usar en varios componentes por toda la aplicaion. Esto lo inyectamos a los componentes que usamos Inyeccion de dependencias.

Angular tiene a Angular Ivy que se encarga de renderizar los componentes en angular con Incremental DOM. Como React usa JSX, Angular tiene su variacion de HTML que no es puro. Lo que hace Angular Ivy es convertir este HTML en un JS para renderizar los componentes en el DOM.

Angular explica que crear una copia de todo el DOM es innecesario, con el Incremental DOM cada componente se convierte en Instrucciones y estas hacen que se ejecute y renderice y actualice el componente, en ningun momento crea copia del DOM y ahorra memoria.

En angular 9 reescribieron el motor completamente. Antes habia que compilar muchas veces cada que cambiabamos componentes. Con Angular Ivy cambio la forma en la que se describe para que los componentes solo se afecten asi mismos y no a los demas.

##  Cómo usar Angular

Codigo en CodeSandbox: https://codesandbox.io/s/movies-angular-25sx5
El resultado: https://25sx5.csb.app/

## ¿Qué es Vue y cómo se construyó?

“El Framework progresivo”

No es un framework tan abrumador como Angular, pero aún así puede ir escalando progresivamente a medida que lo vamos necesitando.

Escalable pero no flexible.

Se integra bien con cualquier herramienta que queramos utilizar.

Es completamente Reactivo.

Vue también usa el Virtual DOM.

En pocas palabras, al principio Vue nos deja trabajar al principio casi como si siguiéramos usando HTML común y corriente pero poco a poco le vamos metiendo JS usando Vue hasta que llega un momento en el que prácticamente todo la aplicación está hecha en JS con componentes de Vue.

Nos deja trabajar con componentes pero no es obligatorio en un inicio.

“El mejor performance”

## Cómo usar Vue.js

Codigo en CodeSandbox: https://codesandbox.io/s/movies-vue-of39d
El resultado: https://of39d.csb.app/

## QUE ES SVELTE Y COMO SE CONSTRUYÓ

Rich Harris creó SVELTE

* La principal característica es que no crea intermediarios entre el código que se escribe en SVELTE y el DOM.
* A diferencia de React, SVELTE no usa el VirtualDOM.
* SVELTE es Espectacular para desarrollar sitios WEB
* SVELTE No es tan fuerte en Aplicaciones WEB
* ARQUITECTURA DE SVELTE:
* No hay un recurso oficial que nos explique como funciona SVELTE por dentro.
* Dustin Deus: escribió un issue acerca de la Documentación:

### Resumen del Resumen del Resumen :0

1.- SVELTE es un Compilador, por tanto, necesita generar un AST(Abstract Syntax Tree).
2.- Para esto necesita 3 Parsers: HTML, CSS, y JavaScript. COMBINA ESTOS 3 ARBOLES.
3.- Envuelve como un envoltura de chocolate 😄, todos los componentes en FRAGMENTS, Una interfaz API del Navegador.
4.- Esa interfaz sirve para ENCAPSULAR: Nodos, y pedazos del DOM, esto no afecta la interfaz de la Página.
5.- Los FRAGMENTS es como un nodo imaginario(No es visible para los usuarios), pero si tiene todos las características de un nodo.(Crear, Actualizar, Borrar)

## Cómo usar Svelte

Codigo en CodeSandbox: https://codesandbox.io/s/movie-svelte-7ue6i
El resultado: https://7ue6i.csb.app/

## CSS-in-JS
CSS-in-JS es una técnica de diseño en la que se usa JavaScript para diseñar componentes. Cuando se analiza este JavaScript, se genera CSS y se adjunta al DOM. Permite abstraer CSS al nivel de componente en sí, usando JavaScript para describir estilos de una manera declarativa y mantenible.

## Componentes en Angular con CSS

Codigo en CodeSandbox: https://codesandbox.io/s/movies-angular-25sx5?resolutionWidth=320&resolutionHeight=675&file=/src/app/app.component.css
El resultado: https://25sx5.csb.app/

## Trabajando con Vue Components y Vue Components con Preprocesadores de CSS

Codigo en CodeSandbox: https://codesandbox.io/s/vue-components-t26mp
El resultado: https://t26mp.csb.app/

## Trabajando en React con Styled Component

Codigo en CodeSandbox: https://codesandbox.io/s/como-usar-react-os80h?file=/src/form.js:259-271
El resultado: https://os80h.csb.app/

## Estilos dinámicos con Styled Components en React

Codigo en CodeSandbox: https://codesandbox.io/s/como-usar-react-os80h?file=/src/form.js
El resultado: https://os80h.csb.app/

## Trabajando en Svelte con Emotion

Codigo en CodeSandbox: https://codesandbox.io/s/movie-svelte-7ue6i?file=/styles.js:696-701
El resultado: https://7ue6i.csb.app/

## Tipos de aplicaciones según su router: SPAs vs. SSR

Antes de las aplicaciones web modernas se usaba el SSR “viejo” (Server Side Rendering), con el que el backend usaba una plantilla de HTML le daba a la plantilla los datos específicos requeridos en cada petición y le enviaba el HTML al navegador. Está forma de hacer render es rápida solo al principio porque el backend no le entrega al navegador la forma de interactuar con los usuarios

### SPAs y CSR

Single Page Applications: Se inventa el Client Side Routing aquí gracias en parte a las API’s se empezó a renderizar el contenido desde JS directamente en el navegador. Es decir, el backend le entregaba al navegador un HTML prácticamente vacío, que tenía solo la petición de un script o alguna hoja de estilos. Entonces el navegador recibía el HTML en blanco, descargaba el JS y CSS y entonces JS podía empezar a renderizar la aplicación, entonces la carga inicial es lentísima, pero luego se hace bastante rápida, no necesita recargarse y cuando requiere información del backend solo hace la consulta a una API (que son fundamentales para estas aplicaciones).

Para trabajar de esta forma tenemos dos componentes:

Los routers son herramientas para manejar las rutas de nuestra aplicación, normalmente de eso se encargaría el servidor.

Si no se tiene control servidor se usa:

* __Hash Router__: Con “#” definimos en que parte de la aplicación estamos (en el home, logout, clientes, admin, etc.).

Si tienes control sobre el servidor:

* __Browser Router__: Sin importar la ruta puedes pedirle al servidor que siempre de el mismo index.html, y con JS podemos determinar en que ruta estamos y que ruta debemos mostrar dependiendo de la ruta que nos dio el servidor o navegaron e interactuaron los usuarios.

### Progressive SSR

Gracias al CSR de la SPA se invento el SSR (Server Side Rendering combinado con Client Side Rendering).

En lugar de mandar un documento HTML vacío al navegador y tardara mucho en descargarlo, se podía acelerar el proceso, desde el backend enviamos al navegador una versión de la aplicación en HTML que los usuarios puedan ver mientras el navegador descarga los archivos de JS y vuelve a hacer render de la aplicación. Entonces, el backend le envía al navegador una versión de la app que solo se puede ver pero no tocar, es decir, los usuarios no pueden interactuar inmediatamente con la app.

NOTA: Para esto se necesita Node.js.

### Generación de Sitios Estáticos

Estos generadores nos permiten usar el Progressive SSR mientras estamos desarrollando el sitio, pero cuando lo compilamos nos generan páginas estáticas que ya tienen cargados los datos que normalmente le pediríamos al backend y cuando hacemos deploy las aplicaciones funcionan de una. Si hay algún dato que nos daba el servidor pero que sabemos que casi no va a cambiar (como un blogpost) podemos volver a hacer deploy si queremos editar el contenido no habrá problema alguno.

## Frameworks sobre frameworks: Next.js

Codigo en CodeSandbox: https://codesandbox.io/s/next-movie-d93iv
El resultado: https://d93iv.sse.codesandbox.io/

## ¿Necesitas un framework o una librería? 📚


Elegir frameworks o librerías de JavaScript para tu próximo proyecto web es una gran responsabilidad. Tus preferencias personales deben ser el último factor a considerar. Lo realmente relevante son el tiempo, presupuesto, requisitos técnicos y el conocimiento + experiencia del equipo de desarrollo con cada tecnología.

Un framework te provee casi todas las herramientas que necesitas para construir un sitio o aplicación web (guía de estilos predefinida, manejo de formularios, facilidad para elegir el tipo de routing o la estrategia de render que necesites…).

Por su parte, las librerías responden a un objetivo más específico y menos general. Una parte importante del desarrollo será elegir qué librerías integrar y realizar la configuración para que funcionen correctamente en conjunto.

También debes considerar que el costo/dificultad de integrar librerías con librerías suele ser muy bajo. Donde realmente aumenta la complejidad es configurando frameworks de JavaScript para trabajar en conjunto con librerías que no fueron específicamente diseñadas para ese framework en particular.

O al menos eso es a lo que estamos acostumbrados.

## Rangos de flexibilidad, integrabilidad y responsabilidad 🚧

Las herramientas de desarrollo frontend no tienen que ser a fuerza un framework o una librería. Más bien, las conocemos de una u otra forma dependiendo de sus rangos de flexibilidad.


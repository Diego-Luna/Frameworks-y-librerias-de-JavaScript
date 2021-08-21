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
En vivo el resultado: https://os80h.csb.app/?

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
En vivo el resultado: https://25sx5.csb.app/

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
En vivo el resultado: https://of39d.csb.app/
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

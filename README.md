# Qué es React JS

[Clase #1](https://platzi.com/clases/1651-react-ejs/21953-que-es-react--0/)

- React es una librería desarrollada por Facebook que nos ayuda a construir interfaces de usuario interactivas para todo tipo de aplicaciones: web, móviles o de escritorio.

- Cada pequeña parte de nuestra página web la - conoceremos como “Componente”. Cada componente se encargará de una función en específico. Además, podremos reutilizar nuestros componentes siempre que lo necesitemos.

- Al unir todos nuestros componentes tendremos una página web que nos permite cambiar, actualizar o eliminar elementos de forma muy sencilla.

## Sitios que utilizan ReactJS

- AirBnb
- Netflix
- Uber (Landings)
- WhatsApp
- Platzi

## Clase 2 - Dom, Virtual DOM y React DOM

[Clase #2](https://platzi.com/clases/1651-react-ejs/21927-dom-virtual-dom-y-react-dom/)

- El DOM es el código HTML que se transforma en páginas web.

- Cada vez que cambiamos alguna parte del DOM, también estamos actualizando el HTML con el que interactúan nuestro usuarios. EL problema es que todas las operaciones, comparaciones y actualizaciones en el DOM con muy costosas.

- El Virtual DOM es una herramienta que utiliza tecnologías como React y Vue para mejorar el rendimiento y velocidad de nuestras aplicaciones.

- Es una copia exacta de DOM, pero mucho más ligera, ya que los cambios no actualizan el verdadero HTML de nuestras páginas web. Gracias al Virtual DOM podemos hacer operaciones y comparaciones de forma sumamente rápida.

- Recuerda que loos ca,sbiios en e Virtual DOM no afecta el HTML que ven los usuarios, así que podemos estar sincronizando constantemente las copias con el DOM. Pero noe te preocupes, React DOM lo hace por nosotros.

## Curso de Prework & Buenas prácticas

[Prework - Best Practices](https://platzi.com/cursos/prework/)

## Clase 3 - Create ReactApp y Tipos de Componentes

[Clase #3](https://platzi.com/clases/1651-react-ejs/21928-create-react-app-y-tipos-de-componentes/)

- Instalar react-app

- npx create-react-app nombre-de-tu-proyecto

- Iniciar el servido de desarrollo:

- npm start

## Creación y Tipos de Componentes

- Los nombres de nuestros componentes deben empezar con una letra mayúscula, al igual que cada nueva palabra del componente. Esto lo conocemos como Pascal Case o Upper Camel Case.

## Componentes Stateful

- Los componentes Stateful son los más robustos de React. Los usamos creando clases que extiendan de React.Component. Nos permiten manejar estado y ciclo de vida (más adelante los estudiaremos a profundidad).

``` import React, { Component } from 'react';

class Stateful extends Component {
  constructor(props) {
    super(props);

    this.state = { hello: 'hello world' };
  }

  render() {
    return (
      <h1>{this.state.hello}h1>
    );
  }
}

export default Stateful;
```

## Componentes Stateless

- También tenemos componentes Stateless o Presentacionales. Los usamos creando funciones que devuelvan código en formato JSX (del cual hablaremos en la próxima clase).

``` import React from 'react';

const Stateless = () => {
  return (
    <h1>¡Hola!h1>
  );
}

// Otra forma de crearlos:
const Stateless = () => <h1>¡Hola!h1>;

export default Stateless;
```

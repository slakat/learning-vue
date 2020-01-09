# Aprendiendo Vue.js
1. Instalación ([pasos](https://www.taniarascia.com/getting-started-with-vue/))
Hay dos formas de instalar Vue: en un proyecto Node o directamente inyectando la librería en un archivo estático de HTML (lo más simple).

. Opción de inyectado; agregar lo siguiente al interior de la etiqueta ::head::

`<script src=“https://cdn.jsdelivr.net/npm/vue/dist/vue.js”></script>` 

Para crear texto podemos usar brackets 

`<div id=“app”>{{message}}</div>`

y dentro de un tag ::script::  enlazar los datos y el DOM. Creamos un nuevo ::vue:: y la propiedad message  on ::data::.

```<script>
      const App = new Vue({
        el: ‘#app',
        data: {
          message: ‘H’llo Vue!’,’        },
      })
    </script>
```

Recordar:
_”Vue is just JavaScript, and there’s no need to get nervous about Node, Babel, Webpack, and so on.”_

## Vue CLi
Hay que aprovechar el ecosistema Node y la forma más fácil es hacerlo a través de la Vue Command Line interface (CLi). Hay que estar un poco familiarizado con Node y npm/yarn, además de cómo organizan sus paquetes de forma global y local.

### Instalar Vue CLi
```# instalar con npm
npm i -g @vue/cli @vue/cli-service-global

# instalar con yarn
yarn global add @vue/cli @vue/cli-service-global

```

Ahora que Vue está instalado globalmente podemos ocuparlo en cualquier parte. Para crear un nuevo proyecto usamos Vue create (equivalente al create-react-app):

`vue create vue-app`


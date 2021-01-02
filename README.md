## Vuex Overlay Tool

![](https://i.imgur.com/RQPG21h.png)

I like Vue, but latest release (Vue 3) working only with new `vue-devtools` version and there is no Vuex in it at the moment.
And I must to create a temporary solution for this problem - `vuex-overlay-tool`.

**Vuex Overlay Tool** plugin for **Vue 3** provides monitoring of the state in the store with feature from `vue-devtools` time-travel.

## Features
* overplay panel with Vuex store from your app
* mutations history
* state & getters overview
* time travel for mutations

PS. Package working with Vuex modules 

## Getting Started
Required

[Vuex 4](https://github.com/vuejs/vuex) & [Vue 3](https://github.com/vuejs/vue-next)

Install
```bash
$ npm install vuex-overlay-tools

# or
$ yarn add vuex-overlay-tools
```

## Usage
`Your application must have Vuex Store`

###### Step 1 - Add VuexOverlay plugin to you application
```js
import { createApp } from "vue";
import VuexOverlay from "vuex-overlay-tools"

import { store } from "./store" // path to vuex store
import App from "./App.vue"

createApp(App)
  .use(store) // required
  .use(VuexOverlay) // add plugin to your app
  .mount('#app')
```
###### Step 2 - Open panel with special button
![](https://i.imgur.com/YcDdvJs.png)

## Previews
###### `State Overview` 
![](https://i.imgur.com/CxFL2Dv.gif)

###### `Getters Overview`
![](https://i.imgur.com/fJBWo73.png)

###### `Mutations History`
![](https://i.imgur.com/FxiBjKJ.png)




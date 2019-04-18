# Abstract (renderless) Vue components

A personal collection of Abstract (aka renderless components). Abstract components allow different UIs only focuses on functionality.

- [ ] Abstract Toggle : Toggle boolean flags (true/false) 
  - [ ] Toggle Button
  - [ ] Toggle Switch 
- [ ] Abstract Expand : Expand and collapse 
  - [ ] Accordion 
  - [ ] Sidebar
- [ ] Abstract Dropdown : Any control that needs a dropdown menu
  - [ ] Dropdown menu
  - [ ] Used in Tag List (below)
- [ ] Abstract List : Add, Remove list items from array
  - [ ] Tag List
  - [ ] Grid


Inspiration: https://adamwathan.me/renderless-components-in-vuejs/

My abstract component follow the follow pattern:

``` javascript
Vue.component('abstract-component-example', {
  // Props, data, methods, etc.
  render() {
    return this.$scopedSlots.default({
      // properties to expose
      prop1: this.prop1,
      prop2: "Something else",
      // typically include bindings, properties we want to add to the component
      bindProps: { },
      // typically events that component needs to use
      bindEvents: { }      
    })
  },
})
```


## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

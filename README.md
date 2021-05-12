# Vue Dynamic Slots example

Have you ever wondered how you can reorganize a components inputs based on a given format? This REPO demonstrates how this can be done using dynamic `slot`s. The beauty of using a `slot` instead of an algorithm to dynamically generate the order is that the slots can be filled out and individually customized with whatever you need (ie custom validation for only one `input` and not _all_ inputs).

## Why is this useful?

A good example of this use case is address formats. Different countries have different formats, like Germany shows a different format from the United States. Perhaps you want to build an `AddressDisplay` component and you want the display to change depending on the country specified. Well you're in luck - with this repo have a look at the `SlotsExample.vue`. Follow this same logic to create a wrapper around your main address component like I have implemented in the `App.vue`.

## Usage

Take a peek at the `App.vue`, it is wrapped with the `SlotsExample.vue` component to dynamically change the order of the fields within `App.vue`.

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

### Lints and fixes files

```
npm run lint
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).

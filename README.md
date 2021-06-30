# Vue Dynamic Slots example

Have you ever wondered how you can reorganize a components structure based on a given format? This repo demonstrates how this can be done using dynamic `slot`s. The beauty of using a `slot` instead of an algorithm to dynamically generate the order is that the slots can be filled out and individually customized with whatever you need (ie custom validation for only one `input` and not _all_ inputs).

## Why is this useful?

In short because it displays the awesomeness of dynamic slots.

A good example of this use case for something like this would be address formats. Different countries have different formats, like Germany shows a different format from the United States or United Kingdom formats.

Perhaps you want to build an `AddressDisplay` component and you want the display order of the address to change depending on a given format. Well you're in luck - with this repo have a look at the `SlotsExample.vue`. Follow this same logic to create a wrapper around your main address component like I have implemented in the `App.vue` and you can get a clean way to dynamically alter the order of your data based on a given format, yet still be able to easily add new fields and maintain existing fields.

## Usage

Look at the `App.vue`, it is wrapped with the `SlotsExample.vue` component to dynamically change the order of the fields within `App.vue`.

## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run dev
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

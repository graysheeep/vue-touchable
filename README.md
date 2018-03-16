# vue-touchable

[![npm](https://img.shields.io/npm/v/vue-touchable.svg?maxAge=2592000?style=flat-square)]()
[![npm](https://img.shields.io/npm/dt/vue-touchable.svg?maxAge=2592000?style=flat-square)]()

> React-Native中TouchableOpacity和TouchableHighlight的Vue组件实现。

[Simple Live Demo](https://graysheeep.github.io/vue-touchable/)

## install

``` bash
npm install vue-touchable
```

## usage

``` js
import { TouchableOpacity, TouchableHighlight } from 'vue-touchable'

<template>
  <touchable-opacity>
    <div>
      Click to toggle opacity
    </div>
  </touchable-opacity>

  <touchable-highlight>
    <div>
      Click to toggle highlight
    </div>
  </touchable-highlight>
</template>
```

## dev

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev
```

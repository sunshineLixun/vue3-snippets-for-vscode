# sjzy-vue3-snippets

这是一个适配 Vue3 Api 的 snippets 插件

## setup 快速创建代码块模板

输入 `setup` 一键创建模板

<img src="https://cdn.jsdelivr.net/gh/sunshineLixun/vue3-snippets-for-vscode@master/assets/guide_1.2.gif?raw=true" style="zoom: 40%;" />

**支持快速 console.log，方便调试**

- 输入 `clg` 一键开起 console，然后直接输入需要打印的变量即可。

<img src="https://cdn.jsdelivr.net/gh/sunshineLixun/vue3-snippets-for-vscode@master/assets/clg_guide.gif?raw=true" style="zoom: 30%;" />

**注意** :本插件可能不完全适用于 vue2

# 特性

目前支持的代码片段

### 模版片段

|  关键词  |                                    代码片段                                    |
| :------: | :----------------------------------------------------------------------------: |
|  setup   | `<script setup lang="ts">xxxxxxx<template></template></script><style></style>` |
|  vinit   |    `<template></template><script setup lang="ts"></script><style></style>`     |
| template |                       `<template><div></div></template>`                       |
| scripte  |                      `<script setup lang="ts"></script>`                       |
|  style   |                           `<style lang=""></style>`                            |
|   css    |                            `<style scoped></style>`                            |
|   scss   |                      `<style lang="scss" scoped></style>`                      |
|   Sass   |                      `<style lang="sass" scoped></style>`                      |
|   Less   |                      `<style lang="less" scoped></style>`                      |

### script&vue 片段

|      关键词      |                   代码片段                   |
| :--------------: | :------------------------------------------: |
|       clg        |   `console.log('output->${0}',${0:name})`    |
|      Import      |          `import {...} from '...'`           |
|       Data       |            `data(){return {...}}`            |
|      Setup       |          `setup(){...return{...}}`           |
|      vText       |                `v-text="..."`                |
|      vHtml       |                `v-html="..."`                |
|      vShow       |                `v-show="..."`                |
|       vIf        |                 `v-if="..."`                 |
|      velse       |                   `v-else`                   |
|     velseif      |              `v-else-if="..."`               |
|       vFor       |       `v-for="... in ..." :key="..."`        |
| vFor(withoutKey) |             `v-for="... in ..."`             |
|       vOn        |                 `v-on="..."`                 |
|      vBind       |                `v-bind="..."`                |
|      vModel      |               `v-model="..."`                |
|      vSlot       |                `v-slot="..."`                |
|      vOnce       |                   `v-once`                   |
|   iscomponent    |     `<component :is="..."></component>`      |
|    **vprops**    | `const props = defineProps({ foo: String })` |
|    **vemits**    |  `const emit = defineEmits(['...', '...'])`  |

### vue-router 片段

|      关键词      |                        代码片段                        |
| :--------------: | :----------------------------------------------------: |
|    beforeeach    |      `router.beforeEach((to, from, next) =>{...}`      |
|  beforeresolve   |    `router.beforeResolve((to, from, next) => {...}`    |
|    afterEach     |         `router.afterEach((to, from) => {...}`         |
|   beforeenter    |          `beforeEnter(to, from, next) {...}`           |
| beforeRouteEnter |        `beforeRouteEnter(to, from, next) {...}`        |
| beforeRouteLeave |        `beforeRouteLeave(to, from, next) {...}`        |
|      vroute      | `{'path':...,name:...,component: () => import('...')}` |

**Enjoy!**

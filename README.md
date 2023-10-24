# viu-ts

Boilerplate template for vue3 using typescript, pinia, vue-router, vite, vitest and cypress 

### Template

+ [ ] [Vue3](https://vuejs.org/)
+ [ ] [Typescript](https://www.typescriptlang.org/)
+ [ ] [Web Worker](https://www.npmjs.com/package/web-worker)
+ [ ] [Dependency Injection](https://www.npmjs.com/package/typescript-ioc)
+ [ ] [Pinia](https://pinia.vuejs.org/)
+ [ ] [Router](https://router.vuejs.org/)
+ [ ] [Vite](https://vitejs.dev/)
+ [ ] [Vitest](https://vitest.dev/)
+ [ ] [Cypress](https://www.cypress.io/)
+ [ ] Sass
+ [ ] Logger


### How to start app

+ File main.ts will look a like

```ts
// main.ts
new ViuApp()
.setModules('development', new HttpModule(), new AuthModule())
.setModules('production', new HttpWebWorkerModule(), new AuthModule())
.setLogLevel('development', LogLevel.Debug)
.setLogLevel('production', LogLevel.Error)
.use(router)
.use(pinia)
.use(CommonComponents)
.setMainScreen(App)
.setName('viu-ts')
.mount('#app')
.start(import.meta.env.MODE)
```

### License

[MIT@tvc12](./LICENSE)

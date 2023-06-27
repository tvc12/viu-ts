# viu-ts
Boilerplate template for vue3 using typescript and vite 

### Template

+ [ ] Vue3
+ [ ] Typescript
+ [ ] Web Worker
+ [ ] Dependency Injection
+ [ ] Pinia
+ [ ] Router
+ [ ] Sass
+ [ ] Logger
+ [ ] Vite


### How to start app

+ File main.ts will look a like

```
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

# shims
i've no idea how it works but it works

```/src/shims-vue.d.ts```
due to unresolved jetbrain vue support for typescript 5
https://youtrack.jetbrains.com/issue/WEB-60063/Introduce-Volar-support-for-Vue-to-fix-a-problem-with-Typescript-5.0-in-Vue-SFC#focus=Comments-27-7057634.0-0
```
declare module '*.vue' {
    import type { DefineComponent } from 'vue'
    const component: DefineComponent<{}, {}, any>
    export default component
}
```
credit to 
https://stackoverflow.com/questions/54622621/what-does-the-shims-tsx-d-ts-file-do-in-a-vue-typescript-project/59788563#59788563




### 注意事项（不要写不易追踪的代码）
- 每一个文件中用到的外部`变量`、`方法`、`css`等等，都要明确声明
- 禁用全局样式
- 禁用`mixin`
- 不建议使用`vuex` 。（如果用：请把变量名取复杂一点）
- 不建议使用 `provide` 和 `injecet`。 （如果用：请把方法名取复杂一点）
- 不建议挂载全局原型链 `Vue.prototype = xxxx`
- 组件创建（单文件组件可以不用文件夹）
  ```
  YourWrapper
      ├── views 【可选】文件夹：路由链
      ├── components 【可选】文件夹：用到的组件
      ├── styles 文件夹：【可选】样式相关
      ├── index.ts/index.js 【可选】
      └── index.vue 【必须】组件入口
  ```
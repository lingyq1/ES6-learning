## typeScript 
- 对象补充

> 对象是包含一组键值对的实例。不可以直接给定义好的对象添加新的方法，而应该先定义一个函数的类型模板。

```js
var obj = {
  name: "Anzo",
  gender: "male",
};
obj.func = function () {
  console.log("Hi " + obj.name);
};
obj.func(); // 报错
```

这样会报错 -- 类型“{ name: string; gender: string; }”上不存在属性“func”。
所以应该先在对象里定义函数，如下：

```js
var obj = {
  name: "Anzo",
  gender: "male",
  func: function () {}, //类型模板
};
obj.func = function () {
  console.log("Hi " + obj.name);
};
obj.func(); // 正确，输出 Hi Anzo
```

- typeScript 区分大小写
- typeScript 分号是可选的
以下代码是合法的
```js
 console.log("Hello!")
 console.log("Hello!");
```
两个语句在同一行，一定要用分号隔开，否则会报错。
```js
console.log("Hello!");console.log("World!");
```

#### typeScript 模块
导入使用关键字：import
导出使用关键字：export
```js  
  // 文件名： SomeInterface.ts
export interface SomeInterface {

}
```

```js
   // 这是另一文件
import  someInterfaceRef = require("./SomeInterface");
```

## 对于 JSX 的书写形式

- 为了便于阅读，一般会把 JSX 拆分为多行。同时，将内容放在括号里面，这样可避免自动插入分号陷阱。

```js
const element = (
    <h1>
      Hi World!
    </h1>
    );

ReactDOM.render(
    element,
    document.getElementById('root')
  );
```

- 因为 JSX 语法上更接近 JavaScript 而不是 HTML，所以 React DOM 使用 camelCase（小驼峰命名）来定义属性的名称，而不使用 HTML 属性名称的命名约定。

## typeScript 对象补充

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
    func: function () { }, //类型模板
};
obj.func = function () {
    console.log("Hi " + obj.name);
};
obj.func(); // 正确，输出 Hi Anzo
```

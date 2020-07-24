#### 选择器

1. C
2. B

#### 简答题

1. 不是。

   首先，需要将data中的属性注入到vue实例vm上。this.dog会出get方法，内部会去或获取data的dog属性。由于observer中会递归遍历data对象，将其属性变成响应式的。但是，起初dog定义时没有name属性，现在获取dog的name属性无法触发get方法，赋值也无法触发set方法。
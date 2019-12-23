# call、apply、bind的用法
由于this可以动态切换，所以给JS创造了巨大的灵活度，使这也使得编程变得模糊而困难。

**call方法：** 可以指定函数内部this的指向，然后在所指定的作用域调用该函数。call方法可以接受多个参数，第一个参数使this所要指向的对象，后续的参数使函数调用时所需的参数，如果第一个参数为空、null或undifined，则默认指向全局对象。

**apply：** 该方法与call方法相似，唯一区别是是他接收一个数组作为函数执行时的参数。

**bind：**  bind方法将函数体内的this指向绑定给某个对象，然后返回一个新函数。bind方法的参数就是索要绑定this的对象。该方法也可以接受更多参数，将这些参数绑定为原函数的参数，如果传入的第一个参数是null或undefined，则等同于将this绑定在全局对象上。
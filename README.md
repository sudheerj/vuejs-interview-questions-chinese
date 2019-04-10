# VueJS 面试题

Original English version: [vuejs-interview-questions](https://github.com/sudheerj/vuejs-interview-questions)

列出了 300 道 VueJS 面试题

> 如果你喜欢这个项目点击 :star:，Pull Requests 是非常赞赏的。

## 内容列表

| 序号 | 问题                                                                                                             |
|------|------------------------------------------------------------------------------------------------------------------|
| 1    | [VueJS 是什么？](#1-vuejs-是什么)                                                                                |
| 2    | [VueJS 的主要功能是什么？](#2-vuejs-的主要功能是什么)                                                            |
| 3    | [VueJS 的生命周期方法是什么？](#3-vuejs-的生命周期方法是什么)                                                    |
| 4    | [条件指令是什么？](#4-条件指令是什么)                                                                            |
| 5    | [v-show 和 v-if 指令有什么不同？](#5-v-show-和-v-if-指令有什么不同)                                              |
| 6    | [v-for 指令的目的是什么？](#6-v-for-指令的目的是什么)                                                            |
| 7    | [vue 实例是什么？](#7-vue-实例是什么)                                                                            |
| 8    | [如何实现条件组元素？](#8-如何实现条件组元素)                                                                    |
| 9    | [如何复用有 key 属性的元素？](#9-如何复用有-key-属性的元素)                                                      |
| 10   | [为什么不能在同一个元素上同时使用 v-if 和 v-for 指令？](#10-为什么不能在同一个元素上同时使用-v-if-和-v-for-指令) |
| 11   | [为什么使用 for 指令时需要 key 属性？](#11-为什么使用-for-指令时需要-key-属性)                                   |
| 12   | [什么是数组检测突变的方法？](#12-什么是数组检测突变的方法)                                                       |
| 13   | [什么是数组检测非突变方法？](#13-什么是数组检测非突变方法)                                                       |
| 14   | [检测数组变化有什么注意事项？](#14-检测数组变化有什么注意事项)                                                   |
| 15   | [检测对象变化有什么注意事项？](#15-检测对象变化有什么注意事项)                                                   |
| 16   | [如何在一个范围内使用 v-for 指令？](#16-如何在一个范围内使用-v-for-指令)                                         |
| 17   | [如何在模板上使用 v-for 指令？](#17-如何在模板上使用-v-for-指令)                                                 |
| 18   | [如何使用事件处理程序？](#18-如何使用事件处理程序)                                                               |
| 19   | [Vue 提供的事件修饰符是什么？](#19-Vue-提供的事件修饰符是什么)                                                   |
| 20   | [什么是 key 修饰符？](#20-什么是-key-修饰符)                                                                     |
| 21   | [如何自定义 key 修饰符别名？](#21-如何自定义-key-修饰符别名)                                                     |
| 22   | [支持什么系统 keys 修饰符？](#22-支持什么系统-keys-修饰符)                                                       |
| 23   | [支持什么鼠标按钮修饰符？](#23-支持什么鼠标按钮修饰符)                                                           |
| 24   | [如何实现双向绑定？](#24-如何实现双向绑定)                                                                       |
| 25   | [model 支持什么修饰符？](#25-model-支持什么修饰符)                                                               |
| 26   | [组件是什么并给个例子？](#26-组件是什么并给个例子)                                                               |
| 27   | [props 是什么？](#27-props-是什么)                                                                               |
| 28   | [何时需要一个单独的根元素？](#28-何时需要一个单独的根元素)                                                       |
| 29   | [父子组件如何通过事件通信？](#29-父子组件如何通过事件通信)                                                       |
| 30   | [怎样在自定义输入框组件上实现 model？](#30-怎样在自定义输入框组件上实现-model)                                   |
| 31   | [什么时 slots？](#31-什么时-slots)                                                                               |
| 32   | [组件中的全局注册是什么？](#32-组件中的全局注册是什么)                                                           |
| 33   | [为什么你需要本地注册？](#33-为什么你需要本地注册)                                                               |
| 34   | [本地注册和全局注册在模块系统中有什么区别？](#34-本地注册和全局注册在模块系统中有什么区别)                       |
| 35   | [什么是可接受的 prop 类型？](#35-什么是可接受的-prop-类型)                                                       |
| 36   | [props 后面的数据流是什么？](#36-props-后面的数据流是什么)                                                       |
| 37   | [什么是非 prop 属性？](#37-什么是非-prop-属性)                                                                   |
| 38   | [props 有哪些可用的验证？](#38-props-有哪些可用的验证)                                                           |
| 39   | [如何为组件自定义 model 指令？](#39-如何为组件自定义-model-指令)                                                 |
| 40   | [提供给 transitions 什么可能的方式？](#40-提供给-transitions-什么可能的方式)                                     |
| 41   | [什么是 vue router 和它的特性？](#41-什么是-vue-router-和它的特性)                                               |
| 42   | [使用 vue router 路由器的步骤是什么并给出一个例子？](#42-使用-vue-router-路由器的步骤是什么并给出一个例子)       |
| 43   | [什么是动态路由匹配？](#43-什么是动态路由匹配)                                                                   |
| 44   | [如何使路由参数的变化为响应式？](#44-如何使路由参数的变化为响应式)                                               |
| 45   | [什么是路线匹配优先级？](#45-什么是路线匹配优先级)                                                               |
| 46   | [什么是嵌套路由？](#46-什么是嵌套路由)                                                                           |
| 47   | [什么是单文件组件？](#47-什么是单文件组件)                                                                       |
| 48   | [单个文件组件是否违反了关注分离？](#48-单个文件组件是否违反了关注分离)                                           |
| 49   | [单文件组件解决了哪些问题？](#49-单文件组件解决了哪些问题)                                                       |
| 50   | [什么是过滤器？](#50-什么是过滤器)                                                                               |

## 1. VueJS 是什么？

**Vue.js** 是一个开源，用于构建用户界面的渐进式 JavaScript 框架。VueJS 的核心库只关注于`视图层`，并且易于装载和集成其他的库或现有的项目。

## 2. VueJS 的主要功能是什么？

以下是一些 VueJS 可用的主要功能
1. **虚拟 DOM：** 它使用的虚拟 DOM 类似于其他现有的框架，例如 ReactJS，Ember etc。虚拟内存是一个轻量级的在内存中原生 HTML DOM 的表示形式并且不影响原生 DOM 的更新。
2. **组件：** 在 VueJS 应用中用于创建可复用的自定义元素。
3. **模板：** VueJS 提供基于 HTML 的模板并将 DOM 和 Vue 实例的 data 绑定。
4. **路由：** 通过 vue-router 实现页面之间的导航。
5. **轻量：** VueJS 相较于其他框架是一个轻量级的库。

## 3. VueJS 的生命周期方法是什么？

生命周期钩子是一个让你看到你正在使用的库是如何在后台工作的窗口。通过这些钩子，你可以知道你的组件何时被创建、添加进 DOM、更新、及销毁。在详细介绍每一个生命周期钩子之前，让我们一起先看一下生命周期的图表。

<img src="https://github.com/sudheerj/vuejs-interview-questions-chinese/blob/master/images/vuelifecycle.png" width="400" height="800">

1. **Creation(初始化):** Creation 钩子允许你在你的组件被添加进 DOM 之前执行行为。如果你需要在客户端和服务端渲染期间设置一些操作则需要使用这些钩子。不同于其他钩子，creation 在服务端渲染期间也会运行。

    1. beforeCreate: 这个钩子会在你的组件初始化时执行。组件中的钩子监听数据 data 并初始化事件。这时 data 还不是响应式的，并且发生在组件生命周期中的事件还未被设置。
        
    ```javascript
    new Vue({
        data: {
            count: 10
        },
        beforeCreate: function () {
            console.log('Nothing gets called at this moment')
            // `this` 指向视图模型的实例
            console.log('count is ' + this.count);
        }
    })
        // count is undefined
    ```
         
    2. created: 这个钩子会在 Vue 设置了事件并监听 data 之后被调用。这时事件是活跃状态并且能够使用响应式的 data 即使模板还未挂载或渲染。
        
    ```javascript
    new Vue({
        data: {
            count: 10
        },
        created: function () {
            console.log('count is: ' + this.count)
        }
    })
    // count is: 10
    ```
    
    **Note:** 记住这点, 你不能使用 DOM 或 挂载元素目标 (this.$el) 在 creation 钩子中。
        
2. **Mounting(DOM 插入):** Mounting 钩子是最常被用到的，它允许你在第一次渲染之后立即使用你的组件。
    
    1. beforeMount: beforeMount 允许你在组件第一次渲染后立即使用组件。
    
    ```javascript
    new Vue({
        beforeMount: function () {
            // `this` points to the view model instance
            console.log(`this.$el is yet to be created`);
        }
    })
    ```
        
    2. mounted:这个是一个最常被使用的钩子，你可以完全使用响应式的组件、模板、和渲染好的 DOM (via. this.$el)。最常用的模式就是获取组件的数据。
        
    ```javascript
    <div id="app">
        <p>I’m text inside the component.</p>
    </div>
    
    new Vue({
        el: ‘#app’,
        mounted: function() {
            console.log(this.$el.textContent); // I'm text inside the component.
        }
    })
    ```
        
3. **Updating (Diff 并 重新渲染):** Updating 钩子会在你的组件中使用的响应式属性改变或其他原因导致重新渲染时被调用
    
    1. beforeUpdate: beforeUpdate 钩子在你的组件 data 改变并且 update 周期开始后，DOM 的修改并重新渲染前运行。
    
    ```javascript
    <div id="app">
        <p>{{counter}}</p>
    </div>
    ...// rest of the code
    new Vue({
        el: '#app',
        data() {
            return {
            counter: 0
            }
        },
        created: function() {
            setInterval(() => {
                this.counter++
            }, 1000)
        },
        beforeUpdate: function() {
            console.log(this.counter) // Logs the counter value every second, before the DOM updates.
        }
    })
    ```
    
    2. updated: 这个钩子在组件 data 改变且 DOM 重新渲染后运行。
    
    ```javascript
    <div id="app">
        <p ref="dom">{{counter}}</p>
    </div>
    ...//
    new Vue({
        el: '#app',
        data() {
            return {
            counter: 0
            }
        },
        created: function() {
            setInterval(() => {
                this.counter++
            }, 1000)
        },
        updated: function() {
            console.log(+this.$refs['dom'].textContent === this.counter) // Logs true every second
        }
    })
    ```
    
4. **Destruction (拆卸):** Destruction 钩子允许你在你的组件被销毁后执行行为

    1. beforeDestroy: `beforeDestroy` 会在拆卸前被调用。如果你需要清理事件或响应订阅，就应使用 beforeDestroy 去做。
    
    ```javascript
    new Vue ({
        data() {
        return {
            message: 'Welcome VueJS developers'
        }
        },
        beforeDestroy: function() {
            this.message = null
            delete this.message
        }
    })
    ```
    
    2. destroyed: 这个钩子会在组件被销毁，指令解绑且事件监听器被移除后调用。
    
    ```javascript
    new Vue ({
        destroyed: function() {
            console.log(this) // Nothing to show here
        }
    })
    ```

## 4. 条件指令是什么？

VueJS 提供了通过指令基于条件来显示或隐藏元素。可用的指令有：**v-if, v-else, v-else-if and v-show**
    
**1. v-if:**  v-if 指令基于给定的表达式添加或移除 DOM 元素，下面的 button 在 isLoggedIn 被设置为 false 时不会显示。

```html
<button v-if="isLoggedIn">Logout</button>
```

将全部元素都包在一个 `<template>` 元素里这样也可以使用一个 v-if 指令基于条件控制多个元素。例如，你可以将条件同事应用于 label 和 button。

```html
<template v-if="isLoggedIn">
    <label> Logout </button>
    <button> Logout </button>
</template>
```

**2. v-else:**  这个指令只会在相邻的 v-if 条件为 false 时用来显示内容。这类似于任何编程语言中的 else 块用来显示可选的内容，并且在它前面是 v-if 或 v-else-if 块。你不需要传递任何值给它。
例如，v-else 在 isLoggedIn 被设置为 false （未登录）时显示 LogIn 按钮。

```html
<button v-if="isLoggedIn"> Logout </button>
<button v-else> Log In </button>
```

**3. v-else-if:** 当我们需要两个以上选项检查时，就会用到这个指令。
例如，当 ifLoginDisabled 属性被设置为 true 时我们想要显示一些文案替代 LogIn 按钮。这就可以通过 v-else 指令实现。

```html
<button v-if="isLoggedIn"> Logout </button>
<label v-else-if="isLoginDisabled"> User login disabled </label>
<button v-else> Log In </button>
```

**4. v-show:** 这个指令类似于 v-if，但是它会将所有元素渲染到 DOM 中并通过 CSS 的 display 属性来 显示 /隐藏 元素。这个指令被推荐用于需要频繁切换开关的元素。

```html
<span v-show="user.name">Welcome user,{{user.name}}</span>
```
## 5. v-show 和 v-if 指令有什么不同？

以下是一些关于 **v-show** 和 **v-if** 指令的不同点：

1. v-if 只在表达式通过的情况下将元素渲染到 DOM 中，而 v-show 渲染全部元素到 DOM 中并基于表达式使用 CSS display 属性来 显示/隐藏 元素。
2. v-if 支持 v-else 和 v-else-if 指令，而 v-show 不支持 else 指令。
3. v-if 有更高的切换开销，而 v-show 有更高的初始化渲染开销。换言之，如果元素会被频繁切换开关则 v-show 有优势，在初始渲染时间方面 v-if 有优势。
4. v-if 支持 `<template>` 选项卡，但 v-show 不支持。
        
## 6. v-for 指令的目的是什么？

内置的 v-for 指令允许我们循环遍历数组或对象中的每一项。你可以迭代数组或对象中的每一个元素。

1. 数组用法：

```javascript
<ul id="list">
    <li v-for="(item, index) in items">
        {{ index }} - {{ item.message }}
    </li>
</ul>

var vm = new Vue({
    el: '#list',
    data: {
        items: [
            { message: 'John' },
            { message: 'Locke' }
        ]
    }
})
```

你也可以使用 `of` 作为分隔符替代 `in`，类似于 javascript iterators。

2. 对象用法：

```javascript
<div id="object">
    <div v-for="(value, key, index) in user">
        {{ index }}. {{ key }}: {{ value }}
    </div>
</div>

var vm = new Vue({
    el: '#object',
    data: {
        user: {
            firstName: 'John',
            lastName: 'Locke',
            age: 30
        }
    }
})
```

## 7. vue 实例是什么？

每个 Vue 应用工作是通过 Vue function 创建一个新的 Vue 实例。一般只用变量 vm（ViewModel 简写）作为 Vue 实例的引用。你可以像下面这样创建一个 Vue 实例，

```javascript
var vm = new Vue({
    // options
})
```

如上面的代码片段所述，你需要传递选项对象。你可以在 API 参考里找到完整的选项列表。
    
## 8. 如何实现条件组元素？

你可以通过对元素组的不可见（不渲染）包装元素 `<template>` 应用 **v-if** 指令实现条件元素组（一次切换多个元素）。例如，你可以根据有效的用户条件对用户详情分组。

```html
<template v-if="condition">
    <h1>Name</h1>
    <p>Address</p>
    <p>Contact Details</p>
</template>
```
    
## 9. 如何复用有 key 属性的元素？
    
Vue 总是尝试尽可能高效地渲染元素。因此它会试图用重用元素替代从零开始构建。但这种行为会在有些情况下导致一些问题。例如，如果你尝试在 `v-if` 和 `v-else` 块中渲染同样的 input 元素，它将会像下面这样在切换后保留先前的值，

```html
<template v-if="loginType === 'Admin'">
    <label>Admin</label>
    <input placeholder="Enter your ID">
</template>
<template v-else>
    <label>Guest</label>
    <input placeholder="Enter your name">
</template>
```

这种情况下，它不应该重用。我们可以像下面这样在 input 元素上使用 **key** 属性分离，

```html
<template v-if="loginType === 'Admin'">
    <label>Admin</label>
    <input placeholder="Enter your ID" key="admin-id">
</template>
<template v-else>
    <label>Guest</label>
    <input placeholder="Enter your name" key="user-name">
</template>
```

上面的代码确保了两个输入框失独立的，且不会影响彼此。
    
## 10. 为什么不能在同一个元素上同时使用 v-if 和 v-for 指令？

建议不要使用 v-if 和 v-for 在同一个元素上。因为 v-for 指令比 v-if 优先级高。有两种情况下开发者会尝试这种组合，

1. 过滤列表的项。例如，如果你尝试使用 v-if 标记过滤列表，
    
```html
<ul>
    <li
        v-for="user in users"
        v-if="user.isActive"
        :key="user.id"
    >
        {{ user.name }}
    <li>
</ul>
```

这可以使用在初始列表上使用计算属性预过滤来避免。

```javascript
computed: {
    activeUsers: function () {
        return this.users.filter(function (user) {
            return user.isActive
        })
    }
}
...... //
...... //
<ul>
    <li
        v-for="user in activeUsers"
        :key="user.id"
    >
        {{ user.name }}
    <li>
</ul>

```
    
2. 避免渲染应该被隐藏的列表。例如，你想根据条件检查用户是否显示还是隐藏

```html
<ul>
    <li
        v-for="user in users"
        v-if="shouldShowUsers"
        :key="user.id"
    >
        {{ user.name }}
    <li>
</ul>
```

可以移动条件到父级避免对每一个用户检查

```html
<ul v-if="shouldShowUsers">
    <li
        v-for="user in users"
        :key="user.id"
    >
        {{ user.name }}
    <li>
</ul>
```

## 11. 为什么使用 for 指令时需要 key 属性？

为了跟踪每个节点的特征，从而重用和重排存在的元素，你需要为每一个 `v-for` 迭代的项提供一个 `key` 属性。一个理想的 key 值是条目的唯一 id，让我们举个例子，

```html
<div v-for="item in items" :key="item.id">
    {{item.name}}
</div>
```

因此，只要有可能，总是建议给 v-for 提供一个 key 值，除非迭代的 DOM 内容很简单。
**Note:** 不应该使用非基本类型的值，如对象和数组作为 v-for 的 key。使用 String 或 Number 类型替代。

## 12. 什么是数组检测突变的方法？

顾名思义，突变方法修改原生数组。以下列出了能触发视图更新的数组突变方法。

1. push()
2. pop()
3. shift()
4. unshift()
5. splice()
6. sort()
7. reverse()

如果执行以上任何一个突变方法都回触发试图更新。

```javascript
vm.todos.push({ message: 'Baz' })
```

## 13. 什么是数组检测非突变方法？

不改变原始数组但总是返回一个新的数组就叫非突变方法。以下列出了非突变方法，

1. filter()
2. concat()
3. slice()

以一个 todo list 为例，在列表中根据 status 过滤的新数组替换旧数组，

```javascript
vm.todos = vm.todos.filter(function (todo) {
    return todo.status.match(/Completed/)
})
```

由于 VueJS 的实现，这种方法不会重新渲染整个列表。

## 14. 检测数组变化有什么注意事项？

以下两种清空 Vue 不能检测数组的变化，

1. 直接根据索引设置项，例如

```javascript
vm.todos[indexOfTodo] = newTodo
```

2. 修改数组的长度，例如

```javascript
vm.todos.length = todosLength
```

可以通过使用 `set` 和 `splice` 方法克服这两种警告，让我们 看一下解决实例，

**第一个解决方案**

```javascript
// Vue.set
Vue.set(vm.todos, indexOfTodo, newTodoValue)
// (or)
// Array.prototype.splice
vm.todos.splice(indexOfTodo, 1, newTodoValue)
```

**第二个解决方案**

```javascript
vm.todos.splice(todosLength)
```

## 15. 检测对象变化有什么注意事项？

Vue 在对象属性增删时无法检测到更改。以 user 数据改变为例，

```javascript
var vm = new Vue({
    data: {
        user: {
            name: 'John'
        }
    }
})

// `vm.name` is now reactive

vm.email = 'john@email.com' // `vm.email` is NOT reactive
```

可以通过使用 Vue.set(object, key, value) 方法或 Object.assign() 克服这个情况。

```javascript
Vue.set(vm.user, 'email', john@email.com);
(or)
vm.user = Object.assign({}, vm.user, {
    email: john@email.com
})
```

## 16. 如何在一个范围内使用 v-for 指令？

可以使用一个整数作为 v-for 指令重复元素的次数。

```javascript
<div>
    <span v-for="n in 20">{{ n }} </span>
</div>
```

它会显示数字 1-20

## 17. 如何在模板上使用 v-for 指令？

就类似于 v-if 指令在木板上一样，也可以使用带有 v-for 指令的 `<template>` 标签来渲染多个元素块。以 todo 为例，

```javascript
<ul>
    <template v-for="todo in todos">
        <li>{{ todo.title }}</li>
        <li class="divider"></li>
    </template>
</ul>
```

## 18. 如何使用事件处理程序？

你可以在 Vue 中使用类似于纯 JavaScript 的事件处理程序。方法调用也支持特殊的 $event 变量。

```javascript
<button v-on:click="show('Welcome to VueJS world', $event)">
    Submit
</button>

methods: {
    show: function (message, event) {
        // now we have access to the native event
        if (event) event.preventDefault()
        console.log(message);
    }
}
```

## 19. Vue 提供的事件修饰符是什么？

通常，JavaScript 提供了 event.preventDefault() 或 event.stopPropagation() 在事件处理程序中。你可以使用 Vue 提供的方法，但这些方法用于数据逻辑而不是处理 DOM 事件。Vue 为 v-on 提供了以下事件修饰符，`.` 表示指令后缀。

1. .stop
2. .prevent
3. .capture
4. .self
5. .once
6. .passive

以 stop 修饰符为例，

```html
<!-- the click event's propagation will be stopped -->
<a v-on:click.stop="methodCall"></a>
```

也可以像下面这样链接修饰符，

```html
<!-- modifiers can be chained -->
<a v-on:click.stop.prevent="doThat"></a>
```

## 20. 什么是 key 修饰符？

Vue 支持 v-on 的 key 修饰符处理键盘事件。以输入 keycode 的 keyup 事件为例。

```html
<!-- only call `vm.show()` when the `keyCode` is 13 -->
<input v-on:keyup.13="show">
```

记住全部 keycode 真的很难。它支持完整 keycode 列表别名

1. .enter
2. .tab
3. .delete (捕获 “Delete” 和 “Backspace” 键)
4. .esc
5. .space
6. .up
7. .down
8. .left
9. .right

现在上面的代码使用别名重写如下，

```html
<input v-on:keyup.enter="submit">
<!-- (OR) -->
<!-- with shorthand notation -->
<input @keyup.enter="submit">
```

**不赞成使用 keycode 事件，新的浏览器可能会不支持。**

## 21. 如何自定义 key 修饰符别名？

你可以通过全局属性 `config.keyCodes` 自定义 key 修饰符别名。对于这个属性，有一些指导

1. 不能使用驼峰，反而你可以使用带双引号的 kebab-case；
2. 可以使用数组格式定义多个值；

```javascript
Vue.config.keyCodes = {
    f1: 112,
    "media-play-pause": 179,
    down: [40, 87]
}
```

## 22. 支持什么系统 keys 修饰符？

Vue 支持以下修饰符在相应的键被按下时触发鼠标或键盘事件监听器，

1. .ctrl
2. .alt
3. .shift
4. .meta

以 点击事件的 control 修饰符举例，

```html
<!-- Ctrl + Click -->
<div @click.ctrl="doSomething">Do something</div>
```

## 23. 支持什么鼠标按钮修饰符？

Vue 支持以下鼠标按钮修饰符

1. .left
2. .right
3. .middle

举例，以下是 `.right` 修饰符的用法

```html
<button
v-if="button === 'right'"
v-on:mousedown.right="increment"
v-on:mousedown.left="decrement"
/>
```

## 24. 如何实现双向绑定？

可以使用 `v-model` 指令为 input textarea 和选择元素创建数据双向绑定。使用 input 组件举例，

```html
<input v-model="message" placeholder="Enter input here">
<p>The message is: {{ message }}</p>
```

记住，v-model 将忽略任何表单元素上的初始 `value`，`checked` 或 `selected` 属性。
因此总是使用 Vue 实例 data 作为真值来源。

## 25. model 支持什么修饰符？

v-model 指令支持 3 种修饰符。

**1. lazy:** 默认情况下，v-model 在输入框每次 input 事件后同步数据。你可以添加 lazy 修饰符使在 change 事件后同步。

```html
<!-- synced after "change" instead of "input" -->
<input v-model.lazy="msg" >
```

**2. number:** 如果你想将用户输入的自动格式转换为一个数字，你可以给 v-model 添加一个 number 修饰符。即使使用 type="number"，HTML input 元素返回的值总是一个字符串。因此这个类型转换修饰符使很必要的。

```html
<input v-model.number="age" type="number">
```

**3. trim:** 如果你想要将用户输入的空格自动修剪，你可以给 v-model 添加一个 trim 修饰符。

```html
<input v-model.trim="msg">
```

## 26. 组件是什么并给个例子？

组件是一个有名字的可重用 Vue 实例。接受与 new Vue 相同的选项，例如 data computed watch methods 和 生命周期钩子（除了 root 特有一些选项如 el）。以计数器组件为例，

```javascript
// 定义一个叫 button-counter 的组件
Vue.component('button-counter', {
    template: '<button v-on:click="count++">You clicked me {{ count }} times.</button>'
    data: function () {
        return {
        count: 0
        }
    },
})
```

让我们在 new Vue 创建的 Vue 根实例中使用这个组件

```html
<div id="app">
    <button-counter></button-counter>
</div>

var vm = new Vue({ el: '#app' });
```

## 27. props 是什么？

Props 是你可以注册在组件上的自定义属性。当一个值传递给 prop 属性时，它就成为了组件实例的属性。你可以传递一个值的列表作为 props 选项，使用它们类似于模板中的 data 变量。

```javascript
Vue.component('todo-item', {
    props: ['title'],
    template: '<h2>{{ title }}</h2>'
})
```

注册 props 后，可以将它们作为自定义属性传递。

```html
<todo-item title="Learn Vue conceptsnfirst"></todo-item>
```

## 28. 何时需要一个单独的根元素？

每一个模板有 **包含有多个元素** 的组件必须有一个根元素。这种情况下，你需要将元素们通过一个父元素包裹。

```html
<div class="todo-item">
    <h2>{{ title }}</h2>
    <div v-html="content"></div>
</div>
```

否则会抛出一个错误说 "Component template should contain exactly one root element..."。

## 29. 父子组件如何通过事件通信？

如果你想要子元素想父元素通信，在子元素中使用 `$emit` 发出一个事件给父组件，

```javascript
Vue.component('todo-tem', {
props: ['todo'],
template: `
    <div class="todo-item">
    <h3>{{ todo.title }}</h3>
    <button v-on:click="$emit('increment-count', 1)">
        Add
    </button>
    <div v-html="todo.description"></div>
    </div>
`
})
```

现在你可以在父组件中使用这个 todo-item 接收 count 值。

```html
<ul v-for="todo in todos">
    <li>
        <todo-item
        v-bind:key="todo.id"
        v-bind:todo="todo" v-on:increment-count="total += 1"></todo-item>
    </li>
</ul>
<span> Total todos count is {{total}}</span>
```

## 30. 怎样在自定义输入框组件上实现 model？

自定义事件也能被用于创建与 v-model 一起使用的输入框。组件中的 `<input>` 必须遵守以下规则，

1. 绑定 value 到一个 prop 值；
2. input 时，使用新 value 发出自定义 input 事件；

让我们以自定义输入框组件为例

```javascript
Vue.component('custom-input', {
props: ['value'],
template: `
    <input
    v-bind:value="value"
    v-on:input="$emit('input', $event.target.value)"
    >
`
})
```

现在你可以在这个组件上使用 `v-model`

```html
<custom-input v-model="searchInput"></custom-input>
```
## 31. 什么时 slots？

Vue 通过使用 <slot> 元素实现了一个内容分发 API。让我们创建一个带有插入内容 slot 的 alert 组件，

```javascript
Vue.component('alert', {
template: `
    <div class="alert-box">
    <strong>Error!</strong>
    <slot></slot>
    </div>
`
})
```

现在你可以像下面这样动态插入内容，

```javascript
<alert>
    There is an issue with in application.
</alert>
```

## 32. 组件中的全局注册是什么？

全局组件可以在任何注册后创建的 Vue 根实例（new Vue）的模板中使用。全局注册中，使用 Vue.component 创建组件，

```javascript
Vue.component('my-component-name', {
// ... options ...
})
```

选取多个 vue 实例中全局注册的组件，

```javascript
Vue.component('component-a', { /* ... */ })
Vue.component('component-b', { /* ... */ })
Vue.component('component-c', { /* ... */ })

new Vue({ el: '#app' })
```

以上组件可以在 vue 实例中使用，

```javascript
<div id="app">
    <component-a></component-a>
    <component-b></component-b>
    <component-c></component-c>
</div>
```

组件也可以在子组件中使用。

## 33. 为什么你需要本地注册？

由于全局注册，即使你不使用该组件，也会包含在最终的构建中，这将成为程序中不必要的 JavaScript。这可以按以下步骤使用本地注册避免，

1. 首先需要将组件定义为普通的 JavaScript 对象

```javascript
var ComponentA = { /* ... */ }
var ComponentB = { /* ... */ }
var ComponentC = { /* ... */ }
```

本地注册的组件不能再子组件中使用。这种情况下，你需要再组件部分添加他们

```javascript
var ComponentA = { /* ... */ }

var ComponentB = {
    components: {
        'component-a': ComponentA
    },
// ...
}
```

2. 你可以使用 vue 实例组件部分中的组件，

```javascript
new Vue({
    el: '#app',
    components: {
        'component-a': ComponentA,
        'component-b': ComponentB
    }
})
```

## 34. 本地注册和全局注册在模块系统中有什么区别？

在**本地注册**，你需要在组建文件夹中创建每个组件并将它们导入到另一个组件文件的组件部分（components）。假设想要在组件 C 中注册组件 A 和组件 B，配置如下，

```javascript
import ComponentA from './ComponentA'
import ComponentB from './ComponentC'

export default {
components: {
    ComponentA,
    ComponentB
},
// ...
}
```

现在可以在组件 C 中的模板里使用组件 A 和组件 B。

在**全局注册**中，你需要将全部公共或基础组件导出到一个单独的文件中。但是一些流行的打包工具如 `webpack` 通过使用 `require.context` 使得整个过程变得简单。

```javascript
import Vue from 'vue'
import upperFirst from 'lodash/upperFirst'
import camelCase from 'lodash/camelCase'

const requireComponent = require.context(
    // 组件文件夹的相对路径
    './components',
    // 是否在子文件夹中查找
    false,
    // 用于匹配基本组件文件名的正则表达式
    /Base[A-Z]\w+\.(vue|js)$/
)

requireComponent.keys().forEach(fileName => {
    // 获取组件配置
    const componentConfig = requireComponent(fileName)

    // 获取组件的 PascalCase 命名
    const componentName = upperFirst(
        camelCase(
            // 删除文件名的前导 `./` 和扩展名
            fileName.replace(/^\.\/(.*)\.\w+$/, '$1')
        )
    )

    // 全局注册组件
    Vue.component(
        componentName,
        // 在 `.default`上查找组件选项，如果组件是用 `.export default` 导出的，则会存在该选项，
        // 否则会返回到模块的根目录。
        componentConfig.default || componentConfig
    )
})
```

## 35. 什么是可接受的 prop 类型？

你可以声明具有或不具有类型的 props。但建议使用 prop 类型，因为它给组件提供了文档，并会在开发者分配数据类型错误时发出警告。

```javascript
props: {
    name: String,
    age: Number,
    isAuthenticated: Boolean,
    phoneNumbers: Array,
    address: Object
}
```

如上述代码片段所述，你可以像一个对象一样列出 props，其中属性的名称和值分别是 prop 的名称和类型。

## 36. props 后面的数据流是什么？

所有的 props 在子属性和父属性之间遵循一个单向向下的绑定。也就是说，当父属性更新后会将最新的 prop 值传递给子，但不会有其他传递途径（子到父）。子组件不应该改变 prop 否则控制台会报错。
可能的改变 prop 情况可以通过如下方式解决，

1. 当你尝试使用父组件 prop 作为 子组件属性的初始值时：

这种情况下你可以在子组件中定义一个本地属性并分配父组件的值作为初始值

```javascript
props: ['defaultUser'],
data: function () {
    return {
        username: this.defaultUser
    }
}
```

2. 当你尝试转换父组件 prop 时：

你可以定义一个计算属性来使用 prop 的值，

```javascript
props: ['environment'],
computed: {
    localEnvironment: function () {
        return this.environment.trim().toUpperCase()
    }
}
```

## 37. 什么是非 prop 属性？

非 prop 属性是传递给组件但未定义相应的 prop 的属性。
例如，如果您使用的是第三方自定义输入组件 custom-input，该组件需要输入 `data-tooltip` 属性，则可以将此属性添加到组件实例中，

```html
<custom-input data-tooltip="Enter your input" />
```

如果你尝试从父组件传递 prop，子组件中同名的 props 将会被重写。但是 `class` 和 `style` 属性时例外，这些属性会和子组件的合并。

```html
<!-- Child component -->
<input type="date" class="date-control">
<!-- Parent component -->
<custom-input class="custom-class" />
```

## 38. props 有哪些可用的验证？

Vue 提供如类型、必要字段、默认值及自定义验证。你可以提供一个有验证需求的对象，属性值如下，

以用户概况 user profile Vue 组件为例，其中包含合理的验证，

```javascript
Vue.component('user-profile', {
    props: {
        // 基本类型检查（ `null` 匹配任何类型）
        age: Number,
        // 多种可能的类型
        identityNumber: [String, Number],
        // 必要的 字符串
        email: {
            type: String,
            required: true
        },
        // 具有默认值的数字
        minBalance: {
            type: Number,
            default: 10000
        },
        // 具有默认值的对象
        message: {
            type: Object,
            // 对象或数组默认值必须从工厂函数返回
            default: function () {
                return { message: 'Welcome to Vue' }
            }
        },
        // 自定义验证方法
        location: {
            validator: function (value) {
                // 该值必须与这些字符串之一匹配
                return ['India', 'Singapore', 'Australia'].indexOf(value) !== -1
            }
        }
    }
})
```

## 39. 如何为组件自定义 model 指令？

v-model 在组件上使用 **value** 作为 prop，**input** 作为 事件，但是一些 input 类型如 `checkboxes` 和 `radio buttons` 也许需要使用 value 属性给服务端。这种情况下最好自定义 model 属性。让我们以 checkbox 组件为例，

```javascript
Vue.component('custom-checkbox', {
    model: {
        prop: 'checked',
        event: 'change'
    },
    props: {
        checked: Boolean
    },
    template: `
        <input
        type="checkbox"
        v-bind:checked="checked"
        v-on:change="$emit('change', $event.target.checked)"
        >
    `
})
```

现在你可以在这个自定义组件上使用 v-model 如下，

```html
<custom-checkbox v-model="selectFramework"></custom-checkbox>
```

selectFramework 属性将被传递给 checked prop ，并且当 checkbox 组件发出有新值的 change 事件时相同的属性将会更新。

## 40. 提供给 transitions 什么可能的方式？

在插入、更新或从 DOM 中删除项时，Vue 提供 transition 效果的方式有很多种。以下是可能的方式，

1. 自动的 CSS transitions 和 animations 的应用类
2. 集成第三方 CSS 动画库。如 Animate.css
3. 在 transition 钩子期间使用 javascript 直接操作 DOM
4. 集成第三方 JavaScript 动画库。如 Velocity.js

## 41. 什么是 vue router 和它的特性？

Vue Router 是一个为使用 Vue.js 框架设计单页应用的官方路由库。以下是它的特性，

1. 嵌套路由 / 视图映射
2. 模块化、基于组件的路由器配置
3. 路由的 params, query, 通配符
4. 基于 vue transition 系统的试图过渡效果
5. 细粒度的导航控制
6. 带有自动添加 CSS active class 名的链接
7. HTML5 history 模式或 hash 模式, IE9 中自动回退
8. history 模式时返回页面恢复滚动条位置

## 42. 使用 vue router 路由器的步骤是什么并给出一个例子？

在 vue 应用中集成 vue router 是非常容易的。让我们看个例子一步一步说明。

**第一步：** 在模板中配置 router link 和 router view

```html
<script src="https://unpkg.com/vue/dist/vue.js"></script>
<script src="https://unpkg.com/vue-router/dist/vue-router.js"></script>

<div id="app">
    <h1>Welcome to Vue routing app!</h1>
    <p>
        <!-- 使用 router-link 组件和 to 属性进行导航。它会被渲染为一个 <a> 标签 -->
        <router-link to="/home">Home</router-link>
        <router-link to="/services">Services</router-link>
    </p>
    <!-- 路由匹配的组件将会展示在这个路由出口 -->
    <router-view></router-view>
</div>
```

**Step 2:** 引入 Vue 和 VueRouter 包并应用 router

```javascript
import Vue from 'vue';
import VueRouter from 'vue-router';

Vue.use(VueRouter)
```

**Step 3:** 定义或引入路由组件

```javascript
const Home = { template: '<div>Home</div>' }
const Services = { template: '<div>Services</div>' }
```

**Step 4:** 定义每个路由和组件的映射

```javascript
const routes = [
    { path: '/home', component: Home },
    { path: '/services', component: Services }
]
```

**Step 5:** 创建路由实例并传入 `routes` 选项

```javascript
const router = new VueRouter({
    routes // short for `routes: routes`
})
```

**Step 6:**  创建并挂载根实例

```javascript
const app = new Vue({
    router
}).$mount('#app')
```

现在你可以在这个 vue 应用中导航到不同的页面 (Home, Services) 了。

## 43. 什么是动态路由匹配？

有时可能会需要根据一个模式将路由映射到同一个组件。让我们用一个 user 组件，使用动态部分映射，url 如 `/user/john/post/123` 和 `/user/jack/post/235`，

```javascript
const User = {
    template: '<div>User {{ $route.params.name }}, PostId: {{ route.params.postid }}</div>'
}

const router = new VueRouter({
    routes: [
        // 动态部分映射以冒号开始
        { path: '/user/:name/post/:postid', component: User }
    ]
})
```

## 44. 如何使路由参数的变化为响应式？

当您使用带有参数的路由从一个URL导航到另一个URL（用单个组件映射）时，相同的组件实例将被重用。
尽管这样比销毁旧实例再创建个新的更高效，但组件的生命周期钩子函数不会被执行。
这个问题可以使用以下任意一种方式解决，

1. Watch $route 对象:

```javascript
const User = {
    template: '<div>User {{ $route.params.name }} </div>',
    watch: {
        '$route' (to, from) {
            // 响应 route 变化 ...
        }
    }
}
```

2. 使用 beforeRouteUpdate 导航守卫（2.2 版本支持）

```javascript
const User = {
    template: '<div>User {{ $route.params.name }} </div>',
    beforeRouteUpdate (to, from, next) {
        // 响应 route 变化并调用 next()
    }
}
```

beforeRouteEnter 导航守卫没有 `this` 权限。你可以通过将回掉函数传递给 `next` 访问 vm 实例。

## 45. 什么是路线匹配优先级？

有时 URL 可能会被多个路由匹配，这时路由匹配优先级用来解决路由匹配哪个组件的混淆问题。
这个优先级是根据 routes 配置的顺序。换句话说，首先声明的路由具有更高的优先级。

```javascript
const router = new VueRouter({
    routes: [
        { path: '/user/:name', component: User } // 这个路由有更高的优先级
        { path: '/user/:name', component: Admin }
        { path: '/user/:name', component: Customer }
    ]
})
```

## 46. 什么是嵌套路由？

通常来说，应用程序由嵌套的多层深度的组件组成。URL 的一部分对应了这些嵌套组件的一个确定结构。要将组件渲染在嵌套的出口，需要在 `VueRouter` 构造器配置中使用 `children` 选项。
让我们看一个有各自路由的 profile 和 posts 组件组成的 user app。当没有匹配的嵌套路由时，你也可以定义一个默认路由。

```javascript
const router = new VueRouter({
    routes: [{
        path: '/user/:id',
        component: User,
        children: [
            {
                // 当匹配 /user/:id/profile 时 UserProfile 将渲染在 User's <router-view> 中
                path: 'profile',
                component: UserProfile
            }, {
                // 当匹配 /user/:id/posts 时 UserPosts 将渲染在 User's <router-view> 中
                path: 'posts',
                component: UserPosts
            }, {
                // 当匹配 /user/:id/ 时 UserHome 将渲染在 User's <router-view> 中
                path: '',
                component: UserHome
            },
        ]
    }]
})
```

## 47. 什么是单文件组件？

单文件组件是一个容易理解的概念。你之前可能听说过应用程序的三个部分（HTML，JavaScript，CSS）都放在不同的文件中。但是单个文件组件将结构、样式和行为封装到一个文件中。一开始，在一个文件中包含这三个部分似乎很奇怪，但实际上它更有意义。
让我们看一个单文件组件的例子

```html
<template>
    <div>
        <h1>Welcome {{ name }}!</h1>
    </div>
</template>

<script>
    module.exports = {
        data: function() {
            return {
                name: 'John'
            }
        }
    }
</script>

<style scoped>
    h1 {
        color: #34c779;
        padding: 3px;
    }
</style>
```

## 48. 单个文件组件是否违反了关注分离？

就最新的现代 UI 开发来说，关注分离并不等于文件类型分离。所以最好将代码基层划分为低耦合的组件并组合使用，而不是划分为很大的互相混杂的三层。
通过将模板、逻辑、样式合并在一个组件中的这种方式使得单文件组件高内聚和更好的可维护性。
你仍然可以通过热重载和预编译的功能坚持将 JavaScript 和 CSS 文件分离。例如，

```html
<template>
    <div>This section will be pre-compiled and hot reloaded</div>
</template>
<script src="./my-component.js"></script>
<style src="./my-component.css"></style>
```

## 49. 单文件组件解决了哪些问题？

单文件组建解决了 .vue js 驱动应用中出现的常见问题。问题清单如下，

1. 全局定义强制每个组件的唯一名称
1. 字符串模板缺少语法高亮并且需要在多行 HTML 后加难看的斜线
3. 不支持 CSS 意味着虽然 HTML 和 JavaScript 被模块化为组件，但 CSS 明显遗漏了
4. 没有构建步骤限制我们使用 HTML 和 ES6

## 50. 什么是过滤器？

过滤器可用于应用普通的文本格式。过滤器应该加到 JavaScript 表达式的末尾，由“管道”（竖线）表示。你可以在两种特定情况下使用：

1. mustache 插值（双花括号）
2. v-bind 表达式

例如，我们在组件的选项中定义一个名为 capitalize 的过滤器

```javascript
filters: {
    capitalize: function (value) {
        if (!value) return ''
        value = value.toString()
        return value.charAt(0).toUpperCase() + value.slice(1)
    }
}
```

现在你可以在 mustache 插值或 v-bind 表达式中使用 filter，

```html
<!-- in mustaches -->
{{ username | capitalize }}

<!-- in v-bind -->
<div v-bind:id="username | capitalize"></div>
```
# Chunk

继承自KISSY的Base，是brick和pagelet类的父类


        设计思路:基类，作为组件底层，完成渲染、数据更新、销毁操作，是模板解析器（Tmpler）和数据管理器（Dataset）的调度者。

## 配置

* `el` {element}

    组件节点，只读。

* `rendered` {Boolen}

    是否已经渲染到页面，只读

* `render` {String|element}

    容器节点

* `tmpl` {String}

    模板字符串

* `autoRender` {Boolen}

    是否自动渲染

## 方法

* `render()`

    将模板渲染到页面

* `setChunkData(datakey, data)`

    设置数据，并刷新模板数据

    * @param {string} datakey 需要更新的数据对象key
    * @param {object} data    数据对象

* `addTmpl(id, arr)`

    给brick添加模板

    * @param {string} id  brick的id
    * @param {array} arr 模板数组

* `destroy()`

    销毁组件或者pagelet


## 事件

* `rendered`

    将模板渲染到页面中触发






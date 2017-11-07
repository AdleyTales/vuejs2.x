# vuejs2.x

> vue2 vue-router vuex axios vue-cli webpack ES6

## vuejs@2.x

官网： [https://cn.vuejs.org/](https://cn.vuejs.org/)

---
# 正式开始：



#### 生命周期：

    1.beforeCreate()： 组件实例刚刚被创建，属性都没有

    2.created()：实例已经创建完成，属性已经绑定

    3.beforeMount()：模板编译之前

    4.mounted()：模板编译完成

    5.beforeUpdate(): 组件更新之前

    6.updated():组件更新完毕

    7.beforeDestroy():组件销毁前

    8.destroyed(): 组件销毁之后     


#### 循环：

    2.0循环默认可以添加重复数据

    去掉隐式循环：

        ul>
            <li v-for="(val,index) in list" >
                {{val}}  {{index}}
            </li>
        </ul>    

    track-by ==> :key="index" 提升循环性能

#### 自定义键盘指令：

    Vue.config.keyCodes.ctrl = 17;

    @keyup.ctrl = "change"

#### 过滤器：

    去掉所有1.0内置的过滤器

    一些简单功能，自己通过js实现

    自定义过滤器：

        Vue.filter('toDou',function(n){return })

        {{msg | toDou('12','5')}}

补充：lodash 工具库 _库

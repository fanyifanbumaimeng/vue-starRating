# vue-starLevelComponent

> 一款vue 的评分插件。


## 运行DEMO项目

```
下载然后打开starRating页面
```
## 特点
1. 简单易用，提供显示和评分两种模式
2. 支持四舍五入，向上取整，向下取整，默认四种模式
3. 提供单独以组件的方式按需引入

## 获取


## 用法

```

### 以组件的形式安装
```
// 在组件中导入插件
import starRating from './starRating/starRating.vue'
// 在组件中注册插件
export default {
  components: { starRating }
}
// 在组件的 temelate 中直接使用
        <star-Rating
                :score=3.2
                :can-Choose=true
                :mode="roundUp"
                v-on:change="afterClick"
        ></star-Rating>
```

## 选项
你可以通过在所在的元素上设置以下属性来配置`starRating`
1. `mode`：默认不进行四舍五入，显示半星
    'round'代表四舍五入
    'roundUp'代表向上取整
    'roundDown'代表向下取整
2. `canChoose'，是否是评分模式，默认为false显示模式，true为评分模式
3. 'score'，单个评分，跟max总分配合使用，默认max为5.

## 事件
`change` 点击进行评分时进行触发


# vue-css-spinner

> VueJS CSS 加载动画组件

## Use

拷贝 `src/components/*.vue` 至你项目的 `src/components` 内

HTML部分
``` html
<spinner></spinner>
```
JS部分
``` js
//import components
import spinner from './src/components/*'

//use components
...
	components: {
		spinner
	}
...
```
另外，你可以用css自定义组件的位置

## 参数表

#### circleLine | Windows8 加载动画样式

| Parameter | Required |   Type  |   Description   |  Example  |
|:---------:| -------- | ------- | --------------- |:---------:|
| `loading` | false    | Boolean | show            | true      |
| `color`   | false    | String  | spinner's color | #F45757   |

#### dot | Google 四色小点

| Parameter | Required |   Type  |   Description   |  Example  |
|:---------:| -------- | ------- | --------------- |:---------:|
| `loading` | false    | Boolean | show            | true      |
| `size`    | false    | Number  | spinner's size  | 10        |
| `color`   | false    | Array   | dot's color     | ['#4285F4', '#DB4437', '#F4B400', '#0F9D58'] |


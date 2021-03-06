# Vue CSS Spinner

> VueJS CSS Loader

## [Live demo](http://jas0ncn.github.io/vue-css-spinner/)

## How to use

Copy one of spinners from `src/components/*.vue` into your project `src/components`

Insert HTML like this
``` html
<spinner></spinner>
```
Import components and add component to `components`
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
Besides,you can add the component's location by CSS

## Parameter list

#### circleLine | Windows8 style

| Parameter | Required |   Type  |   Description   |  Example  |
|:---------:| -------- | ------- | --------------- |:---------:|
| `loading` | false    | Boolean | show            | true      |
| `color`   | false    | String  | spinner's color | #F45757   |

#### dot | Google dots style

| Parameter | Required |   Type  |   Description   |  Example  |
|:---------:| -------- | ------- | --------------- |:---------:|
| `loading` | false    | Boolean | show            | true      |
| `size`    | false    | Number  | spinner's size  | 10        |
| `color`   | false    | Array   | dot's color     | ['#4285F4', '#DB4437', '#F4B400', '#0F9D58'] |


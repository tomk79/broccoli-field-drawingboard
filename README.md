# broccoli-field-drawingboard

drawingboard.js plugin for broccoli-html-editor

## Install

```
$ composer require tomk79/broccoli-field-drawingboard
```

## Usage

### Client Side Option

```html
<script src="/path/to/broccoli-field-drawingboard/dist/broccoli-field-drawingboard.js"></script>
<script>
var broccoli = new Broccoli();
broccoli.init(
	{
		/* 中略 */
		'customFields': {
			'drawingboard': window.broccoliFieldDrawingboard
		},
		/* 中略 */
	} ,
	function(){
		/* 中略 */
	}
);
</script>
```

### Server Side Option

```js
var Broccoli = require('broccoli-html-editor');
var broccoli = new Broccoli();
var broccoliFieldDrawingboard = require('broccoli-field-drawingboard');

// 初期化を実行してください。
broccoli.init(
	{
		/* 中略 */
		'customFields': {
			'drawingboard': broccoliFieldDrawingboard
		} ,
		/* 中略 */
	},
	function(){
		/* 中略 */
	}
);
```

### Module Template Sample

```
<img src="{&{"input":{"type":"drawingboard","name":"main"}}&}" alt="" />
```

## 更新履歴 - Change log

### broccoli-field-drawingboard@0.1.0-beta.1 (2016年??月??日)

- initial release.

## ライセンス - License

MIT License


## 作者 - Author

- Tomoya Koyanagi <tomk79@gmail.com>
- website: <http://www.pxt.jp/>
- Twitter: @tomk79 <http://twitter.com/tomk79/>

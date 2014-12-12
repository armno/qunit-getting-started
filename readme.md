# first qunit test

i'm learning to get start with tdd with jquery. qunit is the first testing framework i pick.

install jquery (of course we'll need jquery)

```sh
$ bower install --save jquery
```

then install qunit as a devDependency

```sh
$ bower install --save-dev qunit
```

create `index.html`

```html
<!doctype html>
<html>
	<head>
		<!-- bower:css -->
		<!-- endbower -->
	</head>
	<body>

		<!-- bower:js -->
		<!-- endbower -->
	</body>
</html>
```

use `wiredep` to include bower components in the page.

```sh
$ npm install --save-dev wiredep
```

```sh
$ node
> require('wiredep')({src: 'index.html', devDependencies: true});
```

start http server using `http-server`

```sh
$ npm install --save-dev http-server
$ http-server .
```

add these 2 `<div>`s in `<body>` tag.

```html
...
<body>
	<div id="qunit"></div>
	<div id="qunit-fixure"></div>
...
</body>
```

reload the page. qunit results should show up.

![qunit page](screeshots/01.png)
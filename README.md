# css-grid-framework

This is my personal implementation of a css 12 column grid framework. 

#### Resets: 
[Normalize.css](https://necolas.github.io/normalize.css/)

#### Preprocessor:
[Sass](http://sass-lang.com/)

#### Usage:
```
<!Doctype html>
<html>
<head> 
  <meta charset="utf-8">
	<title>CSS-Grid-Framework</title>
	<link href="normalize.css">
	<link rel="stylesheet" href="stylesheets/output.css" type="text/css">
</head>
<body>
	<div class="container">
		<div class="row">
			<div class="col-6">
				<p> this columns width is 50% of the page.</p>
			</div>
			<div class="col-3">
				<p> this columm width is 25% of the page.</p>
			</div>
			<div class="col-3">
				<p> this columm width is 25% of the page.</p>
			</div>
		</div>
	</div>
</body>
</html>
```
* Include the css reset inside the head tag ```<link href="normalize.css">```
* Include the stylesheet ```<link rel="stylesheet" href="stylesheets/output.css" type="text/css">```
* Make sure in each row that the sum of the columns is 12.
* Default gutters(padding between each column) is set to 10px by default. 

#### Breakpoints:
Breakpoint is set for any screen less than 800px.
```
@media screen and(max-width:800px){
	[class*="col-"]{width:100%;}
}
```

### Sample
![Image Hover Text](/ss.png)
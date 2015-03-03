# planck

v1.1.0

The worlds smallest CSS grid system.

## Size

- **272 bytes** minified 
- **165 bytes** gzipped  
(minus comments)

## Usage

- Include `planck.min.css` within the `<head>` of your HTML:
	
```html
	<head>
		<link rel="stylesheet" href="planck.min.css">
	</head>
```

- Example structure:

```html
	<div class="x6">
		<!--full width-->
	</div>
	<div class="x2">
		<!--one-third column-->
	</div>
	<div class="x2">
		<!--one-third column-->
	</div>
	<div class="x2">
		<!--one-third column-->
	</div>
```

## Caution

planck uses the [prefix attribute selector](https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors) `[attr^=value]` 

- planck classes `x1` to `x6` **must** be specified **first** within your class definition:

*Good*
```html
	<div class="x3 class">
```
*Bad*
```html
	<div class="class x3">
```

- You can't start with a non planck class definition that begins with `x`:

*Good*
```html
	<div class="x4 xlyophone">
```
*Bad*
```html
	<div class="xylophone">
```

## Notes

- Based on [g.css](https://github.com/edsloan/g.css)
- Author(s): [@edsloan](https://twitter.com/edsloandev)
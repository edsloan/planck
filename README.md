# planck

v1.2.1

The worlds smallest CSS grid system.

It's **218 bytes** minified and **150 bytes** gzipped (minus the comments).

## Usage

- Include `planck.min.css` within the `<head>` of your HTML:
	
```html
	<head>
		<link rel="stylesheet" href="planck.min.css">
	</head>
```

- Example structure:

```html
<div class="r">
	<div class="x6">
		<!--full-width column-->
	</div>
</div>
<div class="r">
	<div class="x2">
		<!--one-third column-->
	</div>
	<div class="x2">
		<!--one-third column-->
	</div>
	<div class="x2">
		<!--one-third column-->
	</div>
</div>
```

## Caution

planck uses the [prefix attribute selector](https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors) `[attr^=value]`, so:

- planck classes `x1` to `x6` **must** be specified **first** within your class definition:

*Good*
```html
	<div class="x3 class">
```
*Bad*
```html
	<div class="class x3">
```

- You can't start with a non planck class definition that begins with the letter `x`:

*Good*
```html
	<div class="x4 xlyophone">
```
*Bad*
```html
	<div class="xylophone">
```

## Notes

- Support: Chrome 10+, Firefox 29+, Safari 5.1+, IE 9+, Opera 9.2+, iOS Safari 5.1+ & Android 4+
- Based on [g.css](https://github.com/edsloan/g.css)
- Author(s): [@edsloan](https://twitter.com/edsloandev)
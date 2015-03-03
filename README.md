# planck

v1.0.1

The worlds smallest CSS grid system.

## Size

- **284 bytes** minified 
- **168 bytes** gzipped  
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

- Planck uses the [prefix attribute selector](https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors) `[attr^=value]`, so the column classes `x1` to `x6` **must** be specified **first** within your markup.

## Notes

- Based on [g.css](https://github.com/edsloan/g.css)
- Author(s): [@edsloan](https://twitter.com/edsloandev)
# Spectre.css notes

## Spectre.css source
* [spectre.css](https://github.com/picturepan2/spectre/blob/master/docs/dist/spectre.css)
* [spectre-exp.css (experimentals)](https://github.com/picturepan2/spectre/blob/master/docs/dist/spectre-exp.css)
* [dist directory](https://github.com/picturepan2/spectre/tree/master/docs/dist)
* [spectre.scss](https://github.com/picturepan2/spectre/blob/master/src/spectre.scss)

## Official docs

* [Elements](https://picturepan2.github.io/spectre/elements.html)
* [Layout](https://picturepan2.github.io/spectre/layout.html)
  * [Navbar](https://picturepan2.github.io/spectre/layout.html#navbar)
* [Components](https://picturepan2.github.io/spectre/components.html)
  * [Tabs](https://picturepan2.github.io/spectre/components.html#tabs)
* [Utilities](https://picturepan2.github.io/spectre/utilities.html)
  * [Colors, both semantic and named background colors](https://picturepan2.github.io/spectre/utilities.html#colors)
  * [Horizontal and vertical dividers](https://picturepan2.github.io/spectre/utilities.html#display)
  * [Positioning for layout, float, margins](https://picturepan2.github.io/spectre/utilities.html#position)
  * [Shaped divs](https://picturepan2.github.io/spectre/utilities.html#shapes)
  * [Text](https://picturepan2.github.io/spectre/utilities.html#text)

## Layout

### Navbar

* Their navbar is horizontal and meant for headers only. They don't have a vertical style for left-side navbars.
* I think my navbar is semantically better than theirs because it avoids using `<section>` tags for formatting purposes:

```html
<header class="navbar" style="margin-top: 3rem;" >
	<!-- Logo on the left -->
	<div class="navbar-section">	
		<a href="#" class="navbar-brand">Project name</a>
	</div>
	<div class="navbar-section">	
		<a href="#" class="btn btn-link selected">Home</a>
		<a href="#" class="btn btn-link">About</a> 
		<a href="#" class="btn btn-link">Contact</a> 
	</div>
</header><!-- .navbar -->
````
## Styles

### .navbar-brand

Style used for a distinguished text element on the navbar, typically indicate a logo or homepage

## Questions
* It looks like the links in [Navbars](https://picturepan2.github.io/spectre/layout.html#navbar) should be styled using the 
* Does the `mr-2` style still exist? See [Navbar example](https://picturepan2.github.io/spectre/layout.html#navbar). It seems like it would be in the [Position Utilities](https://picturepan2.github.io/spectre/utilities.html#position) section.

## Contribution ideas
* Add a [Tabs](https://picturepan2.github.io/spectre/components.html#tabs) section to table of contents on left nav!

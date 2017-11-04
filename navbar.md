## Navbars

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

### Using vertical navbar when screen size is smaller

This example shows how to use a horizontal navbar for screen sizes >= 600 and a vertical one when smaller than 600

```html
		<header class="navbar">
		
			<!-- Horizontal navbar for large form-factor, like desktop or wide phone -->
			<!-- hide-sm means hide when window is <= 600px wide -->
			<!-- Logo on the left -->
			<div class="navbar-section hide-sm">	
				<a onclick="togglePage(this)" href="#" class="navbar-brand">Project name</a>
				<a onclick="togglePage(this)" href="#" data-id="home-page" class="btn btn-link selected">Home</a>
				<a onclick="togglePage(this)" href="#" data-id="about-page" class="btn btn-link">About</a> 
				<a onclick="togglePage(this)" href="#" data-id="contact-page" class="btn btn-link">Contact</a> 
			</div>
			
			<!-- Vertical nav when form factor is smaller -->
			<!-- This example omits the Home link just to show the navigations can be different. -->
			<!-- show-sm means display when window is <= 600px wide -->
			<ul class="nav show-sm">
				<li class="menu-item">
					<a onclick="togglePage(this)" href="#" data-id="home-page" class="btn btn-link selected">Home</a>
				</li>
				<li class="menu-item">
					<a onclick="togglePage(this)" href="#" data-id="about-page" class="btn btn-link">About</a> 
				</li>
				<li class="menu-item">
					<a onclick="togglePage(this)" href="#" data-id="contact-page" class="btn btn-link">Contact</a> 
				</li>
			</ul>
			
			
		</header><!-- .navbar -->
```	            

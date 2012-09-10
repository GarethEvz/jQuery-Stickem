Make items sticky as you scroll, to a point.

## Usage

<pre>&lt;div class="container">
	&lt;div class="row stickem-container">
		&lt;div class="content">
			Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
		&lt;/div>
		
		&lt;div class="aside stickem">
		  I'm gonna be sticky!
		&lt;/div>
	&lt;/div>
&lt;/div></pre>

<pre>.stickem-container {
  position: relative;
}

.stickit {
	margin-left: 660px;
	position: fixed;
	top: 0;
}

.stickit-end {
	bottom: 40px;
	position: absolute;
	right: 0;
}</pre>

<pre>$('.container').stickem();</pre>

### Defaults

*item: '.stickem'*
Items that you want to stick on scroll.

*container: '.stickem-container'*
Container that you want the sticky item to be contained in.

*stickClass: 'stickit'*
Class added to the sticky item once it should start being sticky.

*endStickClass: 'stickit-end'*
Class added to the sticky item once it has reached the end of the container

*offset: 0*
Do you already have a fixed horizontal header on the page? Offset stick 'em by that many pixels.

*start: 0*
If your sticky item isn't at the top of the container, tell it where it should start being sticky.
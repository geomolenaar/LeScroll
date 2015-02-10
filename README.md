# LeScroll
One page scrolling, written in vanilla JavaScript with CSS transitions. 

# Features
Keyboard navigation
Mouse wheel navigation
Bullet navigation
Responsive

# Compatibility
Works with all modern browsers that support CSS3. In the next version IE8 en IE9 will be supported.

# Basic usage
Scroll through the different sections either using the keyboard, mouse wheel or bullet navigation on the right.

# HTML Structure
<pre>	
	<div id="mask">
		<nav>
			<ul>
				<li data-section="0"></li>
				<li data-section="1"></li>
		        <li data-section="2"></li>
				<li data-section="3"></li>
			</ul>
		<div id="container">
			<section>
				Section 1
			</section>
			<section>
				Section 2
			</section>
			<section>
				Section 3
			</section>
			<section>
				Section 4
			</section>
		</div>
	</div>
	<script src="scripts/lescroll.min.js"></script>
</pre>
# Add new section
Simply add a new <section> tag to your html, don't forget to add an extra li with the following data-section

# Public methods
If you want to link a button or other element to a certain section you can use the .addEvent function
<pre>
	To add a class use:
	leScroll.addEvent('.arrowdown', 1);
	To add an ID use:
	leScroll.addEvent('#clickme', 0);
</pre>

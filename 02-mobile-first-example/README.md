Here's a simple example of a mobile-first design using HTML and CSS. In this example, we'll create a basic navigation menu that is initially designed for mobile devices and then progressively enhanced for larger screens.

HTML (index.html):

```html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" type="text/css" href="styles.css" />
    <title>Mobile-First Design Example</title>
  </head>
  <body>
    <header>
      <h1>Website Name</h1>
      <nav>
        <div class="menu-icon">&#9776;</div>
        <ul class="nav-links">
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <!-- Content goes here -->
    </main>
  </body>
</html>
```

CSS (styles.css):

```css
/* Mobile-First Styles */
body {
  font-family: Arial, sans-serif;
}

header {
  background-color: #333;
  color: #fff;
  padding: 10px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h1 {
  margin: 0;
}

.nav-links {
  list-style: none;
  padding: 0;
  display: none;
}

.nav-links li {
  margin: 10px 0;
}

.menu-icon {
  font-size: 24px;
  cursor: pointer;
  display: block;
}

/* Media Query for Larger Screens */
@media screen and (min-width: 768px) {
  .nav-links {
    display: block;
  }

  .nav-links li {
    display: inline;
    margin: 0 15px;
  }

  .menu-icon {
    display: none;
  }
}
```

In this example:

1. The HTML structure includes a mobile-friendly navigation menu with a "hamburger" menu icon initially hidden and a list of navigation links hidden as well.

2. In the CSS, mobile-first styles are applied first. The navigation links and menu icon are hidden, and the header is styled for mobile screens.

3. Then, a media query (`@media screen and (min-width: 768px)`) is used to apply styles for screens with a minimum width of 768 pixels (which could represent larger screens like tablets or desktops). In this query, we display the navigation links as a horizontal list and hide the menu icon.

This example demonstrates the mobile-first design principle by starting with a clean and simple mobile layout and progressively enhancing it for larger screens using CSS media queries.

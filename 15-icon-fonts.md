# Icon Fonts

Bootstrap 5 introduced several changes, including the removal of Glyphicons, which were the default icon font used in previous versions of Bootstrap. Glyphicons were removed due to licensing issues and to encourage developers to use custom icons or third-party icon libraries. Therefore, Bootstrap 5 no longer includes Glyphicons by default.

However, Bootstrap 5 does provide flexibility and guidance on how to use custom icons or third-party icon libraries with your Bootstrap projects. You have several options:

1. **Custom Icons**: You can use your custom icons in Bootstrap 5. This typically involves creating your icon font or using vector icons in SVG format and then adding them to your project's assets. You can then use CSS to apply these custom icons to elements in your HTML.

2. **Third-Party Icon Libraries**: Bootstrap 5 recommends using third-party icon libraries like Font Awesome, Feather Icons, or Material Icons. These libraries offer a wide range of icons that you can easily integrate into your Bootstrap projects. To use them, you include the library's CSS or JavaScript files in your project and use their respective classes or markup to add icons to your elements.

   Example using Font Awesome:

   ```html
   <!-- Include Font Awesome CSS -->
   <link
     href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
     rel="stylesheet"
   />

   <!-- Add a Font Awesome icon -->
   <i class="fas fa-home"></i> Home
   ```

   In this example, we're using Font Awesome to add a home icon to the page.

3. **SVG Icons**: You can also use SVG icons directly in your Bootstrap 5 project by including SVG markup in your HTML. SVG icons are highly customizable and can be easily styled using CSS.

   Example using an SVG icon:

   ```html
   <!-- Add an SVG icon -->
   <svg
     xmlns="http://www.w3.org/2000/svg"
     width="16"
     height="16"
     fill="currentColor"
     class="bi bi-house"
     viewBox="0 0 16 16"
   >
     <path
       d="M.293 7.293a1 1 0 0 1 1.414-1.414L8 13.586V2a1 1 0 0 1 2 0v11.586l6.293-6.293a1 1 0 1 1 1.414 1.414l-7 7a1 1 0 0 1-1.414 0l-7-7a1 1 0 0 1-.001-1.414z"
     />
   </svg>
   Home
   ```

   In this example, we're using an inline SVG icon for the home icon.

Remember that the specific implementation details may vary depending on the icon library or custom icons you choose to use. It's essential to refer to the documentation of the icon library or your custom icon solution for detailed instructions on how to integrate and use icons in your Bootstrap 5 project. Additionally, please check for any updates or changes that may have occurred in Bootstrap 5 since my last knowledge update in September 2021.

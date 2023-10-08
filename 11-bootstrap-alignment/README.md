# Bootstrap alignment

Here's an example of a blog post about great writers using Bootstrap's alignment classes for various elements such as images, text, and headings. This example demonstrates how to use Bootstrap to align and style the content in a blog post:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
    <title>Blog Post about Great Writers</title>
  </head>
  <body>
    <div class="container">
      <h1 class="mt-5 text-center">Great Writers: Masters of Words</h1>
      <p class="text-muted text-center">
        Published on October 15, 2023 by John Doe
      </p>

      <img
        src="writer.jpg"
        alt="Great Writer"
        class="img-fluid rounded mx-auto d-block my-4"
        width="300"
      />

      <div class="row">
        <div class="col-md-8 offset-md-2">
          <p class="lead text-justify">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus
            condimentum efficitur semper. Integer bibendum sapien quis nunc
            bibendum, ut congue quam tempus. Curabitur eu odio nec nisi gravida
            facilisis at eu justo.
          </p>

          <p class="text-justify">
            Sed vel finibus quam, vel efficitur nulla. Nullam ac dapibus lectus.
            Fusce dapibus, urna in facilisis euismod, est erat egestas enim, eu
            dapibus tellus augue nec justo.
          </p>

          <blockquote class="blockquote">
            <p class="mb-0">
              "A writer is someone for whom writing is more difficult than it is
              for other people."
            </p>
            <footer class="blockquote-footer">Thomas Mann</footer>
          </blockquote>

          <p class="text-justify">
            In this blog post, we will explore the lives and works of some of
            the greatest writers in history. These literary giants have left an
            indelible mark on the world through their words and stories.
          </p>

          <p class="text-center">
            <img
              src="book.jpg"
              alt="Books"
              class="img-fluid rounded my-4"
              width="400"
            />
          </p>

          <h2 class="text-center">Jane Austen</h2>
          <p class="text-center">
            Jane Austen was an English novelist known for her six major novels,
            including "Pride and Prejudice" and "Sense and Sensibility." Her
            keen social commentary and wit continue to captivate readers
            worldwide.
          </p>
        </div>
      </div>

      <p class="text-center mt-5">
        <a href="#" class="btn btn-primary btn-lg">Read More</a>
      </p>
    </div>
  </body>
</html>
```

In this example:

- Bootstrap classes like `text-center`, `text-justify`, `img-fluid`, `rounded`, `my-4`, and `mt-5` are used to control the alignment, spacing, and styling of various elements in the blog post.

- The `text-center` class is used to center-align headings and buttons.

- The `text-justify` class is used for justified text alignment.

- `img-fluid` ensures that images are responsive and fit within their container.

- `rounded` adds rounded corners to images.

- `my-4` and `mt-5` control the vertical spacing (margins) between elements.

- A blockquote is used for a quote, and Bootstrap's `blockquote` and `blockquote-footer` classes are applied.

- The Bootstrap grid system is utilized to center-align the content within a column.

This example showcases how to structure and style a blog post about great writers using Bootstrap's alignment and spacing classes to create a visually appealing and readable layout. You can further customize the styles and content to suit your specific needs.

## How would you make text-center into a responsive class that will only apply to LG viewports and up?

To make the `text-center` class apply only to LG (large) viewports and up, you can use Bootstrap's responsive utility classes. In this case, you can use the `text-lg-center` class. Here's how you can modify the previous example to achieve this:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
    <title>Blog Post about Great Writers</title>
  </head>
  <body>
    <div class="container">
      <h1 class="mt-5 text-lg-center">Great Writers: Masters of Words</h1>
      <p class="text-muted text-center">
        Published on October 15, 2023 by John Doe
      </p>

      <!-- ... (the rest of the content) ... -->
    </div>
  </body>
</html>
```

In the modified example, we've changed the `text-center` class for the main heading to `text-lg-center`. This will center-align the heading text only on LG (large) viewports and larger screens. On smaller screens, the text will remain left-aligned.

This way, you can apply responsive text alignment using Bootstrap's responsive utility classes to control how the text is aligned on different screen sizes.

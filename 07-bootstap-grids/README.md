# Bootstrap 5 grids

In Bootstrap 5, you can create a responsive grid system using 12 columns within a single row. Below is an example that demonstrates how to set up a grid system with varying column widths, from 12 columns in a single row to 1 column in a single row.

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
    <title>Bootstrap 5 Grid Example</title>
  </head>
  <body>
    <div class="container">
      <h1>Bootstrap 5 Grid Example</h1>

      <!-- 12 Columns in 1 Row -->
      <div class="row">
        <div class="col">1 of 12</div>
        <div class="col">2 of 12</div>
        <div class="col">3 of 12</div>
        <div class="col">4 of 12</div>
        <div class="col">5 of 12</div>
        <div class="col">6 of 12</div>
        <div class="col">7 of 12</div>
        <div class="col">8 of 12</div>
        <div class="col">9 of 12</div>
        <div class="col">10 of 12</div>
        <div class="col">11 of 12</div>
        <div class="col">12 of 12</div>
      </div>

      <!-- 6 Columns in 1 Row -->
      <div class="row">
        <div class="col-md-2">1 of 6</div>
        <div class="col-md-2">2 of 6</div>
        <div class="col-md-2">3 of 6</div>
        <div class="col-md-2">4 of 6</div>
        <div class="col-md-2">5 of 6</div>
        <div class="col-md-2">6 of 6</div>
      </div>

      <!-- 4 Columns in 1 Row -->
      <div class="row">
        <div class="col-md-3">1 of 4</div>
        <div class="col-md-3">2 of 4</div>
        <div class="col-md-3">3 of 4</div>
        <div class="col-md-3">4 of 4</div>
      </div>

      <!-- 3 Columns in 1 Row -->
      <div class="row">
        <div class="col-md-4">1 of 3</div>
        <div class="col-md-4">2 of 3</div>
        <div class="col-md-4">3 of 3</div>
      </div>

      <!-- 2 Columns in 1 Row -->
      <div class="row">
        <div class="col-md-6">1 of 2</div>
        <div class="col-md-6">2 of 2</div>
      </div>

      <!-- 1 Column in 1 Row -->
      <div class="row">
        <div class="col-md-12">1 of 1</div>
      </div>
    </div>
  </body>
</html>
```

In this example:

- We use the `.container` class to create a responsive container that limits the maximum width of the content.
- Inside the container, we create multiple rows (`.row`) and assign column classes (`.col`) to the content within each row to define the desired column layout.
- We vary the number of columns in each row, from 12 columns (the full width) to 1 column, to demonstrate different grid configurations.

By utilizing the Bootstrap grid system and its responsive classes (e.g., `col-md-6`), you can easily create flexible and responsive layouts for your web pages. Make sure to include the Bootstrap CSS file in your project for the styles to work correctly.

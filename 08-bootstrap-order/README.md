# Bootstrap Order

## TL;DR

By utilizing Bootstrap's order classes, you can control the visual order of elements on different screen sizes to create responsive and customized layouts.

## A deeper dive

You can use Bootstrap's order classes to rearrange elements in a grid-based layout. In this example, we demonstrate how to use Bootstrap order classes to display a list of UK Premier League soccer teams in a specific order on different screen sizes. We'll start with the default order and then rearrange the teams on larger screens.

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
    <title>Bootstrap Order Classes Example</title>
  </head>
  <body>
    <div class="container">
      <h1>UK Premier League Soccer Teams</h1>

      <div class="row">
        <div class="col-md-4">
          <p>1. Manchester City</p>
        </div>
        <div class="col-md-4">
          <p>2. Manchester United</p>
        </div>
        <div class="col-md-4">
          <p>3. Liverpool</p>
        </div>
      </div>

      <!-- Order on Large Screens -->
      <div class="row">
        <div class="col-md-4 order-md-2">
          <p>4. Chelsea</p>
        </div>
        <div class="col-md-4 order-md-1">
          <p>5. Arsenal</p>
        </div>
        <div class="col-md-4 order-md-3">
          <p>6. Tottenham Hotspur</p>
        </div>
      </div>

      <!-- Order on Extra Large Screens -->
      <div class="row">
        <div class="col-xl-2 order-xl-4">
          <p>7. Leicester City</p>
        </div>
        <div class="col-xl-2 order-xl-5">
          <p>8. Everton</p>
        </div>
        <div class="col-xl-2 order-xl-6">
          <p>9. West Ham United</p>
        </div>
        <div class="col-xl-2 order-xl-7">
          <p>10. Aston Villa</p>
        </div>
      </div>
    </div>
  </body>
</html>
```

In this example:

- We create a Bootstrap grid layout with multiple rows and columns.
- The soccer teams are initially ordered from 1 to 3 (Manchester City, Manchester United, Liverpool) in the first row. This is the default order.
- We then use Bootstrap's `order-md-*` classes to change the order of teams when the screen size reaches the medium (`md`) breakpoint. Chelsea moves to position 4, Arsenal to position 5, and Tottenham Hotspur to position 6.
- For extra-large (`xl`) screens, we use `order-xl-*` classes to rearrange teams further. Leicester City, Everton, West Ham United, and Aston Villa are placed in positions 7 to 10.

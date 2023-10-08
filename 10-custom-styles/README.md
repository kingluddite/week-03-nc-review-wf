# Adding Custom Styles

Here's an example of an NFL standings table created with Bootstrap, and we'll use custom styles to override some of Bootstrap's default styles for the table to give it a unique appearance.

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
    <title>NFL Standings Table with Custom Styles</title>
    <style>
      /* Custom styles to override Bootstrap styles for the table */
      .custom-table {
        background-color: #f5f5f5;
        border-radius: 10px;
      }

      .custom-table thead th {
        background-color: #343a40;
        color: #ffffff;
        border-color: #343a40;
      }

      .custom-table tbody tr:nth-child(odd) {
        background-color: #ffffff;
      }

      .custom-table tbody tr:nth-child(even) {
        background-color: #f8f9fa;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <h1>NFL Standings</h1>
      <table class="table custom-table">
        <thead>
          <tr>
            <th scope="col">Team</th>
            <th scope="col">W</th>
            <th scope="col">L</th>
            <th scope="col">T</th>
            <th scope="col">Pct</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <th scope="row">Kansas City Chiefs</th>
            <td>12</td>
            <td>4</td>
            <td>0</td>
            <td>0.750</td>
          </tr>
          <tr>
            <th scope="row">Buffalo Bills</th>
            <td>11</td>
            <td>5</td>
            <td>0</td>
            <td>0.688</td>
          </tr>
          <tr>
            <th scope="row">Tennessee Titans</th>
            <td>11</td>
            <td>5</td>
            <td>0</td>
            <td>0.688</td>
          </tr>
          <tr>
            <th scope="row">Pittsburgh Steelers</th>
            <td>10</td>
            <td>6</td>
            <td>0</td>
            <td>0.625</td>
          </tr>
          <tr>
            <th scope="row">Baltimore Ravens</th>
            <td>10</td>
            <td>6</td>
            <td>0</td>
            <td>0.625</td>
          </tr>
          <tr>
            <th scope="row">Cleveland Browns</th>
            <td>8</td>
            <td>8</td>
            <td>0</td>
            <td>0.500</td>
          </tr>
          <!-- Add more teams as needed -->
        </tbody>
      </table>
    </div>
  </body>
</html>
```

In this example:

- We create a basic NFL standings table using Bootstrap's `table` class.
- We add custom styles in the `<style>` section to override Bootstrap's default styles for the table:
  - `.custom-table` sets a background color and adds border-radius to give the table a card-like appearance.
  - `.custom-table thead th` changes the background color, text color, and border color for table headers.
  - `.custom-table tbody tr:nth-child(odd)` and `.custom-table tbody tr:nth-child(even)` set alternating background colors for table rows to improve readability.

You can further customize the styles to achieve the look you want for your NFL standings table.

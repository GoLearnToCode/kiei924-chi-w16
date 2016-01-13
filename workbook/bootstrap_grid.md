# Cheat Sheet: The Bootstrap Grid

The [Bootstrap CSS Framework](http://getbootstrap.com/) provides out-of-the-box CSS classifications ("classes") that
can apply to your website.  Using their predefined classes, however, means learning the assumptions and conventions that
your HTML is expected to follow, in order for your page to appear correctly.

In this guide, we will cover the most valuable part of the framework, which is the *grid system* for layout out your page
as a set of rows and columns.

The CSS classes that are best to start with are:

* `container` and `container-fluid`
* `row`
* `col-md-1` up through `col-md-12`

## The Container

If you want to use the Bootstrap grid for your page, you must wrap your page content inside a `div` element that applies
the `container` class or `container-fluid` class.  What's the difference? Just Try It!

Here's an example HTML fragment that illustrates how you would use the container:

``` html
<body>
  <div class="container-fluid">

    <!-- Your rows and columns go here -->

  </div>
</body>
```

## Rows

Inside your container, you **must** divide up your content into horizontal rows.  You must have at least one row.

Here's is a snippet that will use two rows.

``` html
<body>
  <div class="container-fluid">

    <div class="row">

      <!-- Your columns go here -->

    </div>

    <div class="row">

      <!-- Your columns go here -->

    </div>

  </div>
</body>
```

## Columns

Now the hard part.  Inside each row, you must have at least one column. You can have up to twelve columns.  

Here's the key: your must specify the width of each column, and the widths **must add up to 12**.

Here's is a one-row, two-column layout, useful for a page with "main section" with a right-hand "sidebar":

``` html
<body>
  <div class="container-fluid">

    <div class="row">

      <div class="col-md-9">
        <p>This is the main section of the page...</p>
      </div>

      <div class="col-md-3">
        <p>This is the sidebar.</p>
      </div>

    </div>

  </div>
</body>
```

The `-md-` part means that columns will appear on "medium"-size screens, and they will automatically "stack" if the screen is any smaller.

## Responsive Design

The `-md-` family of column widths isn't the only option.  To prevent stacking on smaller devices, use `-sm-` and `-xs-` as needed.  

You can even use multiple designations on a column, which is helpful when you want different column widths depending on the device size, like `<div class="col-md-6 col-xs-3">` which would take up half the screen on a medium device but only one-fourth of the screen on an extra-small device.

# daanmichiels.github.io

Website [http://www.daanmichiels.com/](http://www.daanmichiels.com/).


## Styling

The website uses Bootstrap with [the Flatly theme](https://bootswatch.com/flatly/).

Customizations:
- `$container-large-desktop` is set to `(940px + $grid-gutter-width) !default`
  instead of `(1140px + $grid-gutter-width) !default`

- earlier expansion of the menu

  ```
  // this used to be $screen-sm-min !default
  $grid-float-breakpoint:     $screen-xs-min !default;
  ```

- no color change for a `.brand` element on hover;
  this is for the website title in the top bar (it's not clickable, so it
  shouldn't change color);
  I made this changed _after_ building the CSS, because I got lost in
  the bootswatch code when trying to find the right place to adjust it

  ```
  .navbar-default .navbar-brand:hover, .navbar-default .navbar-brand:focus {
    color: #18BC9C; //this line was removed
    background-color: transparent;
  }
  ```

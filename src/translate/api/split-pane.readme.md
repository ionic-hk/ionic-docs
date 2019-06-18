# ion-split-pane

SplitPane is a component that makes it possible to create multi-view layout.
Similar to iPad apps, SplitPane allows UI elements, like Menus, to be
displayed as the viewport increases.

If the devices screen size is below a certain size, the SplitPane will
collapse and the menu will become hidden again. This is especially useful when
creating an app that will be served over a browser or deployed through the app
store to phones and tablets.


### Setting breakpoints

By default, SplitPane will expand when the screen is larger than 992px.
If you want to customize this, use the `when` input. The `when` input can
accept any valid media query, as it uses `matchMedia()` underneath.


SplitPane also provides some predefined media queries that can be used.

```html
<!-- could be "xs", "sm", "md", "lg", or "xl" -->
<ion-split-pane when="md"></ion-split-pane>
```


 | Size | Value                 | Description                                                           |
 |------|-----------------------|-----------------------------------------------------------------------|
 | `xs` | `(min-width: 0px)`    | Show the split-pane when the min-width is 0px (meaning, always)       |
 | `sm` | `(min-width: 576px)`  | Show the split-pane when the min-width is 576px                       |
 | `md` | `(min-width: 768px)`  | Show the split-pane when the min-width is 768px                       |
 | `lg` | `(min-width: 992px)`  | Show the split-pane when the min-width is 992px (default break point) |
 | `xl` | `(min-width: 1200px)` | Show the split-pane when the min-width is 1200px                      |

 You can also pass in boolean values that will trigger SplitPane when the value
 or expression evaluates to true.


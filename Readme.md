The flex property provides a convenient way for specifying how elements stretch and shrink, while simplifying the CSS required. The flex property allows you to declare flex-grow, flex-shrink, and flex-basis all in one line.

Note: The flex property is different from the flex value used for the display property.

.big {
  flex-grow: 2;
  flex-shrink: 1;
  flex-basis: 150px;
}

.small {
  flex-grow: 1;
  flex-shrink: 2;
  flex-basis: 100px;
}
In the example above, all elements with class big will grow twice as much as elements with class small. Keep in mind, this doesn’t mean big items will be twice as big as small items, they’ll just take up more of the extra space.

The CSS below declares these three properties in one line.

.big {
  flex: 2 1 150px;
}

.small {
  flex: 1 2 100px;
}
In the example above, we use the flex property to declare the values for flex-grow, flex-shrink, and flex-basis (in that order) all in one line.

.big {
 flex: 2 1;
}
In the example above, we use the flex property to declare flex-grow and flex-shrink, but not flex-basis.

.small {
  flex: 1 20px;
}
In the example above, we use the flex property to declare flex-grow and flex-basis. Note that there is no way to set only flex-shrink and flex-basis using 2 values.

The browser to the right has two flex containers, each with three flex items. In style.css, examine the values for each of these items. Notice that the flex-grow and flex-basis values are set for the grey divs. Stretch the browser window to increase its width. Observe that once these divs reach 100 pixels wide, the center div begins to grow faster than the outer divs. Shrink the browser window and notice that something important happens: once the divs reach 100 pixels wide, they begin to shrink equally. This is because flex-shrink defaults to 1, whereas flex-grow defaults to 0.

1.
In #top .side, all three values for flex-grow, flex-shrink, and flex-basis are assigned individually. Refactor them to be declared in one line.
2.
In #top .center, all three values for flex-grow, flex-shrink, and flex-basis are assigned individually. Refactor them to be declared in one line.
3.
In #bottom .side, all three values for flex-grow, flex-shrink, and flex-basis are assigned individually. Refactor them to be declared in one line.
4.
In #bottom .center, all three values for flex-grow, flex-shrink, and flex-basis are assigned individually. Refactor them to be declared in one line.

<!--  -->

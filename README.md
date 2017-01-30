#### Button Styling

Here are some of the disadvantages of my approach. I have also included a few revisions I would like to make to my process in the future:

  - Eyeballing the styling of the button on the template, which led to an inaccurate configuration of gradients and shadowing. For example, I tried to account for the heavier gray component of the gradient on the button half of the button by generating a larger inset box shadow, which did not work effectively.

  - I also attempted to use a CSS produced symbol to generate the arrow on the button. This arrow is not very formattable and while I was able to scale it down using `font-size: smaller`, I was unable to make it more narrow to mimic the template. If I attempted this exercise again, I would try to get a more scaled version of the arrow that would easier to format without needing to change specific dimensions.

  - Finally, from a reusability standpoint, this button is fairly hardcoded and would be hard to use out of the box in other applications. From a styling standpoint, I would pull out a lot of the constant colors, spacings, etc. and place them in a dedicated `_styling_constants.scss` partial file. I would also make this button a React class that would take params and would more easily generate the styled button.

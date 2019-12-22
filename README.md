# Amy McGowan: Portfolio Site
[amymcgowan.dev](https://amymcgowan.dev/)

This portfolio site was built from scratch using HTML, CSS, and Bootstrap.  

The original wireframe was built using Figma.

<img src="./assets/wireframe.png" height="250px" align="center">

## Imitation is the highest form of flattery
I have spotted that my code for this site has been borrowed and adapted by a fellow coder.  I'm flattered. :D
- [https://winerock.github.io/portfolio/](https://winerock.github.io/portfolio/)

## Things I've learned
- Subtle [CSS gradients](https://www.w3schools.com/css/css3_gradients.asp) create a really nice effect.
- Creating CSS variables is really helpful, especially when not 100% set on a color palette.
- Ruby icons don't exist in Font Awesome, but they do exist in [Font Mfizz](http://fizzed.com/oss/font-mfizz)
- How to make a sticky nav bar + [how to account for its space so that each section's header is not hidden behind it](https://www.freecodecamp.org/forum/t/scrollspy-navbar-blocks-content/140274/2)
- Bootstrap [card decks](https://getbootstrap.com/docs/4.0/components/card/) are a helpful way to format blocks of information. Card decks create a set of equal width and height cards that aren't connected to each other. (I used these to display my portfolio projects).
- Bootstrap's [scroll spy](https://getbootstrap.com/docs/4.3/components/scrollspy/) is how I created the effect of using the nav to jump to page sections
- [git stash](https://stackoverflow.com/questions/8085838/how-to-move-the-changes-from-one-branch-to-another-branch-git) is helpful
- A border-radius of 50% can make a circle
- Figuring out exactly how to override default bootstrap can get very frustrating
- [This is a really great article](https://app.getpocket.com/read/1247138368) for finding a color palette, especially for finding which coordinating grays to use (I used Figma for that part). 
- My favorite color sites to use are [colorhexa.com](https://www.colorhexa.com/) and [colorbook.io](https://www.colorbook.io/)
- `class="d-flex justify-content-around"` is perfect for spacing the buttons below each project screenshot AND for equally spacing individual publication pieces (it also centers element on the page when it's only one wide)
- [I can change the column order relative to the breakpoint.](https://bootstrapcreative.com/bootstrap-push-pull-column-ordering-tutorial/)  In my case, I wanted the two columns of project #2 to appear as text on left + img on right on larger break points, but when the columns stacked on mobile, I wanted it to be img on top + text underneath.  I wrote the code in the order I wanted it to appear on mobile.  Then added `order-lg-12` to img and `order-lg-1` to the text.  The `1`, `12` set the order at the `lg` breakpoint and up.
- I kept getting mysterious little lines in between my social links on hover.  Turns out it was the underline text-decoration from the <a> tag.  Just [add a CSS declaration](https://stackoverflow.com/questions/27989672/why-is-link-underline-appearing-after-clicking-the-link) for all anchor states to have no text-decoration. voila!
- When setting a circular background/border behind a FA icon, the [width, height, and alignment need to be set](https://markheath.net/post/font-awesome-circle-background) in order to get an actual circle.
- To get skill icons to stack at smaller breakpoints, I separated them into two columns within a grid and then justified text left/right and adjusted padding to get them line up in a single row at larger breakpoints.
- The projects stack at smaller breakpoints, but they kinda looked like they ran together.  I figured out how to put an hr tag between the projects and then make it stop displaying at larger sizes.
- At medium breakpoint in About section, the img was either huge (stacked) or very small with a lot of white space (inline).  To make it look a bit better, I created a new longer version of the img and set it in a separate identical div.  I then set it so that the original img would appear at all breakpoints except md, when the longer img would appear instead.
- I use the github FA icon in a few places, only one of which I want to have a hover effect.  but .fa-github class with a hover selector was causing the other places to change on hover too.  For those that I wanted to remain static, I created a separate class called .github-static with a property of pointer-events: none; ... all fixed!
- Some blog titles are longer than other, causing the card to be longer too.  I set a min length for the title section (and a min height and max width for the card itself for a little extra precision).


## Image sizes
- Blog preview 260x200
- Project screenshot 500x350


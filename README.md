# Amy McGowan: Portfolio Site
[amymcgowan.dev](https://amymcgowan.dev/)



# Things I've learned
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
- I kept getting mysterious little lines in between my social links on hover.  Turns out it was the underline text-decoration from the <a> tag.  Just [add a CSS declaration](https://stackoverflow.com/questions/27989672/why-is-link-underline-appearing-after-clicking-the-link) for all anchor states to have no text-decoration. voila!
- When setting a circular background/border behind a FA icon, the [width, height, and alignment need to be set](https://markheath.net/post/font-awesome-circle-background) in order to get an actual circle.
- To get skill icons to stack at smaller breakpoints, I separated them into two columns within a grid and then justified text left/right and adjusted padding to get them line up in a single row at larger breakpoints.
- The projects stack at smaller breakpoints, but they kinda looked like they ran together.  I figured out how to put an hr tag between the projects and then make it stop displaying at larger sizes.
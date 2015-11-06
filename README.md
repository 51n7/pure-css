# Pure CSS

This project is an experiment in creating pure CSS components. The entire page is built (responsively) with no dependencies or frameworks in order to see what is possible without relying on large libraries such as jQuery or Bootstrap. [View The Demo →](http://jonbest.ca/pe/)

#### The Reason
I was using Bootstrap for a long time, until I found that with the need for custom UI I was using less and less aspects of it on each project. So I dropped the grid system because it couldn't match my given design, then I dropped the mobile menu for a more flexible jQuery option and so on until I was left only using Bootstrap's 960/1170 container. This led me to believe that I didn't need to always leverage a CSS framework and so now everything is custom, no CSS frameworks.

#### The Technique

The three main techniques used to create these components are:

- Radio Buttons
- CSS Pseudo Checked
- Magic

All I'm doing is checking/unchecking a hidden radio button using a ```<label/>``` and with some CSS saying the radio:checked + sibling do something. Basically the label simulates a click event by natively controlling a radio/checkbox, which is something that's been possible in HTML since the beginning. I know this is not the correct usage for labels and radios but it still works great for these purposes.

#### The Components

These components will all work from IE9 and up, since the :checked pseudo is still under the CSS3 spec:

- Mobile Menu (still only one nav in the HTML, reused)
- Accordion Menu
- Modals
- Dropdown
- Checkbox Dropdown
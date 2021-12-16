# Learning Bootstrap4 and Bootstrap5
This repository is intended to store Bootstrap samples and a small project.

# The Project
We want to create a landing page for a conference happening in Hawaii, it should describe what the conference is about, where, who are the speakers and have a form to register as a speaker or buy tickets (in a modal).

This project was originally created in Bootstrap v4.6 and then migrated to Bootrap v5.1.3

You can see the project in this link:

https://jonathlan.github.io/bootstrap4-essentials/project/

# Samples
## Samples folder
You will find a few samples for the different capabilities of Bootstrap, specially on the grid system.

- [basic.html](https://jonathlan.github.io/bootstrap4-essentials/samples/basic.html) - It's just the hello world using Bootstrap and shows how to add the framework to the page.

### Grid folder
This contains a set of samples for the grid manipulation.
1. [basics.html](https://jonathlan.github.io/bootstrap4-essentials/samples/grid/basics.html) - Basic sample where you can see how the grid works in a very general way.
2. [grid-basic-2.html](https://jonathlan.github.io/bootstrap4-essentials/samples/grid/grid-basic-2.html) - A more organized sample where you can see different alignemnts for rows and columns.
3. [grid-responsive-html](https://jonathlan.github.io/bootstrap4-essentials/samples/grid/grid-responsive.html) - This file shows how to change columns' width based on device's sizes.
4. [offsetting.html](https://jonathlan.github.io/bootstrap4-essentials/samples/grid/offsetting.html) - In Bootstrap, it is possible to offset the columns' position based on device's sizes, this file shows how to do that.

# Migration from Bootstrap v4 to v5

It's highly recomended to take a look at the Bootstrap migration document located in:

https://getbootstrap.com/docs/5.1/migration/

For this project, below changes were required:

- Rename .ml-* and .mr-* to .ms-* and .me-*.
- Rename 'data-' attributes to all JS plugins to 'data-bs-'
- Rename .pl-* and .pr-* to .ps-* and .pe-*.
- Rename .text-left and .text-right to .text-start and .text-end.
- Rename 'badge-*' to 'bg-*'
- Drop form-specific layout classes for the  grid system. Use grid and utilities instead of .form-group, .form-row, or .form-inline.
- Update the way Tooltips are enabled via JavaScript.
- Wrap 'Enviar' button in a div with class 'd-grid' because bootstrap5 has dropped .btn-block class.
- Add the 'text-dark' class to the warninig badge because in Bootstrap5 text has changed to white.
- Rename .close to .btn-close for a less generic name. And remove span in the modal, which is not required anymore.
- Add some padding to the badges, Bootrap5 seems to have a slightly smaller one.
- Add padding to the textarea column in the form, because Bootstrap5 dropped form-row class.
- Add 'text-decoration-none' class to footer links, because in  Bootstrap5 links are underlined by default.
# Custom R Theme to Resemble VS Code

I like the look of VS code, so with the help of [Riley Roach's](https://github.com/riley-roach/RStudio-Customizations) and [Tobias Krabel's](https://github.com/tkrabel/rstudio_atom_theme) GitHub pages I created a custom theme. A few notes:

## Installing the Theme

This theme was built to replace "Solarized Dark." To change you theme, replace the css code in `48C0BA77165E379D163EF2BB78F78916.cache.css` with the css code in AsherThemeR.css, by pasting in the new code over the old code. I'd recommend making a backup copy of the code before you do this!

By default, R Studio will make function call text the same color as variable names. To change this, go to "Preference" -> "Code" -> "Display" and check "Highlight R function calls." RStudio will subsequently reference the `.ace_entity.ace_name.ace_function` and `.ace_support.ace_class` parts of the CSS document, which allows you to change the color of calls to functions and packages.

[This page](https://rstudio.github.io/rstudio-extensions/rstudio-theme-creation.html) is very helpful for outlining the different components of the CSS code that makes up an RStudio theme.
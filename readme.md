# Custom R Theme to Resemble VS Code

I like the look of Visual Studio, so with the help of [Riley Roach's](https://github.com/riley-roach/RStudio-Customizations) and [Tobias Krabel's](https://github.com/tkrabel/rstudio_atom_theme) GitHub pages I created a custom theme to make RStudio look similar. It looks like this:

![NewLook](images/RStudioAsherAppearance.png)

## Installing the Theme

This theme was built to replace "Solarized Dark." For Mac Users, locate your RStudio application and right click on the icon. Select "Show Package Contents" and then natigate to the folder `~/RStudio.app/Contents/Resources/www/rstudio`. In that folder, open the .css file `48C0BA77165E379D163EF2BB78F78916.cache.css`. You'll replace the code in this file with the code in AsherThemeR.css by pasting in the new code over the old code. I'd recommend making a backup copy of the code before you do this!

By default, R Studio will make the text for function calls the same color as variable the text for variable names. To change this, go to "Preferences" -> "Code" -> "Display" and check "Highlight R function calls." RStudio will subsequently reference the `.ace_entity.ace_name.ace_function` and `.ace_support.ace_class` parts of the CSS document, which allows you to change the color of calls to functions and packages.

[This page](https://rstudio.github.io/rstudio-extensions/rstudio-theme-creation.html) is very helpful for outlining the different components of the CSS code that makes up an RStudio theme.

## Changing RStudio so Surrounding Regions are Black

The updates, described above, change only the layout of the panes (e.g. the console, source, etc.). If you want to change the colors that surround the panes to further resemble VS code (which has a darker black color), you can add a new .css file to your `~/RStudio.app/Contents/Resources/www/` folder and make an update to the `index.htm` document to reference the new .css file. [Riley Roach](https://github.com/riley-roach/RStudio-Customizations) provides the necessary code to do so (along with instructions).
# WPF.Themes
Themes for WPF

There are all kinds of resources on the internet for theming WPF. Some really good ones too...
https://github.com/MahApps/MahApps.Metro/tree/develop/src/MahApps.Metro/Styles
https://github.com/MaterialDesignInXAML/MaterialDesignInXamlToolkit/tree/master/MaterialDesignThemes.Wpf/Themes
https://github.com/fluentribbon/Fluent.Ribbon
https://github.com/ControlzEx/ControlzEx

There is even a cool ThemeManager as a part of one of the GitHub packages. I think this looks pretty cool. 
https://github.com/ControlzEx/ControlzEx/blob/develop/Wiki/ThemeManager.md

###Theming Made Easy
Even with those resources I didn't want nuget packages or a collection of resource dictionaries. I wanted one. So I set out to make one. Got to generating templates via Blend. Found Show Me The Templates! (https://sellsbrothers.com/2091) and grabbed a few from there. I also referenced what the MahApp folks did quite a bit.

Finding Show Me The Templates! lead me to making an improved version of the tool which can be found here (https://github.com/AaronAmberman/WPF.DefaultControlTemplateViewer). It has the power to generate the entire resource dictionary from the Microsoft themes like Luna or Royale. This is cool because you can see what MS did to develop their Aero, Luna, Luna Homestead, Luna Metallic, Classic or Royale themes. Always helpful to see what the developers of the language do. Check it out!

I made a large ***highly organized and readable*** resource dictionary containing all my resources. This way I don't need to clone a whole GitHub repo (or you if you use this). Just go to the GitHub page for the file and click the *"Copy raw contents"* button...
![CopyContentsOnGitHub](https://user-images.githubusercontent.com/23512394/153728498-1586d61a-5c7d-4ccb-9c53-cab629302c48.png)

This ***will style the built in WPF controls*** but it does not colorize all controls.

Unaffected types...
 - All panels
 - Border
 - Grid
 - Recangle
 - TextBlock (yup, you'll have to set a "defult" style for dark themes where you wish to have white text, I do not do this for reasons)
 - UserControl
 - Window
 
I am sure there may be a few more but you get the idea.

**Each theme's templates are not the same**. The LightTheme was mostly auto generated templates that were not modified much. The LightTheme is 99% the same as the default look and feel. Some colors are slightly different.  DarkTheme (and others in the future) will not have the same template structures as some of the auto generated templates act strangely and can be hard to modify. Making overridden styles for Borders and TextBlocks affects many other control templates so be careful when apply global styling to these types.

File organization...
![Example1](https://user-images.githubusercontent.com/23512394/153728514-e8503a63-710c-4d7a-918c-edd0a01decf0.png)
![Example2](https://user-images.githubusercontent.com/23512394/153728788-4c71a2af-a860-4ccc-b2e1-63ebdfda5811.png)


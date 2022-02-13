# WPF.Themes
Themes for WPF

There are all kinds of resources on the internet for theming WPF. Some really good ones too...
https://github.com/MahApps/MahApps.Metro/tree/develop/src/MahApps.Metro/Styles
https://github.com/MaterialDesignInXAML/MaterialDesignInXamlToolkit/tree/master/MaterialDesignThemes.Wpf/Themes
https://github.com/fluentribbon/Fluent.Ribbon
https://github.com/ControlzEx/ControlzEx

There is even a cool ThemeManager as a part of one of the GitHub packages. I think this looks pretty cool. 
https://github.com/ControlzEx/ControlzEx/blob/develop/Wiki/ThemeManager.md

All that being said, I didn't want to have to pull in Nuget packages or have 27 different XAML resource dictionaries holding all my templates. I just wanted **one** file even if it was going to be big because I like one stop shopping. As long as the ***file was highly organized and easy to read***. So I got to generating templates through Blend. Got most of what I have from Blend. I found a tool online called Show Me The Templates! (https://sellsbrothers.com/2091) and used that to grab templates I didn't have from Blend that it had.

Which lead me to making an improved version of the tool which can be found here (https://github.com/AaronAmberman/WPF.DefaultControlTemplateViewer). It has the power to generate the entire resource dictionary from the Microsoft themes like Luna or Royale. This is cool because you can see what MS did to develop their Aero, Luna, Luna Homestead, Luna Metallic, Classic or Royale themes. Always helpful to see what the developers of the language do. Check it out!

As aforementioned the file is very highly organized and changing colors should be easy (as long as you don't want to change the template). Just modify all the colors at the top of the file. Their name is a good indication of what they are used for. So if you see colors Button.Background, Button.Border and Button.Foreground then you can probably very easily figure out what those apply to. Anyway, tried to make theming easy by making it one stop shopping and highly organized. You don't even need to clone the repo. Just go to the GitHub page for the file and click the *"Copy raw contents"* button...

![CopyContentsOnGitHub](https://user-images.githubusercontent.com/23512394/153728498-1586d61a-5c7d-4ccb-9c53-cab629302c48.png)

Just to be clear, the resource dictionary ***will style the built in WPF controls*** but it does not colorize all controls. The Grid, Border, Recangle, UserControl, etc. all still have native transparent backgrounds. The Window Background property was not set either so in darker themes you may still see some white. Its up to you to close these gaps as you see fit.

File organization...
![Example1](https://user-images.githubusercontent.com/23512394/153728514-e8503a63-710c-4d7a-918c-edd0a01decf0.png)
![Example2](https://user-images.githubusercontent.com/23512394/153728788-4c71a2af-a860-4ccc-b2e1-63ebdfda5811.png)

The LightTheme is 99% the same as the default look and feel. Some colors are slightly different. 
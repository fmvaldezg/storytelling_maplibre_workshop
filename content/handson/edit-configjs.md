---
layout: default
title: Edit Your config.js file
parent: Hands On
nav_order: 2
---
# Edit Your config.js
First we're going to make a few quick edits to your new repository's config.js file. This file contains the story main content and the map controls.

### *1*{: .circle .circle-blue} Open your repository files in `Visual Studio Code`.

While on `GitHub Desktop`, click on the option to `Open in Visual Studio Code`


![Open on Visual Studio Code](../img/config0.png)  

This will open `Visual Studio Code`.

### *2*{: .circle .circle-blue} Rename the file.  

You are going to see a list with all the files and folders on your repository. 

![Open on Visual Studio Code](../img/config1.png)  

Right click on the file `config.js.template` and select the `Rename` option.

![Open on Visual Studio Code](../img/config2.png)  

Change the name of the file to `config.js`, without the word template at the end.

### *3*{: .circle .circle-blue} Make some edits to your `config.js` file.  

Click on the file you just renamed. Its content will be displayed in the central panel on GitHub Desktop.

The first 17 lines of this file contain the main configurations for your new sotrymap. 

![Edit your README](../img/config3.png)

Step 1
{: .label .label-step}

Give your map a title by replacing the text after `title:`

Input
{: .label .label-green }
```
title: 'My first StoryMap'
```

Be aware that al these properties are build by a pair of values. Values other than boolean (true,flase) should be between ``. 
{: .warn}
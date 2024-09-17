---
layout: default
title: Add chapter data
parent: Hands On
nav_order: 4
---
# Add chapters

Now that you have the basic configuration of your storymap, it is time to add data to your chapters.
Chapters contain the contents of your story. Each of them is a box with text and mutimedia that will scroll on top of your basemap.

You will need to add and set some details in the `config.js` file to create the chapters of your story.
Starting on line 18 of the `config.js` file, you will see the chapters and its properties.

At the bottom of this page you have a detail on the function of each property of the chapters in the `config.js` file.
We will go through the basic properties in the following steps.

### *1*{: .circle .circle-blue} Setting up your first chapter.

Step 1
{: .label .label-step}

Add an `id` to your fist chapter. Just type any text that will identify your firts chapter.

Input
{: .label .label-green }
```
20  id: 'my-first-chapter'
```
Remember to use dashes to separate words and lowercase letters for the chpater id. 
{: .warn}

![screenshot of the chapter id](../img/chapters1.png)

Step 2
{: .label .label-step}






| Property | Function
| --- | ---
| `id:` | A slug-style ID for the chapter. This is read by the JavaScript driving the app and is assigned as an HTML `id` for the `div` element containing the rest of the story. A best-practice format would be to use kebab case, like `my-story-chapter-1`.
| `alignment:` | This defines where the story text should appear over the map. Options are `center`, `left`, `right`, and `full`.
| `hidden:` | Sets the visibility of the chapter to hidden when `true`. The chapter will still trigger a map and layer transition.
| `title:` | The title of the section, displayed in an `h3` element.
| `image:` | The path to an image to display in this section.
| `caption:` | Adds a caption for the image.
| `author:` | Adds an author to display at the bottom of the chapter.
| `website:` | Adds a website to display at the bottom of the chapter.
| `legend:` | Adds a HTML legend box for this chapter. `legend` must be enabled in the config settings above as well.
| `description:` | The main story content for the section. This should be aligned with what the reader is seeing on the map. In the vanilla version, this field will render as HTML. Images, links, and other items can be included as HTML.
| `location:` | Details about the map display and camera view. `center`: Center coordinates of the map, as longitude, latitude. `zoom`: Zoom level of the map. `pitch`: Angle of the map view. 0 is straight down, and 60 is highly tilted. `bearing`: Degrees of rotation clockwise from North (0). Negative values represent counter-clockwise rotation.
| `mapAnimation:` | Defines the animation type for transitioning between locations. This property supports `flyTo`, `easeTo`, and `jumpTo` animations. If not specified, defaults to `flyTo`.
| `rotateAnimation:` | Starts a slow rotation animation at the end of the map transition when set to `true`. The map will rotate 90 degrees over 24 seconds.
| `mapInteractive:` | When set to `true`, sets this chapter to be interactive, allowing the user to pan and zoom across the map, and adds navigation controls.
| `callback:` | Accepts the name of a JavaScript function and executes the function. Use this if you have custom code you want to run for a chapter, like turning a legend on or off, adding data from an API request, or displaying an interactive graph.
| `onChapterEnter:` | Layers to be displayed/hidden/muted when the section becomes active. `layer`: Layer name as assigned in MapLibre style. `opacity`: The opacity to display the layer. `0` is fully transparent, `1` is fully opaque. `duration`: The length of the opacity transition, numeric, in milliseconds. Default is 300. This is an optional parameter and can be omitted.
| `onChapterExit:` | Same as `onChapterEnter` except it is triggered when the section becomes inactive.
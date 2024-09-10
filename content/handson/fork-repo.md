---
layout: default
title: Fork The Storytelling Template
parent: Hands On
nav_order: 1
---
# Fork the storytelling template
In this workshop we're going to duplicate the storytelling template created by [Digital Democracy](https://www.digital-democracy.org/) to your own GitHub account, then make some edits together. Can tinker and reuse this template anytime on your own account.

### *1*{: .circle .circle-blue} Go to [Digital Democracy Interactive Storytelling with Maplibre repository](https://github.com/digidem/maplibre-storymap){:target="_blank"}


### *2*{: .circle .circle-blue} Click on the option to Fork the repository
You'll see an option to Fork at the top right of your screen.   

![Fork location](./content/img/fork-location.png)

GitHub should pause for a moment while it copies the files from this repo to yours. When it's finished, you'll see a note that the repo has been "forked from [digidem/maplibre-storymap](https://github.com/digidem/maplibre-storymap)" in the top left.

```  
Alternatively, if you are using GitHub Desktop, simply copy the repository URL https://github.com/digidem/maplibre-storymap.git and paste it in the 'Clone a repository' window in the app, or download the ZIP file of the repository and add it to your GitHub Desktop app.
{: .note}
```

You should also see your new repository which contains the following files and directories:
```
.
├── demo
├── dist
├── images
├── map
├── .gitignore
├── LICENSE
├── README.md
├── build.js
├── config.js.example
├── index.html
├── index.js
├── package-lock.json
├── package.json
└── sources.js
```
In this workshop we're only going to be looking at a couple of these including the `config.js` file, the `index.html` file, and the files inside the `images` and `map` folders.
{: .note}

### *3*{: .circle .circle-blue} Edit your config.js
We will need to publish this repository as a "GitHub Page", so that it's live at **[your GitHub username].github.io**. Right now it's configured to appear at **ubc-lib-geo.github.io**. Before we publish, we'll need to make some edits to our main site configuration file, '_config.yml'.

Step 1
{: .label .label-step}
Click on the `_config.yml` file in your list of files
{: .step}

Step 2
{: .label .label-step}
Select the **edit file** tool on the top left
{: .step}
![Edit file](../img/edit-file.png)

Step 3
{: .label .label-step}
Scroll down to line 28 and add your base hostname
{: .step}
You will want to make sure `https://ubc-lib-geo.github.io` is changed to `https://[YOUR GITHUB USERNAME].github.io`

Step 4
{: .label .label-step}
Next, go to line 40 and update the footer.
{: .step}
In line 40, you'll want to replace `ubc-lib-geo` with your own username. The result should look like this:  
`footer_content: <a href="https://github.com/your_username/gis-workshop-waml-template" target="_blank">View this workshop in GitHub</a>`  

Step 5
{: .label .label-step}
Add a commit message and save
{: .step}
Add something brief to your commit message – you can literally recycle the provided "Updated _config.yml" language – then press **Commit changes**.  

### *4*{: .circle .circle-blue} Go to your repository's Settings menu
We're almost ready to publish our workshop site! We can do that in our site's **Settings** which is found by clicking the top right tab.
![Edit file](../img/settings.png)

### *5*{: .circle .circle-blue} Publish your workshop site
Scroll down to the settings for GitHub Pages (almost to the bottom (Danger Zone!)). Under **Source** select your only branch (either `main` or `master`).  

Your site will take a moment (up to a couple of minutes) to build and propagate, but should soon be available at `https://[YOUR GITHUB USERNAME].github.io/gis-workshop-waml-template/`

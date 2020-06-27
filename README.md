# figma-plugins-vue-ts-boilerplate
A very simple vue.js/typescript boilerplate for creating figma plugins. Does include:
- figma.d.ts typings dependency
- Sass (.scss)
- Webpack
- Vue Views
- Inter font loaded in UI
- a11y (accessibility) global helper class, that detects if the user is using keyboard and turns :focus outlines on, or off if he is using the mouse.

# Installation
### Step 1 
Just clone this repo and cd into it.
```
git clone https://github.com/madebyfabian/figma-plugins-vue-ts-boilerplate.git
cd figma-plugins-vue-ts-boilerplate
```

Now you are in the project root. You can open it in VSCode for example, with `code .`, or with any other Editor.

### Step 2
Open the command line and hit
```
npm install
```

This will install any dependencies which are needed.

**Now you're good to go :)**

# Usage
There are two ways of getting the plugin to run. 

### Development
Just type
```
npm start
```
to execute the webpack watcher (Re-builds everytime you save).

### Production
If you only want to build it once for production, just type
```
npm run build
```
This is useful to see how your plugin reacts in the "real world". Also, when you submit your plugin to the Figma community, you should submit the files generated with this build-command.

### Usage in Figma
After you ran one of those two commands, you'll notice that new `build` folder in the root of the project folder. 

Now you can import it in Figma, just:
1. Open Figma
2. Go to the Plugins overview
3. Click on "+" next to "Create your own plugin"
4. On the popup, click `Click to choose a manifest.json file`
5. Now select the file `build/manifest.json`.

# Support / Questions / Feature requests
Just hit me up via [Twitter (@madebyfabian)](https://twitter.com/madebyfabian) or create an issue / PR.
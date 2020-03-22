# figma-plugins-vue-ts-boilerplate
A very simple vue.js/typescript boilerplate for creating figma plugins. Does include:
- TypeScript Support for vue
- figma.d.ts typings file
- Sass (.scss)
- Webpack
- Vue Views
- Inter font loaded in UI
- a11y (accessibility) global helper class, that detects if the user is using keyboard and turns :focus outlines on, or off if he is using the mouse.

# Installation
### Step 1 
First you have to create a new plugin folder with the Figma Desktop app, just to generate your unique plugin ID.

1. Open Figma 
2. Go to the Plugins overview
3. Click on "+" next to "Create new plugin"
4. Type in something like `my-temp-plugin-folder` hit "Continue ->"
5. Select "With UI & browser APIs" and hit "Save as...". Save it somewhere on your PC.

Then go to the new folder you saved, and open the `my-temp-plugin-folder/manifest.json` file. In this, you'll see a id. Copy it to cour clipboard.

### Step 2

Just clone this repo with 
```
git clone https://github.com/madebyfabian/figma-plugins-vue-ts-boilerplate.git
```

then just
```
cd figma-plugins-vue-ts-boilerplate
```

Open this folder with your favourite IDE. Paste in the copied plugin ID from Step 1 into the `id` field of the `figma-plugins-vue-ts-boilerplate/manifest.json` file.

Be sure to do 
```
npm install
```

You now can delete your self-generated plugin-folder `my-temp-plugin-folder` from step 1.

**Now you're good to go!**

# Usage
Webpack will create a folder called `dist`, in which all plugin-related files are. Figma only needs files from this folder.

### Development
Just type
```
npm start
```
to execute the webpack watcher. 

### Production
If you only want to build it once for production, just type
```
npm run build
```

### Usage in Figma
After you ran either `npm start` or `npm run build`, you'll notice that new `dist` folder in the root of `figma-plugins-vue-ts-boilerplate`. 

Now you can import it in Figma, just:
1. Open Figma
2. Go to the Plugins overview
3. Click on "+" next to "Create new plugin"
4. On the popup, click `Click to choose a manifest.json file`
5. Now select the `figma-plugins-vue-ts-boilerplate/dist/manifest.json` file.

# Support / Questions / Feature requests
Just hit me up via [Twitter (@madebyfabian)](https://twitter.com/madebyfabian) or create an issue / PR.
# SaaS - Fixed Watch Loop

## The below text comes from a message from Adrian Gould regarding the `npm run watch` loop that was occuring

- Do the following:

 1. Rename the public folder to assets
 2. Create a new public folder at the root of the project (easiest way is to right mouse click on the project name, new -> directory)
 3. Move the html and php files from the assets folder to the new public folder
 4. Edit the `webpack.mix.js` file, replace public with assets - see below
  
  ``` javascript
  mix.setPublicPath('assets')
  mix.setResourceRoot('../')

  mix.js('src/js/app.js', 'assets/js')
      .sass('src/sass/app.scss', 'assets/css')
      .postCss('src/css/app.css', 'assets/css',
        [
            require('postcss-import'),
            require('tailwindcss'),
            require('autoprefixer'),
        ]
    )

    if (mix.inProduction()) {
        mix.version();
    }
  ```

 5. Save the changes
 6. In the Commander (CMDER Terminal) run: `npm run watch`
 7. Edit the `tailwind.config.js` file replacing the `purge` section with the below:

``` javascript
const defaultTheme = require('tailwindcss/defaultTheme')
const colors = require('tailwindcss/colors')

module.exports = {
  content: [
    './public/**/*.{php,html}',
    './src/**/*.{js,vue}',
  ],

  theme: [     
    etc...
```

- This should now watch for changes in the HTML and PHP and update the CSS files correctly.

## To make sure you can see changes update your files when the PHP, HTML, JS or CSS changes do the following

1. Open the settings (CTRL+ALT+S) and open the Plugins section.
2. Click on Marketplace and search for "Live Edit"
3. Install the plugin.
4. Search for the "Live Edit" settings (Build, Execution, Deployment -> Debugger -> Live Edit) and tick the Track Changes in HTML, CS and JS option.
5. Also tick the update in chrome to include HTML, CSS and JS.
6. OK the changes.

- (from:<https://www.jetbrains.com/help/phpstorm/live-editing.html#ws_live_edit_activate_procedure>)

**You may still not get immediate updates when it has to compile in a new item that has not been used before.**

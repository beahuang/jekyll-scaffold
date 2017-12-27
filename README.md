# Example Jekyll Scaffold

## Setup

#### Prerequisites
1. Mac Command Line Tools `xcode-select --install`
2. [nvm](https://github.com/creationix/nvm) `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash`

#### Setting up the project
1. Get the right node version `nvm use`
2. Install [Jekyll](http://jekyllrb.com/) `gem install jekyll`
3. Install [Gulp](http://gulpjs.com/) `npm install -g gulp`
4. Clone the repo
5. Install all dev dependencies `npm install`
6. Build all of the assets `gulp build`
7. Open a locally hosted copy of the files in your browser `gulp serve`

## Development
- Use `gulp` to build your files and watch your source files to have them be built automatically
- Files are being served from the `_site` folder

##### Jekyll Docs: https://jekyllrb.com/docs/structure/

## Code Structure

* `_data` - yaml files containing data
* `_includes` - HTML partials for each section
* `_layouts` - holds page layouts
  * base.html - main skeleton for site
* `_scripts` - JavaScript for the site
  * `modules` - module JavaScript files
  * `vendor` - vendor JavaScript files
  * `main.js` - entry point for the JavaScript modules
* `_scss` - styles
  * `partials` - scss partials for each section
  * main.scss - general styles, each partial gets imported in this file
* `_site` - built static site
* `fonts` - font files
* `gulp`- gulp task files which are injected into the gulpfile
* `img` - images
* `.editorconfig` - sets coding styles for IDEs
* `.nvmrc` - indicates node version
* `_config.yml` - general info for the site
* `.gitignore` - specifies git ignores
* `gulpfile.js` - entry point for build scripts
* `index.html` - where HTML partials are imported (from `_includes`)
* `package.json` - specifies npm dependencies

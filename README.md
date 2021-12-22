## Resume Source

The source for my resume static site. Instructions below:

##### To dev
```
$ grunt // generates the js files and serves the project
```

##### To deploy
```
$ grunt build // builds the static site in the "build" directory
```

Visit [http://localhost:8888](http://localhost:8888) to see changes.

##### Testing JSON changes
Test changes by updating `resume.json` file inside `node_modules/resume-schema/` folder. Rerun `grunt` optional: `exec:run_server` after any changes to `resume.json`

##### Updating styles
All the LESS files are organized under the folder `assets/less/`. Check the comments inside `theme.less` to find out which file to make LESS changes. Grunt compiles `assets/less/theme.less` to `assets/css/theme.css` which is used eventually in the theme. 

##### Updating Javascript
All the javascript changes go into `index.js` which is responsible for rendering the resume.

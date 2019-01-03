# Angular-Ionic-Apps

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.1.4.

## Steps to create this project
### Angular app
1. Global installation of the Angular CLI: 

    `$ npm install @angular/cli@7.1.4 --global` or `$ npm i @angular/cli@7.1.4 -g`

2. Create a new angular workspace with no default application:

    `$ ng new angular-ionic-apps --createApplication=false`

    More information: 
    - [Angular Workspace: No Application for You!](https://blog.angularindepth.com/angular-workspace-no-application-for-you-4b451afcc2ba)

3. Open the project folder: 

    `$ cd .\angular-ionic-apps\`

4. Create a new angular application inside of the workspace: 

    `$ ng generate application web-app --style=scss`

    More information:
    - [Angular - Mulitple projects](https://github.com/angular/angular-cli/wiki/stories-multiple-projects)
    - [Angular CLI SASS options](https://stackoverflow.com/questions/36220256/angular-cli-sass-options)

5. Start the angular project:

    `$ ng serve --project=web-app`

### Ionic app
1. Global installation of the Ionic CLI: 

    `$ npm install ionic@4.6.0 --global` or `$ npm i ionic@4.6.0 -g`

2. Create the file `ionic.config.json` in the default workspace folder.

    More information:
    - [Ionic 4 - Multi-app projects](https://beta.ionicframework.com/docs/cli/configuration#multi-app-projects)

3. Create a new ionic applicaion inside of the workspace:

    `$ ionic start mobile-app --no-deps`

4. Move the new created folder `/mobile-app/` into the `/projects/` folder.

5. Rename the project `mobile-app` to `app` in the file `ionic.config.json`.

6. Also change the path of the `app` project to `"root": "projects/mobile-app"` in the file `ionic.config.json`.

7. Go the `mobile-app` folder with the command `$ cd .\projects\mobile-app\`.

8. Then install all dependencies of the `mobile-app` project:
    
    `$ npm install` or `$ npm i`

9. Go back to the workspace folder `/angular-ionic-apps/`:

    `$ cd ../..`

10. Then start the ionic projec:

    `$ ionic serve --project=app`

---
## More helpful links
- [Nx Workspace demo to share ngrx-based logic (state, action and reducers) between Ionic4 and Angular7 apps ](https://github.com/benorama/ngrx-demo-workspace)
- [Angular - Library support](https://github.com/angular/angular-cli/wiki/stories-create-library)

---
## Development server

### Angular app

Run `$ ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files. 
For a special project run `$ ng serve --project=web-app`.

### Ionic app

Run `$ ionic serve` for a dev server. Navigate to `http://localhost:8100/`. The app will automatically reload if you change any of the source files. 
For a special project run `$ ionic serve --project=app`.

## Code scaffolding

### Angular app
Run `$ ng generate component component-name` to generate a new component. You can also use `$ ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

### Angular app
Run `$ ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

### Angular app
Run `$ ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

### Angular app
Run `$ ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

### Angular app
To get more help on the Angular CLI use `$ ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

### Ionic app
To get more help on the Ionic CLI use `$ ionic help` or go check out the [Ionic CLI README](https://github.com/ionic-team/ionic-cli/blob/master/README.md).
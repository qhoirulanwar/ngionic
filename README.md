# Menambahkan component ionic 4 pada angular 8

**1. install @ionic/angular**

	$ npm i @ionic/angular

**2. Tambahkan IonicModule pada app.module.ts**

    import { IonicModule } from '@ionic/angular';

    imports: [
	    BrowserModule,
	    IonicModule.forRoot()
	  ]
**3. Tambahkan assets build ionicons pada angular.json**

    "assets": [
              "src/favicon.ico",
              "src/assets",
              {
                "glob": "**/*.svg",
                "input": "node_modules/ionicons/dist/ionicons/svg",
                "output": "./svg"
              }
            ],
**4. Tambahkan style build css ionic pada angular.json**

    "styles": [
              "src/styles.scss",
              "./node_modules/@ionic/angular/css/core.css",
              "./node_modules/@ionic/angular/css/normalize.css",
              "./node_modules/@ionic/angular/css/structure.css",
              "./node_modules/@ionic/angular/css/typography.css",
              "./node_modules/@ionic/angular/css/display.css",
              "./node_modules/@ionic/angular/css/padding.css",
              "./node_modules/@ionic/angular/css/float-elements.css",
              "./node_modules/@ionic/angular/css/text-alignment.css",
              "./node_modules/@ionic/angular/css/text-transformation.css",
              "./node_modules/@ionic/angular/css/flex-utils.css"
            ],

**5. silahkan uji coba component ionic pada file component.html**
saya mencoba pada app.component.html

    <ion-button>Tombol</ion-button>

#

# Ngionic

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.10.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

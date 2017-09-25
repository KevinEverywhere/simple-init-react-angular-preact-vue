# simple-init-react-angular-preact-vue

This project is an example of current framework cli-build processes. Once the initial files are created, you can experiment in each of the apps in their own child directory.

## instructions

Each framework has its own installation and launch scripts. It is recommended that you use yarn for package management and running scripts.

```
git clone git@github.com:KevinEverywhere/simple-init-react-angular-preact-vue.git
cd simple-init-react-angular-preact-vue
npm install
```

### Run All Four

Running the startAll script will execute startReact, startPreact, startAngular, and startVue. Please look to the individual script to see cli specifics.

Ensure that you have previously installed yarn and then run this line of code.
```
yarn run startAll
```
The most typical errors when they occur come from ports 3000, 8080, 6789 and 4200 already being used; and yarn not being installed. If you do not have yarn installed, run the following line of code.

```
npm install -g yarn
```

### react

Running the startReact script will first test to see if it has ever been run before (testReact). After the directory has been recognized or created, the startReact script runs yarn start in the my-react-app directory. When you run yarn start, it will install or check for updates in the repo's dependencies. From the root directory (simple-init-react-angular-preact-vue), run the following script and the application will launch in the browser at http://localhost:3000.

```
yarn run startReact
```

### angular

Running the startAngular script will first test to see if it has ever been run before (testAngular). After the directory has been recognized or created, the startAngular runs ng serve
in the my-angular-app directory. When you run ng serve, it will launch the app in port 4200. From the root directory (simple-init-react-preact), run the following script and it will launch at http://localhost:4200.

```
yarn run startAngular
```

### preact

Running the startPreact script will first test to see if it has ever been run before (testPreact). After the directory has been recognized or created, the startPreact runs preact watch -p 6789
in the my-preact-app directory. When you run yarn start, it will install or check for updates in the repo's dependencies. From the root directory (simple-init-react-preact), run the following script and once it creates the application, you can find it at http://localhost:6789.

```
yarn run startPreact
```

### vue

Unlike the other CLI tools, the vue-cli will require some interactivity during the creation process. You can easily just hit return and accept the defaults at the command line which will create a new vue app titled my-vue-app. Once the startVue script calls testVue to see if it has ever been run and creates the app and directory if it has not, it then runs yarn start from the my-vue-app directory. When you run yarn start, it installs and checks for updates in the repo's dependencies. From the root directory (simple-init-react-angular-preact-vue), run the following script and the application will launch in the browser at http://localhost:8080.

```
yarn run startVue
```

## summary

This truly is meant as nothing more than a way to quickly see the state of current CLI framework development in September 2017. This should save some time for those wanting to have a quick view of how they compare and look under the hood.

## reference

This repo uses the initialization scripts described in the [preact-cli][preact-cli], for preact, [create-react-app][create-react-app] for react, [angular-cli][angular-cli], for angular, and [vue-cli][vue-cli] for vue to create base applications. For more information, please use the links below to discover best practices and state of the moment examples and documentation.

[react][whatsnew]

[angular][angular]

[preact][preact]

[vue][vue]

-------------

[whatsnew]: https://facebook.github.io/react/blog/2017/05/18/whats-new-in-create-react-app.html
[create-react-app]: https://github.com/facebookincubator/create-react-app

[angular]: https://github.com/angular/angular
[angular-cli]: https://github.com/angular/angular-cli

[preact]: https://preactjs.com/
[preact-cli]: https://github.com/developit/preact-cli

[vue]: https://vuejs.org/v2/guide/
[vue-cli]: https://github.com/vuejs/vue-cli

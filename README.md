# Aurelia-Node

This is a NodeJS Express App bundled with the [Skeleton App](https://github.com/aurelia/skeleton-navigation) of the [Aurelia](http://www.aurelia.io/) platform. It sets up a standard navigation-style app using gulp to build your ES6 code with the 6to5 compiler. Karma/Jasmine testing is also configured.

For more info please visit the official site: http://www.aurelia.io/


## Running The App

1. Fork or download this repo
2. Navigate into the folder
3. Install the Apps dependencies

  ```shell
  npm install
  ```
4. Download a fresh copy of the skeleton app by issuing following command:

  ```shell
  node bin/install
  ```
5. Navigate to the frontend folder

  ```shell
  cd public/app
  ```
6. Ensure that [Gulp](http://gulpjs.com/) is installed. If you need to install it, use the following command:

  ```shell
  npm install -g gulp
  ```
7. Ensure that [jspm](http://jspm.io/) is installed. If you need to install it, use the following command:

  ```shell
  npm install -g jspm
  ```
  > **Note:** jspm queries GitHub to install semver packages, but GitHub has a rate limit on anonymous API requests. It is advised that you configure jspm with your GitHub credentials in order to avoid problems. You can do this by executing `jspm endpoint config github` and following the prompts.
8. Install the client-side dependencies with jspm:

  ```shell
  jspm install
  ```
  >**Note:** Windows users, if you experience an error of "unknown command unzip" you can solve this problem by doing `npm install -g unzip` and then re-running `jspm install`.
9. To run the app go back to the project root and execute the following command:

  ```shell
  gulp watch
  ```
10. Browse to [http://localhost:7000](http://localhost:7000) to see the app. You can make changes in the code found under `src` and the browser should auto-refresh itself as you save files.

  >**Note:** If you prefer to run the node app without Gulp just do ``` node app.js ```
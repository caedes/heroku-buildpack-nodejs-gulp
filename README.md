# Heroku Buildpack for Node.js and gulp.js

## Usage

1. Add a Gulp task called `heroku:production` that builds your app

2. Serve your app using [Express](https://github.com/visionmedia/express) or [Shuss](https://github.com/ArnaudRinquin/shuss)

3. Set your Heroku app's buildpack URL by:

  ```sh
  $ heroku config:set BUILDPACK_URL=https://github.com/caedes/heroku-buildpack-nodejs-gulp.git
  ```

  To be safe, you should really fork this and use your fork's URL.

4. Set your environment to `production` (or any other name):

  ```sh
  $ heroku config:set NODE_ENV=production
  ```

## Credits

Forked from [heroku-buildpack-nodejs](https://github.com/heroku/heroku-buildpack-nodejs).

Heavily based on [heroku-buildpack-nodejs-grunt](https://github.com/mbuchetics/heroku-buildpack-nodejs-grunt).

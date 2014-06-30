# Heroku Buildpack for Node.js and gulp.js

## Usage

* Set your Heroku app's buildpack URL to `https://github.com/caedes/heroku-buildpack-nodejs-gulp.git`
  To be safe, you should really fork this and use your fork's URL.
* Run `heroku config:set NODE_ENV=production` to set your environment to `production` (or any other name)
* Add a Gulp task called `heroku:production` that builds your app
* Serve your app using [Express](https://github.com/visionmedia/express) or [Shuss](https://github.com/ArnaudRinquin/shuss)

## Credits

Forked from [heroku-buildpack-nodejs](https://github.com/heroku/heroku-buildpack-nodejs).

Heavily based on [heroku-buildpack-nodejs-grunt](https://github.com/mbuchetics/heroku-buildpack-nodejs-grunt).

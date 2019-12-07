Heroku buildpack: Firefox with geckodriver
=======================

This is a [Heroku buildpack](https://devcenter.heroku.com/articles/buildpacks) for [Firefox](https://www.mozilla.org/firefox). Meant to be used in combination with something like xvfb, for headless operation.

Usage
-----

Example usage:

```shell
$ heroku create --buildpack https://github.com/evosystem-jp/heroku-buildpack-firefox

# or if your app is already created:
$ heroku buildpacks:add https://github.com/evosystem-jp/heroku-buildpack-firefox

$ git push heroku master
```

Then, set Selenium configuration to below and launch.

- geckodriver path to `/app/vendor/geckodriver/geckodriver`
- firefox binary path to `/app/vendor/firefox/firefox`
# Scala and NodeJS buildpack [![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/Jarlakxen/heroku-buildpack-scala-grunt/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

### Enjoy using Grunt, Bower and Scala for develop your webapps. ###

This buildpack is a wrapper of the:

- [Scala Buildpack](https://github.com/heroku/heroku-buildpack-scala)

- [Nodejs Buildpack](https://github.com/heroku/heroku-buildpack-nodejs)

for make it work together

### Using Grunt and Bower ###

#### package.json

	{
		"name": "xxxxx",
		"version": "1.0.0",
		"dependencies": {
			"grunt-cli": "0.1.13",
			"bower": "1.2.8",
			"grunt": "0.4.2",
		},
		"engines": {
			"node": "~0.10.0"
		},
		"scripts": {
			"postinstall": "./node_modules/.bin/bower install; ./node_modules/.bin/grunt"
		}
	}

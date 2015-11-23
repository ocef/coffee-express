# Coffee Express Template

  [![NPM Version][npm-image]][npm-url]
  [![NPM Downloads][npm-downloads-image]][npm-downloads-url]
  [![Linux Build][travis-image]][travis-url]

[npm-image]: https://img.shields.io/npm/v/coffee-express.svg
[npm-url]: https://npmjs.org/package/coffee-express
[npm-downloads-image]: https://img.shields.io/npm/dm/coffee-express.svg
[npm-downloads-url]: https://npmjs.org/package/coffee-express
[travis-image]: https://img.shields.io/travis/pengkui/coffee-express/master.svg?label=TravisCI
[travis-url]: https://travis-ci.org/pengkui/coffee-express

This is a template for getting started writing Express.js application in
CoffeeScript, Jade, and Stylus, for both server app and client assets.

It comes ready to go with base setup for an Express Web App.
It includes a `Cakefile` that lets you build, spec,
and watch your CoffeeScript as you develop.
You hack in the `src` folder and run `cake build` to build you server files,
write your mocha in your test folder
and run `cake test` or `cake spec` to run your test suite.
Create your Jade views in the `views` folder
and put your public assets in the `public` folder.

It folks twilson63/express-coffee with mongodb dependencies removed.


## Technologies
This is a template that can be used to create nodejs applications using

* [NodeJs](http://nodejs.org) v4.2
* [Express](http://expressjs.com) v4.13
* [CoffeeScript](http://coffeescript.org) v1.10
* [Jade](http://jade-lang.com/) v1.11
* [Stylus](http://learnboost.github.io/stylus/) v0.52
* [bootstrap-stylus](https://github.com/Acquisio/bootstrap-stylus) v2.3.1 (not a npm module)
* [Nib](http://visionmedia.github.io/nib/) v1.1
* [connect-assets](http://github.com/TrevorBurnham/connect-assets) v2.5
* [Mocha](http://visionmedia.github.com/mocha/)

These will install with npm, just do

    git clone http://github.com/pengkui/coffee-express.git [project-name]
    cd [project-name]
    npm install

---


## Install coffee-script, mocha and docco

    npm install coffee-script -g
    npm install mocha -g
    npm install docco -g

# Run

    cake dev

### Mocha and Request for testing

Mocha is an extremely powerful and easy to use testing framework

see [http://visionmedia.github.com/mocha/](http://visionmedia.github.com/mocha/)

    describe 'Sample test', ->
      it 'should be true', ->
        true.should.equal true

To run mocha

    cake test

### Setup to deploy to heroku

    rm -rf .git
    git init
    echo 'node_modules' >> '.gitignore'
    git add .
    git commit -am "first commit"
    heroku create
    git push heroku master
    heroku open

## Contribute

Pull requests are welcome.

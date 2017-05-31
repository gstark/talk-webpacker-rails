# Webpacker w/ Rails

---

![stretch](https://media.tenor.co/images/0421521b4dd83516c44fab32d1fc07b6/tenor.gif)

---

# But first a confession

---

![fit](https://cdn.meme.am/instances/500x/76466776/dr-mccoy-im-not-a-doctor-javascript-dev-but-i-play-one-on-tv.jpg)

---

<br>
<br>
<br>

# [fit] JavScript makes me 😡

---

<br>
<br>
<br>

# [fit] My ❤️  belongs to 💎

^ I am not a JavaScript expert. I am known as a JavaScript hater

---

# [fit] However ...

<br>

# [fit] Modern JS no longer makes me 😱

<br>

# [fit] Over time I'm mostly 🤔

---

# But also ...

## I'm not a fan of the asset pipeline

---

# sbecker shoutout for asset packager!

![right fit](http://touchonthis.com/welcome/wp-content/uploads/2013/03/1.gif)

## https://github.com/sbecker/asset_packager

---

# Next generation

## jammit

![right stretch](https://media.giphy.com/media/bKnEnd65zqxfq/giphy.gif)

---

# Asset Pipeline

## Weird commented files

## Non standard tags in SCSS

## ERB tags in CSS

![right stretch](http://releaseyourclutter.com/wp-content/uploads/2011/08/overflowing-closet.jpg)

---

# Modern Javascript Tools

![autoplay](https://www.youtube.com/watch?v=vyUoCxjnXHE)

---

# Not settling for the status quo

---

# Webpack

> webpack is a module bundler for modern JavaScript applications.

---

# Webpack

> It is incredibly configurable

---

# Webpack

> But editing/adding-to a webpack config requires some more than cursory understanding of webpack

---

# Packaging Javascript code

> Where is the `gem` equivalent in JavaScript land?

---

# npm

- If you've done any javascript work with `npm` you know it is a :angry: experience
- Most frustrating: sllllooooowwwww

---

# Yarn

## fast
## caching
## parallelize

---

# Yarn

> Will use this to download packages and all of their dependencies

<br>

> There are a *LOT* of dependencies...

---

# Asset Pipeline

> Sprockets

- A great gem but reproduces a lot of what the JS world already has
- Maintenance is apparently quite difficult

---

# Can we merge the two?

![right fit](https://pbs.twimg.com/media/CywTph0WQAAm1eW.jpg)

---

![fit](http://www.reactiongifs.com/wp-content/uploads/2013/10/tim-and-eric-mind-blown.gif)

---

# [fit] rails/webpacker

---

# Small gem

- Mostly configuration
- ... and passing information to existing tools

---

# Rails "4.2"..."5.1"

## Officially deployed as part of 5.1

- At the same time we :skull: jQuery as a standard dependency

---

# Getting started

`https://github.com/rails/webpacker`

---

# Rails "4.2"..."5.1"

## Add gem to Gemfile

- For < `5.1`
- `gem 'webpacker', github: 'rails/webpacker'`

---

# Rails 5.1

`rails new --webpack`
`rails new --webpack=react`
`rails new --webpack=angular`

---

# MOAR CONFIGS!

- `config/webpack/*.js`

> Follows similar conventions of ruby configs
> Broken down into dev, test, prod

---

# [fit] YAPFC

> Yet Another Place For Code

---

# [fit] `app/javascript/packs/*`

---

# Each js file is the name of a `pack`

> These can be brought into a page with

> `javascript_pack_tag 'NAME'`

---

# Each css file is also the name of a `pack`

> These can be brought into a page with

> `stylesheet_pack_tag 'NAME'`

---

# [fit] Lets look at the sample

> ./bin/webpack-dev-server
> rails s

---

![fit](http://blog-assets.risingstack.com/2016/Jan/react_best_practices-1453211146748.png)

---

# [fit] `rails webpacker:install:react`

---

# [fit] I like `es2015` bleeding edge stuff!

<br>

# [fit] :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire:
# [fit] :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire:
# [fit] :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire:
# [fit] :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire: :fire:

---

# [fit] Add the dependencies

<br>

# [fit] `yarn add babel-preset-stage-0`
# [fit] `yarn add babel-preset-es2015`

---

```
// config/webpack/loaders/babel.js
// config/webpack/loaders/react.js
// .babelrc

"presets": [
  "react",
  "es2015",
  "stage-0",
  ["env", { "modules": false }]
]
```

---

# [fit] Lets make some `React` components!

---

## Managed Javascript Dependencies
### (no more downloading js bundles)
## Keep up with the _Joneses_
## es{2015,2016,2017} is a _decent_ version of javascript

![fit right](http://images.hellogiggles.com/uploads/2016/12/05063142/A_Whole_New_World.jpg)

---

# [fit] Thank You!

<br>
<br>
<br>

# P.S. Ruby Rulez

---

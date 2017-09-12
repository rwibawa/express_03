# express_03
[Express application generator](https://expressjs.com/en/starter/generator.html)

## 1. Setup
```bash
$ npm install express-generator -g
$ express -h
$ express --view=pug express_03
$ cd express_03
$ npm install

$ DEBUG=express_03:* npm start

$ tree
.
├── README.md
├── app.js
├── bin
│   └── www
├── package.json
├── public
│   ├── images
│   ├── javascripts
│   └── stylesheets
│       └── style.css
├── routes
│   ├── index.js
│   └── users.js
└── views
    ├── error.pug
    ├── index.pug
    └── layout.pug
```

### Open it
[http://localhost:3000/](http://localhost:3000/)

## 2. Pug template engine (formerly Jade)
* [Pug doc](https://pugjs.org/language/attributes.html)
* [expresjs integration](https://expressjs.com/en/guide/using-template-engines.html)

## 3. Heroku deployment

### Create a `Procfile`
```
web: npm start
```

### Heroku commands
```bash
$ heroku login
$ heroku create
Creating app... done, ⬢ morning-escarpment-26219
https://morning-escarpment-26219.herokuapp.com/ | https://git.heroku.com/morning-escarpment-26219.git

$ git push heroku master
...
remote: -----> Caching build
remote:        Clearing previous node cache
remote:        Saving 2 cacheDirectories (default):
remote:        - node_modules
remote:        - bower_components (nothing to cache)
remote:
remote: -----> Build succeeded!
remote: -----> Discovering process types
remote:        Procfile declares types -> web
remote:
remote: -----> Compressing...
remote:        Done: 19.1M
remote: -----> Launching...
remote:        Released v3
remote:        https://morning-escarpment-26219.herokuapp.com/ deployed to Heroku
remote:
remote: Verifying deploy... done.
To https://git.heroku.com/morning-escarpment-26219.git
 * [new branch]      master -> master


$ heroku open
$ heroku logs --tail
```

## 4. Setup Angular UI
```bash
$ mkdir public/vendor

$ echo '{"directory" : "public/vendor"}' > .bowerrc
$ npm install bower --save

$ bower init
$ bower install bootstrap --save
$ bower install angular --save
$ bower install angular-ui --save
$ bower install font-awesome --save
```
 
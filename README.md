# express_03
Express application generator

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


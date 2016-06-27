# adonistest

0) Run `npm i` in both foldtest and adonis-validation-provider

1) In adonis-validation-provider run `npm link`

2) In foldtest run `npm link adonis-validation-provider`

3) In foldtest run `npm run dev`

    Error: Cannot find module 'Helpers'
        at Function.Module._resolveFilename (module.js:326:15)
        at Function.Module._load (module.js:277:25)
        at Module.require (module.js:354:17)
        at require (internal/module.js:12:17)
        at requireStack (Your/Path/Here/adonisfoldissue/adonis-validation-provider/node_modules/require-stack/src/index.js:44:12)
        at Ioc.use (Your/Path/Here/adonisfoldissue/adonis-validation-provider/node_modules/adonis-fold/src/Ioc/index.js:342:14)
        at Your/Path/Here/adonisfoldissue/foldtest/bootstrap/http.js:44:23
        at process._tickCallback (node.js:382:9)
        at Function.Module.runMain (module.js:432:11)
        at startup (node.js:141:18)

4) In foldtest run `npm unlink adonis-validation-provider`

5) In foldtest run `npm i` to reinstall adonis-validation-provider

6) In foldtest run `npm run dev`

    [nodemon] 1.9.2
    [nodemon] to restart at any time, enter `rs`
    [nodemon] starting `node --harmony_proxies server.js`
    info adonis:framework +9ms serving app on localhost:3333

Back in business.

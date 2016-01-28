

See https://angular.io/docs/ts/latest/quickstart.html

run > npm install....

Preparation:
============
 1) create the package.json for use with npm (from the command line)
    Package.json is used in 2 places:
       1) when running > npm install to download all required libraries (and their dependencies)
       2) when running > npm start to run concurrently invoke the tsc and running the lite server.

 2) the tsconfig.json is for use by tsc (also run from command line).
    Run > npm start. This will do 2 things:
       - watch the directory for changes and invoke the tsc compiler if this is the case.
       - use node file server to serve our files. It also invokes the browser at http://localhost:3000/
         to test the index.html file.

 3) In Settings > Typescript Tsc, set:
     - Resolve objects using tsconfig.json
     - Enable Typescript compiler
        - track changes
     - use tsconfig.json



This is a SUCCESSFUL project in 2 ways:
  - the tsc compiler watches the relevant files (see output below)
  - the node.file

Here's the output of > npm start:

    C:\Users\Thanh Nguyen\IDEAPROJECTS\2016_01_07\Games_01\Angular2_Tut_1>npm start

    > angular2-quickstart@1.0.0 start C:\Users\Thanh Nguyen\IDEAPROJECTS\2016_01_07\Games_01\Angular2_Tut_1
    > concurrent "npm run tsc:w" "npm run lite"

    [0]
    [0] > angular2-quickstart@1.0.0 tsc:w C:\Users\Thanh Nguyen\IDEAPROJECTS\2016_01_07\Games_01\Angular2_Tut_1
    [0] > tsc -w
    [0]
    [1]
    [1] > angular2-quickstart@1.0.0 lite C:\Users\Thanh Nguyen\IDEAPROJECTS\2016_01_07\Games_01\Angular2_Tut_1
    [1] > lite-server
    [1]
    [0] 10:52:23 PM - Compilation complete. Watching for file changes.
    [1] [BS] Access URLs:
    [1]  -------------------------------------
    [1]        Local: http://localhost:3000
    [1]     External: http://192.168.2.16:3000
    [1]  -------------------------------------
    [1]           UI: http://localhost:3001
    [1]  UI External: http://192.168.2.16:3001
    [1]  -------------------------------------
    [1] [BS] Serving files from: ./
    [1] [BS] Watching files...
    [1] 16.01.27 22:52:30 200 GET /./index.html (Unknown - 170ms)
    [1] 16.01.27 22:52:31 304 GET /node_modules/es6-shim/es6-shim.min.js (Unknown - 60ms)
    [1] 16.01.27 22:52:31 304 GET /node_modules/systemjs/dist/system-polyfills.js (Unknown - 61ms)
    [1] 16.01.27 22:52:31 304 GET /node_modules/angular2/bundles/angular2-polyfills.js (Unknown - 60ms)
    [1] 16.01.27 22:52:31 304 GET /node_modules/systemjs/dist/system.src.js (Unknown - 60ms)
    [1] 16.01.27 22:52:31 304 GET /node_modules/rxjs/bundles/Rx.js (Unknown - 60ms)
    [1] 16.01.27 22:52:31 304 GET /node_modules/angular2/bundles/angular2.dev.js (Unknown - 61ms)
    [1] 16.01.27 22:52:32 200 GET /app/boot.js (Unknown - 71ms)
    [1] 16.01.27 22:52:33 200 GET /app/app.component.js (Unknown - 99ms)

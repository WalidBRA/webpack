# `Quick start`

node -v <br />
the version must be : 21.1.0.

npm -v
the version must be: 10.2.1
npm install -g aurelia-cli
**Note:** the version of Aurelia must be: global aurelia-cli v3.0.2
cd path/to/project
npm install
au run --open
python3 -m venv venv-kdt-rfs
source venv-kdt-rfs/bin/activate
python3 -m pip install -r requirements.txt
robot --outputdir robot_output test/ui/todos.robot

## Run dev app

Run `npm start`, then open `http://localhost:8080`

You can change the standard webpack configurations from CLI easily with something like this: `npm start -- --open --port 8888`. However, it is better to change the respective npm scripts or `webpack.config.js` with these options, as per your need.

To enable Webpack Bundle Analyzer, do `npm run analyze` (production build).

To enable hot module reload, do `npm start -- --hmr`.

To change dev server port, do `npm start -- --port 8888`.

To change dev server host, do `npm start -- --host 127.0.0.1`

**PS:** You could mix all the flags as well, `npm start -- --host 127.0.0.1 --port 7070 --open --hmr`

For long time aurelia-cli user, you can still use `au run` with those arguments like `au run --env prod --open --hmr`. But `au run` now simply executes `npm start` command.

## Build for production

Run `npm run build`, or the old way `au build --env prod`.

## Unit tests

Run `au test` (or `au jest`).

To run in watch mode, `au test --watch` or `au jest --watch`.

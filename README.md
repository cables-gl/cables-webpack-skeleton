# cables.gl webpack skeleton

## requirements
* download this skeleton (do not clone the git repository if you are just using this for your own projects)
* install nodejs and npm
* this guide assumes you have some kind of "shell" working (linux, osx, windows linux subsystem (WSL))
* get/create an api-key in cables (https://cables.gl/settings -> apikeys -> create)
* copy the patch-id into package.json in the "patchup"-script call (replacing ##patchId##)

## prepare
`npm install`
* installs neccessary dependencies to local node_modules/ folder

## synchronize patch with cables
`npm run patchup`
* deletes all local files in the patch/ directory
* download current version of the patch in cables.gl to patch/
* might ask for authorization by api-key on first run
* find more documentation at: https://github.com/cables-gl/cables-cli

## run
`npm run start`
* runs a local webserver that hotswaps all the files for development

## build
`npm run build`
* builds the standalone webapp including all assets to the dist/ folder

## deploy
### to production
1. build the project
2. copy dist/ folder to webserver
3. ???
4. profit

# Angular library template

## Install

After cloning this repository, install dependancies.

> npm install

## Change prefix

In "angular.json" file, change "prefix".

![Prefix in angular config](/docs/images/angular.png "Prefix in angular config")

In "library/tslint.json", change "prefix".

![Prefix in tslint config](/docs/images/tslint.png "Prefix in tslint config")

## Create a new component

In root project :

> ng g component my_component --project library

![New component](/docs/images/component.png "New component")

After, export this component in library.module.ts and public_api.ts.

## Build

In root project :

> npm build

## Publish

The library will be published under the name "library".
To change this, update name value in library/package.json.

![Publish name](/docs/images/package.png "Publish name")

## Use

In new angular project, import the library.

> npm install *my_library*

If your library has been published in private registry.

> npm install *my_library* --registry *http://npm.myregistry.com*

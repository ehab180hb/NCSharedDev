# @naturalcycles/shared-dev

To be installed as __dev__ dependency:

    yarn add -D @naturalcycles/shared-dev
    
Upgrade it like this:

    yarn upgrade @naturalcycles/shared-dev
    
# Idea

Only dependencies that's gonna be used as __dev__ dependencies should be added here.

If package has a chance to be a part of __prod__ dependencies - __DON'T__ add it, to avoid
many different versions installed at the same time.

If package has peerDependencies, or some other package peer-depend on it - __DON'T__ add it, cause
it will show `warning: missing peerDependency` in the main package. Example - things that depend on `jest`.

## Common deps

```
yarn add \
luxon \
bluebird

``` 

## Common dev deps

```
yarn add -D \
@types/bluebird \
@types/fs-extra \
@types/jest \
@types/node \
@types/yargs \
del-cli \
fs-extra \
husky \
jest \
jest-fetch-mock \
jest-junit \
lint-staged \
prettier \
ts-jest \
ts-node \
tslint \
tslint-eslint-rules \
yargs \

```

## Other deps
```
nunjucks
@types/nunjucks
cheerio
@types/cheerio
```

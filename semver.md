# May 2021

## Wednesday, 26th

Today I learned about Semantic Versioning and what different notations regarding versions of dependencies of a given npm packages mean.

The general syntax is when descriping a version of an application's dependencies is like this, Major.Minor.Patch.

* Patch is used for fixing bugs
* Minor is used for adding features that don't break the existing API
* Major is used for adding features that could potentially break the existing applications that depend upon this version of a given npm package

Here is an example:
```js
"dependencies": {
    "mongoose": "^4.13.6",
    "underscore": "1.8.3",
    "lodash": "~4.0.3" 
}
```



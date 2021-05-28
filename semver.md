# May 2021

## 26

### SemVer
Today I learned about Semantic Versioning and what different notations regarding versions of dependencies of a given npm packages mean.

The general syntax of versions of packages/dependencies is like this, Major.Minor.Patch.

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

What the symbols in front of the major mean:
* ^ [caret] means that any version as long as the major version is 4 will do
* ~ [tilda] means that any version as long as the major is 4 and minor is 0 will do
* Empty means that this exact mentioned version is necessary for the application to work properly

### Make list of installed packages
I *also* learned how to make a list of installed packages, that there are time consuming ways to do it and fast ways to do it.  

One way to do this is by following the path
 *node_modules>[npm_package]>package.json* and then look for "version" at the button of the file.  
 
 A faster way to do this is by using the terminal. In order to get a list of installed dependencies and their exact versions, write the following:  
 `$npm list`  
 
 To get a list that shows x levels of installed dependencies and their exact versions, instead write:  
 `$npm list --depth=x`

 If one is only interested in dependencies of their own application, use:  
 `¤npm list --depth=0`

### View metadata of npm packages
Lastly, I learned how to view metadata of a given npm package. Of course these information can be looked up on npmjs.com. However, these information can also be obtained by using a terminal.   
In order to view metadata in a package.json file of a given npm package, simply write: 
`$npm view lodash`

If one is only interested in the dependencies of a given npm package, instead write: 
`$npm view lodash dependencies`

To get a list of all released versions of an npm package so far, use: 
`$npm view lodash versions`
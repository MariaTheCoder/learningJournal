
# May 2021

## 27

### Check for updates and update installed dependencies
Today I learned how to check in terminal whether there updated versions of installed packages have been released. By writing the following command, one should receive a table of outdated npm packages currently installed.  
`$ npm outdated`

To update the packages, use  
`$ npm update`
However, this command only works with minor and patches updates, not major. 

In case of major updates, it is necessary to install a new command line tool called npm-check-updates.   
`$ npm i -g npm-check-updates`

By running the new command line tool, you get an overview of installed outdates packages.
`$ npm-check-updates`

This package can then be used to update the section about dependencies in the package.json file.  
`$ ncu -u`  
Beware that we haven't installed the update yet - we have only updated the package.json file.  

To install the major update of an installed dependency, use  
`$ npm i`

### DevDependencies
Some dependencies are not needed to run an application but solely used to develop the application. Good examples of these are packages such as prettier, jshint, npm-check-updates and so on. As these dependencies are used by developers during the development, they have been named DevDependencies. 

This is how to install a DevDependency  
`$ npm i jshint --save-dev`





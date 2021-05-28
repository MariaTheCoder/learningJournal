
# May 2021

## 25

Today I learned about SCM/VCM (Source/Version Controle Management). Since a node_module folder can quickly take up many MB, the node_modules folder is often excluded when it is intended to share source code.   
Is that a problem? No, because the dependencies of the code will be listed in package.json file. 

When to make a commit to GitHub, and you do not want to save the node_modules folder, you can tell Git by creating a new file called ".gitignore". Inside this file, you type in which files or folders to ignore. 
If one desides to ignore the "node_modules/". This notation indicates that the element to ignore is a folder.

I also learned how to commit to git via terminals such as GitBash. 

* Use `$git init` to initialize empty Git repository. 
* Use `$git status` to view untracked files. 
* Use `$git add .` to indicate that current status is what you desire to commit. Dot always means *this folder*.
* Use `$git commit -m` when you want to do your commit. -m is the message of the commit. 

Lastly, I learned about Markdown today.
<img src="sun.jpg" alt="Happy Sun" style="height: 250px, width: auto">

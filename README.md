# Website for Google Student Developer Club San Jose State University


## Run in your local

```
git clone https://github.com/dscsjsu/sjsu-gdsc-website.git 
```

```
brew install hugo
```
```
cd sjsu-gdsc-website
```


```
hugo server
```


## To contribute

1. Make sure your local repo is the latest update.
2. Create a branch, code, push to your branch and make a pull request. 
3. Design team will review the pull request and merge it with master branch. 

Some basic git commands:


Make sure your local repo is the up-to-date.
```
git pull origin master
```

See branch
```
git branch
```

Create branch
```
git branch branchname
```

Change branch
```
git checkout branchname
```

Code. Then push to your branch
```
git add .
git commit -m 'your message here'
git push origin branchname
```

Go to online github repo, and create pull request. 
Design team will review, merge to master branch and delete the branch.
After the pull request is merged. Proceed to update your local repo and delete the local branch. 

```
git checkout master
git pull origin master
git branch -d branchname
```

## Understanding the architecture

This website is built using the [Academic](https://sourcethemes.com/academic/) on [Hugo](https://gohugo.io) static website generator. 

```bash
├── app
│   ├── css
│   │   ├── **/*.css
│   ├── favicon.ico
│   ├── images
│   ├── index.html
│   ├── js
│   │   ├── **/*.js
│   └── partials/template
├── dist (or build)
├── node_modules
├── bower_components (if using bower)
├── test
├── Gruntfile.js/gulpfile.js
├── README.md
├── package.json
├── bower.json (if using bower)
└── .gitignore
```




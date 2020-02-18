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

## Understanding the structure

This website was built with the [Academic](https://sourcethemes.com/academic/) theme on [Hugo](https://gohugo.io) static website generator hosted on [Github](https://github.com/dscsjsu/sjsu-gdsc-website) served by [Netlify](https://www.netlify.com).

Hugo prioritize all the files that's not in the `./themes` folder. If such file does not exist, then it will run the file from `./themes` folder. 

So, `./themes` contains the default design of the website. and the files outsides of the `./themes` folder are the contents of the website.

Therefore, in order to edit/update the design of the website, you must identify the correct html files and the css scripts. Copy/paste the html files from the `./themes/academic/layouts` folder and put it in the the root directory `./layouts` folder. 
Identify the right css script, copy/paste it into the `./assets/scss/custom.scss` file. Edit the html file and the css script. 

This theme is using a widget system. A page can contain one or multiple widgets which are the sections of the page. 

Edit the markdown file in the `./content` folder accordingly to add more contents. 

Below are the important directory for this website. 
```bash
├── assets
│   ├── js #put all custom local js in this folder
│   └── scss
│       └── custom.scss #all custom css files are in here
│
├── config
│   └── _default
│       ├── menus.toml #to add/hide navbar menu
│       └── params.toml 
│
├── content
│   ├── authors #default folder for adding user or people in the team
│   ├── project #default folder for adding resources for resources page (tools) page
│   ├── talk #default folder to add events
│   ├── home #A page -- a homepage that has multiple section of "widgets" in .md file
│   └── tools # A page -- a custom page. To create a page, just create a folder in ./content
│
├── layouts # all updated html files
│
├── static
│   └── img #all static images are in here
│
└── themes
    └── academic # academic theme templating
        └── layouts 
            └── partials 
                └── widgets #to add/edit the html design of each widgetr section. Copy from here
                            #and paste in ./layouts/ accordingly with the same hierarchy

```




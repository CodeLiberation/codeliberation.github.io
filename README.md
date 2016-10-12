Code Liberation website
========================

Hello! Below is some information about contributing to this website. If you'd like to see it live, [it's on the internet](http://codeliberation.github.io).

# Contributing
Please request contributor access or submit a pull request to push your code to this repository.

## Getting started
To begin, set up an area on your computer where you'll be doing development. Once you're ready, open your command line program of choice and enter:

`git clone git@github.com:CodeLiberation/codeliberation.github.io.git`

This repository will now be available on your computer.

### Jekyll
This project uses [Jekyll](https://jekyllrb.com/). Once you've cloned the repository, please install Jekyll by entering the text below into your command line program of choice:

`gem install jekyll`

If this command doesn't work, you need to install [Ruby](https://www.ruby-lang.org/en/). Do that and come back.

After you install Jekyll, it's ready to go!

## Running the site on your local computer
To run a local version of the site, enter the following your command line program of choice:

`jekyll serve`

You should now be able to see the site in your browser by going to `http://127.0.0.1:4000/`. Every time you make an edit to an image, HTML, JS, or CSS file, you can reload and see your change. However, you will need to cancel and re-enter your command any time you make a change to the _config.yml file.

## Making edits
The folder structure is already somewhat straightforward, but here's a general explanation to make it extra clear!

### _bios
Team member biographies go here. They are markdown files and can be edited with any text editor. As for properties: `title` should be the name of the team member; `image` should be **the lowercase first name + filetype** for this team member's image (you can find and put images in `img/team`), and the type should either be `director`, `member` (this is probably you!), or `emeritus` (alumni of Code Liberation).

### _includes
Snippets of code that can be included and reused are placed here.

### _layouts
Common layouts found across the site are in this folder. These are like includes but larger-scale (page-level vs. content-level).

### _posts
Blog posts are all in here. To write a new one, duplicate the template file called `YYYY-DD-MM-post-template.markdown` and follow its instructions.

### _sass
All the CSS goes here. Learn more about sass [via their site](http://sass-lang.com/). If you need to create a new css file, please follow the naming convention then link at the bottom of `css/main.scss` following the convention shown in the file.

### _site
Don't touch this – this is automatically compiled by Jekyll.

### about, blog, sponsors, team, and volunteer
These folders contain the templates (and content, for the most part) for these pages. Look at them to understand how they work.

### css
Contains the file that joins all the sass files. See _sass above for more info.

### files
Store non-image, non-font files here.

### fonts
Put fonts here.

### img
Put images here. Images are organized in folders according to purpose right now. Follow the convention and create new folders as needed!

That's it! You know all about files now! Yay! Go forth and EDIT.

## Pushing changes
To push changes, put the following into your command line program of choice. 

`git status`

This lets you see the changes you've made.

`git add .`

This will add ALL modified tracked files to your upcoming submission.

`git commit -m "YOUR_MESSAGE_HERE"`

This will save your changes to the local repository with a message.

`git pull --rebase`

Always make sure your repository is up to date and that changes don't hurt others' repositories by running `git pull` with the [rebase](https://git-scm.com/book/en/v2/Git-Branching-Rebasing) command before pushing new changes!

`git push`

This will upload your changes to master! HUZZAH!

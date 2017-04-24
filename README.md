## Git Essentials Workshop

This tutorial is to get you comfortable working with and understanding some basic git concepts.

But first some intro concepts!

## Version Control
Is basically managing changes in documents or code. As projects get bigger and bigger, it’s very important keep track of changes and versions so we can go back and forth when needed.

### Git Overview
- version control system behind Github
- written by Linus Torvald
  - to version control the Linux kernel.
There are many interfaces to use git, but today we’ll work from the terminal.

### How it can help you?
Why learn Git:
- keeps a copy of all the older version
- can give you a timeline of changes to files
- structure your projects better
- documentation
- makes sharing and collaborating easier!


## Git Workshop
After going through this tutorial, you will:

- Understand what version control is about
- Know the basics of how to use Git and GitHub from the command line
- Be able to start using GitHub to share and collaborate!

### Step 1: Prerequisites

First, you’ll need:
- git installed
- a github account
- an SSH key added to your Github account

### Step 2: Fork this Repo

On Github, fork this repo. Your forked repo will give you commands to set up this repo on your machine.

`git init`
`git remote add origin` of the repo

### Step 2: Create your `develop` branch

Now that you have the site setup, you should be inside your git-tutorial repo folder. If you type `git status` you’ll see that your repo is up to date.

Now, lets say we want to work on a specific feature. Let’s create a branch called `develop`.
 To do this we use the command `git checkout -b develop` which creates the develop branch from the branch we’re on (`master`) and moves us to it.

### Step 3: Take a look at the files in the repo

Open these files in the text editor of your choice. For now, we just have these two files in the repo. This `readme.md` and an `index.html`.

Your job is to change the title of our lovely `index.html` page.
So go ahead and find the `<title> Something something </title>` and change the words inside the `<title>` tags.

### Step 4: Seeing your changes

Now that you’ve changed the title of the page, save the file `CTRL+S`. Go back to your terminal and type `git status`.

Now you’ll see a new message. This time git is telling you that a file has been changed! To look at these changes, we use `git diff` (what’s the difference between my remote branch - the one on github and my local branch - the one on my machine).

This command will output all the changes in the repo. You’ll see your title change here!

### Step 5: Committing your changes

Now we want to share our changes with the world. Since we’ve seen the diff, we decide to add these changes to the repo.

We use the command `git add PATHTOFILE`

Now, to see what happened, run `git status`. You’ll see that the staged file (which was probably red) is now green, because it’s ready for commit.
 Now that we’ve prepared our change, we commit with a message. Use the command `git commit -m` where the `-m` flag allows us to type a message like so:

`git commit - "Changed the title to something else."`

This will commit the change we made to the file with this message. Commit messages are super useful on large projects when you have to hunt down when something was added or removed and why.

### Step 6: Looking at the version control log.

Now that you’ve committed, you can take a look at the version control history. To do this, use the command `git log --decorate` I personally like the `--decorate` flag because it makes things more interesting.

You can try both. `git log` and then `git log --decorate` for your preference.

This will show you the first commit - when I created this repo - and your commit - the changes you just made. Exciting!

### Step 7: Pushing your changes to Github.

Now we’re ready to show the world what we’ve done! Since our commit all ready to go, we just have to push it up to Github. To do this, we use the command `git push`

You can now go to your forked repo on github.com and take a look at your commit.

***That’s all we’ve got for today! *** There are more exciting things that can be done with Github like pull request and code releases, but we’ll tackle them another time.

## Resources

## Useful Links and Resources
- [Git Cheat Sheet - PDF with most used commands](00fe6987fe1a65434ee900da09b4c54113ee3dd0)
- [Code School - Interactive 15-minute tutorial, very useful for beginners](https://try.github.io/levels/1/challenges/1)
- [Youtube - Derek Banas - Git Video Tutorials Playlist](https://www.youtube.com/playlist?list=PLGLfVvz_LVvQHO1PfyscjIPkNJjgHsLyH)
- [Markdown Tutorial - Interactive tutorial to learn Markdown (the standard used to format readme files)](http://www.markdowntutorial.com/)

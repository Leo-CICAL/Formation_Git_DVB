
# Mini TP Git 

(Oui je l'ai écrit en anglais, ça vous fait bosser en encore plus <3)

Practice using git + Github

This project will consist of three separate mini-projects to get you comfortable with the kinds of activities you'll be using GIT for throughout the class. 

In the first mini-project, you'll be mimicking the steps you'll take when you first start your personal project. Creating a repository, linking it to your computer, then pushing those changes up to your GitHub.

In the second mini-project, you'll be mimicking the steps you'll take with nearly every DevMountain project you do. You'll 'fork' the DevMountain repository, link your computer with your fork, then push those changes up to your GitHub.

Finally, in the last mini-project you'll see the power of Git when you're programmming with a groupe !

I hope you're going to like it, and I'me here if you need me ! (If I made any errors using english, sorry not sorry <3)

## Mini-Project 1: Personal Project

## Step 1

### Summary

In this step we will create a repository on GitHUB.

### Instructions

* Go to <a href="https://github.com/">GitHub</a>.
* Sign in to GitHub.
* On the right side of the page, click on the green `New repository` button.
* Give your repository any name you like (for example, 'DVBcTroKool' ) and make sure that the repository is public.
* Also make sure that the `Initialize this repository with a README` is <b>NOT</b> checked !

## Step 2

### Summary

In this step we will setup the origin for the GitHub repository. We'll do this by connecting code on our computer to the GitHub repository we just created.

### Instructions

* In your computer, create a folder called `myProject`.
* Go into that folder.
* Create a file called `myName.txt` and add your name to that file.
* Save the file and open a terminal window (if you're on Windows, Right-Click and Select 'Open a Git Bash').
* In your terminal window, `cd` to your `myProject` folder (so go to your folder with the terminal).
* Run `git init`. 
  * <details>

    <summary> What just happened? </summary>

    <br />

    You've just told your computer that you want git to watch the `myProject` folder and to keep track of any changes. This also allows us to run git commands inside of the folder. (Warning:  Be very careful to make sure you're in the right directory when you run `git init`!)

    </details>
* Run `git remote add origin [Repository URL goes here]`. You can get your URL from going to repository you made earlier in your browser and copying the address.
  * <details>

    <summary> What just happened? </summary>

    <br />

    Basically, we tell our computer "Hey, I created this repo on GitHub, so when I push, I want my code to go to this GitHub repo." Now whenever you run `git push origin master` your computer knows that origin is pointing to your repo you made on GitHub and it pushes your changes there.

    <br />

    ( If you accidentally DID initialize your repository with a README, you must do a `git pull origin master` first - to get the README file on your computer - before you'll be able to push. ) 

    </details>

## Step 3: Push your code to GitHub

### Summary

In this step, we will push code and files to GitHub.

### Instructions

* Open a terminal window and make sure it is in the directory of `myProject`.
* Run `git status`.
  * <details>

    <summary> What does this do? </summary>

    <br />

    This will show what files have been changed. This also helps us determine what files we want to add to GitHub and what files we don't want to add to GitHub.

    </details>
* Run `git diff`.
  * <details>

    <summary> What does this do? </summary>

    <br />

    This will show the actual code that has been changed. Again, we want to make sure we don't push anything to GitHub that shouldn't be there.

    </details>
* Run `git add nameOfMyFile.fileExtension`.
  * <details>

    <summary> What does this do? </summary>

    <br />

    This adds our file(s) to the 'staging area'. This is basically a fail safe if you accidentially add something you don't want. You can view items that our staged by running `git status`.

    </details>
* Run `git commit -m "The sentence I want associated with this commit message"`.
  * <details>

    <summary> What does this do? </summary>

    <br />

    This tells your computer: 'Hey, the next time code is pushed to GitHub, take all of this code with it.' The message also specifies what GitHub will display in relation to this commit.

    </details>
* Run `git push origin master`
  * <details>

    <summary> What does this do? </summary>

    <br />

    Your code is now pushed to GitHub. Be sure to include `origin master`, as this tells GitHub which branch you want to push to, and creates the branch if it doesn't exist yet.

    </details>
* Go to your repository on GitHub and see your updates.

## Mini-Project 2: DevMountain Project

## Step 1

### Summary

In this step, we will fork this tutorial repository.

### Instructions

* On this current GitHub repository (so my repository GitHub, https://github.com/Leo-CICAL/forma_git_dvb/), scroll to the top and look for a button that says `fork`.
* Click the `fork` button.
  * <details>

    <summary> What does this do? </summary>

    <br />

    This will essentially copy all of the code from this repository, but make it as a new repository under your account. As you can imagine, you can't push directly to the DevMountain repo, because that would not be secure for DevMountain (anyone could make any changes they want). What you should do is create a fork of this repo, then push to your own fork because it's under your own account.

    </details>

## Step 2

### Summary

In this step, we will take the forked repository and clone it down to our machine.

### Instructions

* Go to your forked repository on GitHub. It should appear under `Your repositories` which is next to the `New repository` button.
* Click on the green `clone or download` button and copy the URL.
* Open a terminal window and navigate to your Desktop.
* Run `git clone [the url you copied]`.
  * <details>

    <summary> What does this do? </summary>

    <br />

    This takes what's on GitHub and essentially downloads it so you can now make changes to it on your local computer.

    </details>

## Step 3

### Summary

In this step, we will make changes to our clone and push them to GitHub.

### Instructions

* Open the folder in your coding IDE.
* Make a change in a file (for example, change a phrase in the ReadMe file).
* Run through the steps outlined in `Step 3` of the first project : git status, git add, git commit and git push (WHEN YOU GIT PUSH, JUST "git push")
  * Since you've cloned this repository, it is already pointing to your forked version. Therefore, you don't need to tell your computer where to push the code.


## Mini-Project 3 : Group Project together :D

### Summary

You're going to clone a Private Repository with a program that you're all going to modified. 

### Instructions

* Give me your Git's Username, because I have to had your account in the private repository that you're going to use.
* Go to this repository : https://github.com/Leo-CICAL/tp_git
* Clone it.
* Go to the file 'name.py' and add a print with your name on it.
* Run through the process of pushing to GitHub ( status, diff, add, commit, push).
* You'll see whent the diffetent commit will arrive :D.

## Contributions

If you see a problem or a typo, please fork, make the necessary changes, and create a pull request so we can review your changes and merge them into the master repo and branch.



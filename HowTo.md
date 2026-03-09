Assuming you have had a branch made for you, here is how to use github. 
First you must be able to access and use your terminal or command prompt on your computer (personal only, school blocks).
All commands shown are ran in a command line that has been opened inside your root folder. On Windows, open the folder and 
right click -> open in terminal.
On MacOS, follow the picture below.
<img width="590" height="651" alt="Screen Shot 2026-03-09 at 8 15 17 AM" src="https://github.com/user-attachments/assets/06c94bf9-e73b-47ba-b48d-172ed5fa2fb0" />

(Open the folder, and then right click it at the bottom of finder and click open in terminal.)


# Setting up
## "Logging" in
Open terminal or command prompt in any way and run
```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```
Replace your name and email with the ones you use on Github.

## Repository and Branch setup
Run this command inside of a folder you have dedicated to rocketry but replace <branch-name> with the name of your branch. This is your root folder. 
```
git clone -b <branch-name> --single-branch https://github.com/1shiv1/dprocketry
```
I will most likely create a branch with just your folders, so you will not need to work outside of it. If you need to/do make changes 
outside of your file, let me know so I can handle any conflicts.
For example, your files should only be EggChallenge, inside it the folder with your name, and all of the folders in there are
yours.

# Working in your workspace

Now, inside your challenge/name folder, you can upload your .ork file and/or any other files. You can also edit your ReadMe for your rocket, which you can add notes for other people. 
You will primarily need to know three commands when working.

## Pulling
The first thing you need to do, which you should always do before opening and working on your file, is running
```
git pull
```
This will update the work on your computer with any changes that have been made and uploaded by someone else to your file. 
This will only happen if you edited something directly from the github website or are working with someone else.

## Staging
Now that we have made changes, I will refer to everything like you are shipping a box.
First, stage every file you would like to update in the repository. Staging means you are going to "pack it in a box for shipping."
Run
```
git add <file or path to file>
```
For example, if you need to add your newly added file in egg challenge, you run
```
git add EggChallenge/MyName/myRocket.ork
```
Do this for all files you want to be updated. They are all now in the staging area.

If you run
```
git status
```
You will be able to see all files that you have staged ("put into the box") for pushing and "shipping". Green means it is staged, red means it is not staged.

## Commits and Pushes
Now, after you had made changes/notable progress, you can run the commit command. 
The commit command will take everything in your staging area and "pack it into a box and label it."
```
git commit -m "This is the title" -m "This is the description"
```
This will update your local repository, which is just the folder on your computer, which contains all of your "snapshots" of work. Another way to think of it
is where you keep all of your labeled boxes.
To sync the local repo on your computer to Github, run
```
git push
```
This will sync everything on your computer to github. You are now "Shipping" the box to github, updating the repository.

And that is the workflow. Let me know if you have any questions.

# Workflow
1. ```git pull``` (Get updates)
2. ... do your work in OpenRocket ...
3. ```git add <your-folder-path>``` (Pack the box)
4. ```git status``` (Double check the box)
5. ```git commit -m "Title" -m "Desc"``` (Label the box)
6. ```git push``` (Ship it)

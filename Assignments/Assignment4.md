# Assignment 4 - Persistent Data on Client

## In this assignment your app needs to do the following:

* Have a Form
    * Just needs to be some way for the user to give input does not need to be a formal form for this. 
* Store a Persistent state in the SQLite DB or SharedPreferences on the phone or web
* Form updates the state
* View updates based on the changed state

As long as your app does those tasks you will get credit for this assignment.

## Getting Graded

When you have your APK move it to the root directory of your GIT repo that you were given to turn in assignments for this class. Do not use Android Studio or VScode to manage your VCS/Repo as it may screw up the repo. So for this assignment you should have a directory that looks like the following:

```
    /
    ...app-release.apk
    ...AssignmentProject/
    ......android/
    ......ios/
    ......web/
    ......lib/
    ......pubspec.yaml
    ......(Rest of App Files)
```

### Alternatively

```
    /
    ...web.md
    ...AssignmentProject/
    ......android/
    ......ios/
    ......lib/
    ......web/
    ......pubspec.yaml
    ......(Rest of firebase App Files)
```
In your web.md file you should have a web URL for your assignment hosted online. 

### Now submit your code to the **assignment4** branch on GitLab:

```
git checkout -b assignment4 #create branch and switch to it
git add -A #add all
git commit -m "Assignment 4 Submission" #Commit changes to branch
git push --set-upstream origin assignment4 #Push code up to assignment3 branch on remote
```

Make sure your branch is exactly named **assignment4** matching the case, spacing, etc as my grading script will only pull your submission if it matches exactly.

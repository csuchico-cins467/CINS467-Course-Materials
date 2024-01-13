# Assignment 5 - Firebase

## In this assignment your app needs to do the following:

* **Use a Form**
  * Needs to be some way for the user to give input.
  * This can be implemented with either an [EditableText](https://api.flutter.dev/flutter/widgets/EditableText-class.html) field or an actual [Flutter Form](https://api.flutter.dev/flutter/widgets/Form-class.html) with a TextField.
* **Store a Persistent state on Firebase**
  * You must set up a project on [Firebase](https://firebase.google.com/)
  * You will need to use the [cloud_firestore](https://pub.dev/packages/cloud_firestore) and [firebase_core](https://pub.dev/packages/firebase_core) plugins
* **Form updates Firebase**
  * When the form receives user input, it must update data that is stored in the Firestore database.
* **View updates based on the changed state**
  * When the data in your Firestore Database changes, the view that the user sees in your app must also update to reflect that change.

As long as your app does those tasks you will get credit for this assignment.

The goal of Assignment 5 is similar to the goal of Assignment 4, but this assignment is specifically aimed at giving you experience working with Firebase Cloud Storage. Cloud Storage is more reliable and more scalable than other persistent storage options, and it expands the capabilities of your app, allowing for features like in-app collaboration and syncing across multiple devices.

## Getting Graded

> After completing Option 1 or Option 2, remember to submit your code to the `assignment5` branch!

### Option 1 - Android APK

Create a new APK for this assignment by running the `flutter clean` command, and then running the `flutter build apk` command. For more detailed instructions on creating and locating an APK, refer back to the instructions in [Assignment 1](https://github.com/shelleywong/CINS467-Course-Materials/blob/main/Assignments/Assignment1.md#getting-graded).

When you have your APK, move it to the root directory of your GIT repo that you were given to turn in assignments for this class. You must only have **one** APK in your root directory (remember, each assignment should be submitted to a unique branch, so you can overwrite any previous APKs). Do not use Android Studio or VSCode to manage your VCS/Repo as it may screw up the repo. So for this assignment you should have a directory that looks like the following:

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

### (Alternatively) Option 2 - Web URL

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

### Now submit your code to the **assignment5** branch on GitLab:

```bash
git checkout -b assignment5  #create branch and switch to it
git add -A  #add all
git commit -m "Assignment 5 Submission"  #Commit changes to branch
git push origin assignment5  #Push code up to assignment5 branch on remote
```

Make sure your branch is exactly named `assignment5` matching the case, spacing, etc as my grading script will only pull your submission if it matches exactly.

If you plan on making multiple updates to the code on this branch, you can include the `--set-upstream` option when you push the code (i.e. `git push --set-upstream origin assignment5`) -- this adds an upstream (tracking) reference so that, any time you push or pull from this branch in the future, you can simply use `git push` or `git pull`, without specifying the remote and branch.

If you would like to merge your `assignment5` branch with your `main` branch, you can run the following commands:
```bash
git checkout main  #switch to the main branch
git merge assignment5  #join the development history from the assignment5 branch with the current (main) branch
git push origin main  #push the assignment5 history up to the main branch on the remote
```

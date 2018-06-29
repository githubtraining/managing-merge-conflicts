## Step 3: Resolve a simple conflict

You may merge a lot of pull requests before you encounter your first merge conflict. That’s because Git is really smart when it comes to merging. Unless you're paying close attention to other branches in your repository, you usually won't know you have a conflict until you create the pull request.

This branch is a great example. In this scenario, two of our friends have been working in this repository. They both created branches, made changes to the `_config.yml` file, and opened pull requests. One pull request was merged to `master` without problems, but now the other pull request shows a conflict.

The history of `master` and this branch look something like this:

![deviated branches](https://user-images.githubusercontent.com/13326548/36703493-b8f4d5ee-1b10-11e8-9f95-4ec9993fe704.png)

However, because this pull request changes the same lines in the `_config.yml` file, there is a merge conflict. 

Let's help our friends resolve this conflict.

### :keyboard: Activity: Resolving your first merge conflict

1. At the bottom of the page in the "This branch has conflicts that must be resolved" section of the Pull Request, click the **Resolve conflicts** button
1. Look for the highlighted sections that begins with  `<<<<<<<  update-config` and ends with `>>>>>>> master`. These markers are added by Git to show you the content that is in conflict
1. Remove the changes made on the master branch by deleting all of the content below the `=======` and above `>>>>>>> master`
1. Next, remove the merge conflict markers by deleting the following lines:

       <<<<<<< update-config
       =======
       >>>>>>> master

1. **Optional:** If you'd like, you can edit the `_config.yml` file with your own information. Change any of the lines within the file, even outside of where the markers were. More about this below
1. With the merge conflict markers removed, click **Mark as resolved**
1. Finally, click **Commit merge**

> Sometimes, the best way to resolve a merge conflict is to add content that's different from both branches, or even to combine all of the changes from both branches. This is why Git needs a human to look at the code and make the proper fixes.

<hr>
<h3 align="center">Watch below for my response</h3>

## Welcome to Managing Merge Conflicts :tada:

Hello, and welcome! If you're here to learn about and practice resolving merge conflicts, you're in the right place.

In this course, you'll learn why merge conflicts happen and solve a few of them. The merge conflicts in this course are simple enough to solve from GitHub.com. But, if you'd prefer, you can solve them using the command line or other local tools.

As an added bonus, the project we are using for this course is a resume hosted on [GitHub Pages](https://pages.github.com/)! So, if you want to keep working after you complete this course, please feel free!

Before starting this course, we recommend completing the [Introduction to GitHub Learning Lab](https://lab.github.com/githubtraining/introduction-to-github) first. 

> Note: You may notice that some branches and pull requests already exist. We'll be using them in later activities in this course.

### How merge conflicts happen

A **Merge conflict** occurs when changes are made to the same part of the same file on two different branches. You usually find out about conflicts in a pull request. 

This can be intimidating, but have no fear, Git knows how to handle this! It only needs a human to decide how to resolve the conflict.

## Step 1: Resolve a simple conflict

You may merge a lot of pull requests before you encounter your first merge conflict. That’s because Git is smart when it comes to merging. Unless you're paying close attention to other branches, you won't know about conflicts until you create a pull request.

This branch is a great example. In this scenario, two of our friends have been working in this repository. They both created branches, made changes to the `_config.yml` file, and opened pull requests. One pull request was merged to `master` without problems, but now the other pull request has a conflict.

The history of `master` and this branch look something like this:

![deviated branches](https://user-images.githubusercontent.com/13326548/36703493-b8f4d5ee-1b10-11e8-9f95-4ec9993fe704.png)

Because this pull request changes the same lines in the `_config.yml` file, there is a merge conflict. 

Let's help our friends resolve this conflict.

### :keyboard: Activity: Resolving your first merge conflict

{% if preferences.gitTool == 'cli' %}

1. Open your preferred command line interface, which we'll call your shell from now on.
1. Clone this repository:
      ```shell
     git clone {{ thePayload.repository.clone_url }}
      ```
1. Navigate to the repository in your shell:
      ```shell
      cd {{ thePayload.repository.name }}
      ```
1. Checkout to the `update-config` branch and ensure it is up to date:
    ```shell
    git checkout update-config
    git pull
    ```
1. Merge the `master` branch into the `update-config` branch. To ensure that you're working with an up to date copy of `master`, we'll use its remote tracking branch:
    ```shell
    git merge origin/master
    ```
1. In Git's response, you'll see the file with the conflict. Open it in your text editor.
1. Look for the marked hunks that begin with  `<<<<<<<  update-config` and ends with `>>>>>>> master`. These markers are added by Git to show you the content that is in conflict.
1. Remove the changes made on the master branch by deleting all of the content below the `=======` and above `>>>>>>> master`.
1. Next, remove the merge conflict markers by deleting the following lines:

       <<<<<<< update-config
       =======
        >>>>>>> master

1. Save and close the file. Stage and commit your changes:
    ```shell
    git add .
    git commit -m "merge master into update-config"
    ```
1. Push your merged branches to GitHub:
    ```shell
    git push
    ```

{% elsif preferences.gitTool == 'desktop' %}

1. First, make sure you have [GitHub Desktop](https://desktop.github.com/) installed and [configured](https://help.github.com/en/desktop/getting-started-with-github-desktop/authenticating-to-github). 
1. On the `code` tab of this repository, click the green **Clone or download** button. Click **Open in Desktop**. 
1. In GitHub Desktop, confirm the blue **Clone** button in the pop up window. 
1. Checkout to the `update-config` branch by clicking **Current branch**, and selecting `update-config`. 
1. Merge `master` into the `update-config` branch by clicking **Current branch**, and selecting **Choose a branch to merge into update-config**. 
1. Select the `master` branch, and click **Merge master into update-config**.
1. You'll be prompted about the merge conflict, and asked if you'd like to resolve it in your default editor. Click the button to open the file in your default editor. 
1. Look for the marked hunks that begin with  `<<<<<<<  update-config` and ends with `>>>>>>> master`. These markers are added by Git to show you the content that is in conflict.
1. Remove the changes made on the master branch by deleting all of the content below the `=======` and above `>>>>>>> master`.
1. Next, remove the merge conflict markers by deleting the following lines:

       <<<<<<< update-config
       =======
        >>>>>> master

1. Save and close the file.
1. Back in GitHub Desktop, click **Commit merge**.
1. Push your changes back to the remote by clicking **Push origin**.

{% else %}

1. At the bottom of the page in the "This branch has conflicts that must be resolved" section of the Pull Request, click the **Resolve conflicts** button.
2. Look for the highlighted sections that begins with  `<<<<<<<  update-config` and ends with `>>>>>>> master`. These markers are added by Git to show you the content that is in conflict.
3. Remove the changes made on the master branch by deleting all of the content below the `=======` and above `>>>>>>> master`.
4. Next, remove the merge conflict markers by deleting the following lines:

       <<<<<<< update-config
       =======
        >>>>>>> master

5. With the merge conflict markers removed, click **Mark as resolved**.
6. Finally, click **Commit merge**.

{% endif %}

> Sometimes, the best way to resolve a merge conflict is to add content that's from both branches, or even something that isn't on either! This is why Git needs a human to look at the code and make the proper fixes.

<hr>
<h3 align="center">Watch below for my response.</h3>


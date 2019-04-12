## Step 3: Resolve more complex conflicts

Just like your first conflict, this pull request is already conflicted.

This time, however, I've made it a bit more complicated.

- Instead of one conflict, you get three!
- Instead of conflicts in one file only, you get two!  
- One of your files actually has some leftover merge conflict markers. This can happen if someone forgets to remove the markers while resolving a conflict.

### :keyboard: Activity: Resolve these conflicts

{% if preferences.gitTool == 'cli' %}
1. Checkout to the `add-experience` branch and ensure it is up to date:
    ```shell
    git checkout add-experience
    git pull
    ```
1. Merge the `master` branch into the `add-experience` branch. To ensure that you're working with an up to date copy of `master`, we'll use its remote tracking branch:
    ```shell
    git merge origin/master
    ```
1. In Git's response, you'll see two files with conflicts: `_data/experience.yml` and `_data/interests.yml`.
1. Open `_data/experience.yml` in your text editor.
1. Remove the conflict markers and pick your desired content. 
1. With the merge conflicts resolved and the markers removed in the `_data/experience.yml` file, stage the file:
    ```shell
    git add _data/experience.yml
    ```
1. Open the next file in your text editor: `_data/interests.yml`.
1. Remove the conflict markers and pick your desired content. 
1.  Close the file. Stage it and commit your changes:
    ```shell
    git add _data/interests.yml
    git commit -m "merge master into add-experience"
    ```
11. Push your merged branches to GitHub:
    ```shell
    git push
    ```
{% elsif preferences.gitTool == 'desktop' %}
1. Checkout to the `add-experience` branch by clicking **Current branch**, and selecting `add-experience`. 
1. Merge `master` into the `add-experience` branch by clicking **Current branch**, and selecting **Choose a branch to merge into update-config**. 
1. Select the `master` branch, and click **Merge master into update-config**.
1. You'll be prompted about the merge conflict, and asked if you'd like to resolve it in your default editor. Click the button to open each file in your default editor. 
1. Remove the conflict markers and pick your desired content for each file. 
1. Save and close the files.
1. Back in GitHub Desktop, click **Commit merge**.
1. Push your changes back to the remote by clicking **Push origin**.
{% else %}
1. Click **Resolve conflicts**.
1. On the left, you will notice two files listed: `_data/experience.yml` and `_data/interests.yml`. Let's start with `_data/experience.yml`.
1. Remove the conflict markers and pick your desired content. 
1. With the merge conflicts resolved and the markers removed in the `_data/experience.yml` file, click **Mark as resolved**.
1. GitHub will present the next file with conflicts, `_data/interests.yml`.
1. Remove the conflict markers and pick your desired content. 
1. When you are finished, click **Mark as resolved**.
1. Click **Commit merge**.
{% endif %}
<hr>
<h3 align="center">Watch below for my response.</h3>


## Step 9: Resolve conflicts in the Advanced Conflicts pull request

Just like your first conflict, this pull request is already conflicted.

This time, however, I've made it a bit more complicated.

- Instead of one conflict, you get three!
- Instead of conflicts in one file only, you get two!  
- One of your files actually has some leftover merge conflict markers. This can happen if your colleagues resolve merge conflicts locally and forget to remove the markers.

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
1. Open `experience.yml` in your text editor.
1. Notice there are two distinct sets of conflict markers. This is because multiple sections of the file were modified on both branches, so Git identified the two changes within the file as two separate conflicts. Remove the conflict markers and pick your desired content. 
1. **Optional:** Again, if you're trying to use this course to build a resume, you can resolve the conflicting files with your own information
1. With the merge conflicts resolved and the markers removed in the `experience.yml` file, stage the file:
    ```shell
    git add _data/experience.yml
    ```
1. Open the next file in your text editor: `_data/interests.yml`
1. This file has some extra merge commit markers. Simply select the Interests you would like to list and remove the others (and all those extra conflict markers).
1. Close the file. Stage it and commit your changes:
    ```shell
    git add .
    git commit -m "merge master into add-experience"
    ```
1. Push your merged branches to GitHub:
    ```shell
    git push
    ```
{% else %}
1. Click **Resolve conflicts**
1. On the left, you will notice two files listed: `_data/experience.yml` and `_data/interests.yml`. Let's start with `experience.yml`
1. Notice there are two distinct sets of conflict markers. This is because multiple sections of the file were modified on both branches, so Git identified the two changes within the file as two separate conflicts
1. **Optional:** Again, if you're trying to use this course to build a resume, you can resolve the conflicting files with your own information
1. With the merge conflicts resolved and the markers removed in the `experience.yml` file, click **Mark as resolved**
1. GitHub will present the next file with conflicts, `interests.yml`
1. This file has some extra merge commit markers. Simply select the Interests you would like to list and remove the others (and all those extra conflict markers)
1. When you are finished, click **Mark as resolved**
1. Click **Commit merge**
{% endif %}
<hr>
<h3 align="center">Watch below for my response</h3>

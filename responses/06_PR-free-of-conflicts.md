## Step 7: Merge the  pull request

Great job, @{{ user.username }}, your pull request is free of conflicts. :tada: Go ahead and merge this pull request now. 
 
### :keyboard: Activity: Merge this pull request


1. Click **Merge pull request** below.
2. Click **Confirm Merge**.
3. Click **Delete branch**.

{% if preferences.gitTool == 'cli' %}
You can also merge locally:
1. Checkout to the master branch:
    ```shell
    git checkout master
    ```
1. Ensure the master branch is up to date:
    ```shell
    git pull
    ```
1. Merge the `{{ branch }}` branch:
    ```shell
    git merge {{ branch }}
    ```
1. Enter a commit message, if asked.
1. Push your merged branches up to GitHub:
    ```shell
    git push
    ```
{% elsif preferences.gitTool == 'desktop' %}
You can also merge locally:
1. Checkout to the `master` branch.
2. Ensure the branch is up to date by clicking **Fetch origin**. 
3. Merge `{{ branch}} ` into the `master` branch by clicking **Current branch**, and selecting **Choose a branch to merge into master**. 
4. Select the `{{ branch }}` branch, and click **Merge {{ branch }} into master**.
5. Push your changes back to the remote by clicking **Push origin**.
{% endif %}

<hr>
<h3 align="center">Watch below for my response.</h3>


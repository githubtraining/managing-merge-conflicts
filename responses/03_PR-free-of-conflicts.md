## Step 4: Merge pull request

Great job, @{{ user.username }}, your pull request is free of conflicts. :tada:

### :keyboard: Activity: Merge this pull request

Go ahead and merge this pull request now.

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
1. Checkout to the `master` branch by clicking **Current branch**, and selecting `master`.
1. Ensure the branch is up to date by clicking **Fetch origin**. 
2. Merge `{{ branch}} ` into the `master` branch by clicking **Current branch**, and selecting **Choose a branch to merge into master**. 
3. Select the `{{ branch }}` branch, and click **Merge {{ branch }} into master**.
4. Push your changes back to the remote by clicking **Push origin**.
{% endif %}

<hr>
<h3 align="center">Watch below for my response.</h3>

## Step 8: Merge the third pull request

Great job, @{{ user.username }}, your pull request is free of conflicts. :tada:

### :keyboard: Activity: Merge this pull request

Go ahead and merge this pull request now.

1. Click **Merge pull request** below
1. Click **Confirm Merge**
1. Click **Delete branch**

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
{% endif %}

<hr>
<h3 align="center">Watch below for my response</h3>

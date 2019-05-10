You did it, @{{ user.username }}! Nice job resolving the conflict. Most conflicts in your day to day experience should be pretty simple, as in that activity. You may need to discuss the resolution with your peers. If your team is working together and reviewing pull requests, resolving conflicts is easy.

### What just happened?

Resolving a conflict doesn't automatically merge the Pull Request in GitHub. Instead, it stores the resolution of the conflict in a merge commit and allows you and your team to keep working.

To resolve a conflict, GitHub performs what is known as a *reverse merge*. This means that the changes from the `master` branch were  merged into your `update-config` branch. 

With a reverse merge, only the `update-config` branch is updated. This allows you to test the resolved code on your branch before you merge it into `master`. The `master` branch should be treated as production ready, bug-free code.

## Step 2: Merge the first resolved pull request

Go ahead and merge this pull request now.

> I have already approved this pull request, so if you still see "Review required" in the merge view, try refreshing the page.
> 
### :keyboard: Activity: Merge this pull request

1. Click **Merge pull request** below.
1. Click **Confirm merge**.
1. Click **Delete branch** and get ready for your next activity.

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


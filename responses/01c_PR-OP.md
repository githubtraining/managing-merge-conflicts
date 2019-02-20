## Step 2: Merge the pull request

Great work, @{{ user.username }}! You've created your first pull request successfully, and so far, there are no conflicts.

... but what actually is a pull request?  

A pull request is a proposal to **merge** your changes with the code on the base branch, usually `master`.

Back to our visualization. When you opened your pull request, your Git <sup>[:book:](https://help.github.com/articles/github-glossary/#git)</sup> history looked like this:

![branch with commits image again](https://user-images.githubusercontent.com/13326548/36703461-95bd5466-1b10-11e8-98d0-e2c43aa3f925.png)

Your pull request simply indicates that you want to apply the history of your branch (in this case `{{ branch }}`), into the `master` branch.

That merge _might_ look something like this:

![simple merge with master](https://user-images.githubusercontent.com/13326548/36703466-a09e583a-1b10-11e8-9208-cb536a97afd0.png)

### :keyboard: Activity: Merge the pull request

> _Protip:_ I have already approved this pull request, so if you still see "Review required" in the merge view, try refreshing the page.

1. Click **Merge pull request** below
1. Click **Confirm merge**
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
1. Merge the `change-skills` branch:
    ```shell
    git merge change-skills
    ```
1. Enter a commit message, if asked.
1. Push your merged branches up to GitHub:
    ```shell
    git push
    ```
{% endif %}
<hr>
<h3 align="center">Watch below for my response</h3>

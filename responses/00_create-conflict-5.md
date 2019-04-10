## Step 5: Create your own conflict

So far, this pull request doesn't have any conflicts, but I have added some new branch protections to prevent you from merging before you're ready.

In the last activity, you solved a merge conflict that someone else created. This time, you'll create the merge conflict yourself.

### :keyboard: Activity: Make changes on this branch

{% if preferences.gitTool == 'cli' %}
1. Check out to this branch:
    ```shell
    git checkout add-education
    ```
1. Open `_data/education.yml` in your text editor.
1. Modify the content in the `degree:`, `uni:`, `year:`, and `summary:` lines
1. Stage and commit the changes:
    ```shell
    git add _data/education.yml
    git commit -m "<YOUR-MESSAGE>"
    ```
1. Push your changes to GitHub:
    ```shell
    git push
    ```
{% else %}
1. Click on the **Files changed** tab in this pull request
1. Click the :pencil2: found in the top right-hand corner of the `_data/education.yml` file that had been previously modified
1. Modify the content in the `degree:`, `uni:`, `year:`, and `summary:` lines
1. Scroll to the bottom of the page and enter a commit message for your change
1. Click the **Commit changes** button, making sure the "Commit directly to the **add-education** branch" option is selected
{% endif %}
<hr>
<h3 align="center">Watch below for my response</h3>

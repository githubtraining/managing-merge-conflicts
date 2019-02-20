Uh oh, it would appear that in your excitement to complete this activity you accidentally created a merge conflict outside of the class activity. I'm just going to consider this an opportunity for you to have some extra practice handling merge conflicts :grinning:. 

To resolve this merge conflict, I'm going to reference the following example:

```
<<<<<<< HEAD or current branch name with the changes you recently made
I am the newer change 
==========
I was a new change until someone made a newer change
>>>>>>> Master or another branch name with an existing change
```

### :keyboard: Activity: Remove an unexpected merge conflict

{% if preferences.gitTool == 'cli' %}
Even though you're working on the command line, you may find it easier to use GitHub's web interface to troubleshoot your conflict:
{% endif %}

1. Scroll down and click the **Resolve conflict** button.
   
      - If the **Resolve conflict** button is greyed out, that means your merge conflict is too advanced for the GitHub.com UI to handle. The UI will provide instructions on how to handle the merge conflict on your locally, however, if you are uncomfortable resolving the merge conflict locally, you can always close this Pull Request and re-start the activity on a new branch. 

1. The file or files that have a conflict are displayed on the left side of the Resolve Conflicts screen. After you select a file, it will be displayed in the pane on the right side. 
1. In the file you selected, there should be a block of content that looks similar to the example merge conflict I shared above :point-up:.
1. To resolve the merge conflict, remove the branch identifiers: `<<<<<<< HEAD`, `=======`, and `>>>>>>> Master` as examples. 
1. Determine which change you do not want to keep, `I am the newer change` and `I was a new change until someone made a newer change` as example and remove the content from the file.

     - Merge conflicts can contain multiple lines of content, so you may need to remove multiple lines to resolve the merge conflict.

1. Once you have resolved all of the merge conflicts in the file, click the **Resolve conflicts** button. If you have other files with a merge conflict, repeat the above steps for each of the files with a merge conflict.
1. With all of your merge conflicts resolved, click the **Merge commit** button. 

{% if preferences.gitTool == 'cli' %}
To try and resolve the conflict locally:
1. Checkout to this branch:
      ```shell
      git checkout {{ branch }}
      ```
1. Merge in the `master` branch:
      ```shell
      git merge master
      ```
1. Look in Git's response for the files with a conflict.
1. Open each file, remove the conflict markers, and choose the content you'd like to keep.
1. Stage and commit your files:
      ```shell
      git add .
      git commit -m "merge master into {{ branch }}"
      ```
1. Push your changes to GitHub:
      ```shell
      git push
      ```
1. With all of your merge conflicts resolved, click the **Merge commit** button. 
{% endif %}

If you would like assistance troubleshooting the issue you are encountering, create a post on the [GitHub Community]({{ communityBoard }}) board. You might also want to search for your issue to see if other people have resolved it in the past.

## Step 5b: Merging similar changes

Good job! Remember from the last issue that your history now looks something like this, without conflicts:

![branch commits](https://user-images.githubusercontent.com/13326548/36703529-e1458976-1b10-11e8-97cb-ae4c2361bd20.png)

However, in a real world scenario, it's possible that a peer or colleague will have edited the same file in the same place as your pull request.

To demonstrate, I'll stand in as your colleague :wave:. In Pull Request {{ secondPR }}, you'll see that the education file has been changed. The other pull request was just merged to `master`, which means there's now a conflict in your pull request.

## Step 6: Resolve new conflicts you created

Good job! By making commits on two branches, you've created a history just like you saw in your previous conflict.

![deviated branches](https://user-images.githubusercontent.com/13326548/36703541-ef3c48f8-1b10-11e8-899f-bbaaf5927d24.png)

Typically, this happens when someone else merges a branch into `master` that has commits in the same files you've been working on.

### :keyboard: Activity: Resolve the conflict

{% if preferences.gitTool == 'cli' %}
1. Resolve the conflicts locally by checking out to this branch and repeating your previous steps.
{% else %}
1. In the "This branch has conflicts that must be resolved" section of the pull request, click **Resolve conflicts**.
{% endif %}

Because you created both conflicts, feel free to resolve these conflicts as you wish.

<hr>
<h3 align="center">Return to this pull request for next steps</h3>

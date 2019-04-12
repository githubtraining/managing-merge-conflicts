## Where do conflicts come from?

In a real world scenario, it's possible that a peer or colleague will have edited the same file in the same place as your pull request.

To demonstrate, I'll stand in as your colleague :wave:. In this other pull request {{ secondPR }}, you'll see that the education file has been changed. The other pull request was just merged to `master`, which means there's now a conflict in your pull request.

## Step 6: Resolve new conflicts

### :keyboard: Activity: Resolve the conflict

{% if preferences.gitTool == 'cli' %}
1. Make sure master is up to date by checking out to `master`, and typing `git pull`. 
1. Resolve the conflicts locally by checking out to the `add-education` branch, merging `master`, and repeating your previous steps.
{% elsif preferences.gitTool == 'desktop' %}
1. Get any new changes by clicking **Fetch origin**.
1. Resolve the conflicts locally by checking out to the `add-education` branch, merging `master`, and repeating your previous steps.
{% else %}
1. In the "This branch has conflicts that must be resolved" section of the pull request, click **Resolve conflicts**.
{% endif %}

Because you created the conflict, feel free to resolve this conflict as you wish.

<hr>
<h3 align="center">Return to this pull request for next steps.</h3>

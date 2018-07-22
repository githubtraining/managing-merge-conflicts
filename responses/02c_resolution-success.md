## Step 4: Merge the first resolved pull request

You did it, @{{ user.username }}! Nice job resolving that conflict. Most conflicts in your day to day experience should be pretty simple, as in that activity. You may need to discuss the resolution with your peers, but if your team is regularly working together and reviewing pull requests, resolving conflicts is easy.

### What just happened?

Resolving a conflict doesn't automatically merge the Pull Request in GitHub. Instead, it stores the resolution of the conflict in a merge commit and allows you and your team to keep working.

To resolve a conflict, GitHub performs what is known as a *reverse merge*. This means that the changes from the `master` branch were successfully merged into your `update-config` branch. If you merged your branch in to `master`, it would look like this:

![merge after conflict](https://user-images.githubusercontent.com/13326548/36703509-c8bab1ec-1b10-11e8-80ac-5398e066a18d.png)

But with a reverse merge, only the `update-config` branch is updated:

![reverse merge after conflict](https://user-images.githubusercontent.com/13326548/36703516-d31730ac-1b10-11e8-8e4d-0fa17baead36.png)

This allows you to test the resolved code on your branch before you merge it into `master`. The `master` branch should be treated as production ready, bug-free code.

### :keyboard: Activity: Merge this pull request

Go ahead and merge this pull request now.

> I have already approved this pull request, so if you still see "Review required" in the merge view, try refreshing the page.

1. Click **Merge pull request** below
1. Click **Confirm merge**
1. Click **Delete branch** and get ready for your next activity

<hr>
<h3 align="center">Watch below for my response</h3>

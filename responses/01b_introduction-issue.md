## Welcome to Managing Merge Conflicts :tada:

Hello, and welcome! If you're here to learn about and practice resolving merge conflicts, you're in the right place.

In this course, you'll learn why merge conflits happen by solving **four merge conflicts**. All of the merge conflicts in this course will be simple enough to solve from within the GitHub.com user interface, but if you'd prefer, you can solve them using the command line or other local tools.

As an added bonus, the project we are using for this course is a resume hosted on [GitHub Pages](https://pages.github.com/)! So, if you want to keep working after you complete this course, please feel free!

> Note: You may notice that some branches and pull requests already exist. We'll be using them in later activities in this course.

### How merge conflicts happen

*Version control* lets you make incremental changes to your code or file base while keeping the history. Git operates as a linked list, so a small history of three commits <sup>[:book:](https://help.github.com/articles/github-glossary/#commit)</sup> might look like this:

![three commits in a linked list format](https://user-images.githubusercontent.com/13326548/36703370-32b56354-1b10-11e8-881f-f356838111d4.png)

In the **GitHub Flow**, you...
- first create a new branch <sup>[:book:](https://help.github.com/articles/github-glossary/#branch)</sup> off of the base branch, which is really just a reference point to a commit on the base branch. 

![add a branch](https://user-images.githubusercontent.com/13326548/36703385-4590b28a-1b10-11e8-90c7-a5ededee0950.png)

- Next, you add one or more commits that, for now, exist only on your branch. The other commits stay fixed to their reference point in history.

![branch with new commit](https://user-images.githubusercontent.com/13326548/36703395-52d2e364-1b10-11e8-9bba-a61d4d72e02b.png)

- Finally, you open a pull request <sup>[:book:](https://help.github.com/articles/github-glossary/#pull-request)</sup> to propose that your new commits be included in the base branch, optionally add more commits, and then merge <sup>[:book:](https://help.github.com/articles/github-glossary/#merge)</sup> and delete your branch!

A **Merge conflict** occurs when someone else made a change on the base branch in the same file and location where you proposed changes. This usually happens when someone else merges in their branch before you merge yours.

This can be intimidating, but have no fear, Git knows how to handle this! It only needs a human to decide how to resolve the conflict. 

## Step 1: Create a Pull Request

Before we get too far ahead of ourselves, let's first practice making a simple change on a branch. Visualize your actions using the flow you reviewed above.

### :keyboard: Activity: Create a normal pull request

1. On the **Code** tab, click the `_data/skills.yml` file
1. In the upper right corner of the file view, click the :pencil2: icon to open the file editor
1. In the file, add a skill or two that you're proficient in
1. Scroll to the bottom of the page and select the option to "Create a new branch for this commit and start a pull request"
1. Replace the default patch branch name with `change-skills`
1. Select **Propose file change**
1. In the "Leave a comment" field of the pull request, describe the change you made
1. Click **Create pull request**
1. :construction: Don't merge yet! :construction: Refresh the pull request to receive the next comment/instructions.

For a printable version of the steps in this course, check out the [Quick Reference Guide]({{ host }}/public/{{ course.slug }}.pdf).

<hr>
<h3 align="center">Look for my next response in your pull request</h3>

> _Sometimes I respond too fast for the page to update! If you perform an expected action and don't see a response from me, wait a few seconds and refresh the page for your next steps._

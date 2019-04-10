## Nice work

![celebrate](https://octodex.github.com/images/benevocats.jpg)

Congratulations @{{ user.username }}, you've completed this course!

### What went well

Before I say good-bye, here's a recap of all the tasks you've accomplished in your repository:

- You learned why merge conflicts happen
- You practiced a normal merge
- You resolved a simple merge conflict
- You created a merge conflict, and resolved it!
- You resolved a multi-file merge conflict

### What's next?

Here are some instructions you can use to keep working on your resumé:

<details>
  <summary>Finishing the resume</summary>
  <hr>
  
  #### Finishing the resume
  
  To modify the other sections of the resume, simply create a new branch and modify the files found in the `_data` folder.

  For example, to modify the "Projects" section, edit the `_data/projects.yml` file. After making your changes, create a new pull request and merge your changes.
  
  <hr>
</details>

<details>
  <summary>Changing the picture</summary>
  <hr>
  
  #### Changing the picture
  
  If you would like to change the image used on your resume, you need to make a few changes to the files.

  1. Create a new branch, maybe name it something like `new-avatar`.
  1. Navigate to the `images` directory and click the **Upload files** button.
  1. [Drag and drop your image](https://help.github.com/articles/adding-a-file-to-a-repository/).
  1. Commit your change by clicking **Commit changes**.
  1. On the `new-avatar` branch, open the `_layouts/resume.html` file and edit line 16. Replace `images/bob-avatar.jpg` with `images/YOURFILENAME`.
  1. Create a pull request.
  1. Merge the pull request, and delete the branch.
  
  <hr>
</details>

<details>
  <summary>Enabling GitHub Pages</summary>
  <hr>
  
  #### Enabling GitHub Pages
  
  When you are happy with your resume, you will need to publish it with GitHub Pages. This resume is ready for GitHub Pages, you just need to turn it on. Follow these steps to enable GitHub Pages when you are ready to officially publish your resume:

  1. Click on the [**Settings**](https://github.com/{{ user.username }}/{{ repo }}/settings) tab.
  1. Scroll to the "GitHub Pages" section.
  1. In the "Source" drop-down, select **master branch**.
  1. Click **Save**.
  1. :construction: Warning! :construction: Make sure you don't see any [errors after you select save](https://user-images.githubusercontent.com/13326548/36769372-bc9b43d4-1bf8-11e8-8050-2b08cf8d146b.png). If you do, your page won't build correctly and this step will be incomplete.
  
  Your GitHub Pages resumé site will be live very shortly. [Click here to check it out.]({{url}})
 
  <hr>
</details>

### Keep Learning

Want to work on resolving merge conflicts using the command line? Check out [this documentation](https://help.github.com/articles/resolving-a-merge-conflict-using-the-command-line/).

Want to keep learning? Feel free to [check out our other courses]({{ host }}/courses)?

<hr>
<h3 align="center">I won't respond to this issue, go ahead and close it when finished!</h3>

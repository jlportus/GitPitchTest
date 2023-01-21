# Markdown-to-Presentation In Just 60 Seconds con GITPITCH

Today’s post is a very short tutorial that will take you through creating a simple GitPitch presentation in 60 seconds.

At the end of this tutorial you will end up with a presentation that looks just like the presentation shown here. You can click on the image to see the sample presentation live in your browser window:
[GitPitch Presentation] — In 60 Seconds Tutorial — Click To View

Ok, so let’s get started.
Step 1. Create a Git Repository

Using an existing account on GitHub, GitLab, or Bitbucket either:

    Create a new repository on and clone it to your local disk or
    Select one of your existing repositories on and make sure it has been cloned to your local disk

The rest of this tutorial will show how by adding a markdown file to your chosen repository, https://gitpitch.com can read and automatically translate that file into an online slideshow presentation.
Step 2. Create a PITCHME.md Markdown File

Using your preferred code editor create a file called PITCHME.md in the root directory of your repository, then add and save the following Markdown content within that file:

# Flux 

An application architecture for React

---

### Flux Design

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

![Flux Explained](https://facebook.github.io/flux/img/flux-simple-f8-diagram-explained-1300w.png)

Please take note of the following:

    The PITCHME.md file name is a new convention introduced by GitPitch
    The PITCHME.md file name is case sensitive
    The PITCHME.md file content is standard GitHub Flavored Markdown
    The --- markdown fragment acts as a slide delimiter that partitions your slideshow content

For the sample markdown used in this tutorial, when GitPitch processes the sample PITCHME.md markdown content it will result in a simple presentation with just three slides.
Step 3. Push PITCHME.md to your upstream Repository in the Cloud

At this point you have simply created one new file within your chosen repository. Now you need to add this file under Git version control and then push your local changes to your upstream repository on in the cloud:

git add PITCHME.md
git commit -m "Added my first GitPitch slideshow content."
git push

At this point, the upstream version of your chosen repository in the cloud should have the new PITCHME.md file in it’s root directory.
Step 4. Done!

After you git-push, you are done! Your GitPitch slideshow presentation is now waiting for you to share or present at its public URL.

You can build the public URL for your slideshow presentation on gitpitch.com using the following structure:

https://gitpitch.com/$USER/$REPO/$BRANCH

Where the following substitutions must be made by you to reflect your specific Git account and respository details:

    $USER - must be replaced with your Git account name
    $REPO - must be replaced with the name of your chosen Git repository
    $BRANCH - must be replaced with the branch you used when adding your PITCHME.md file. If you did not specifically create a feature branch for this tutorial, then the default branch name is master.

    GitLab and Bitbucket users, see special notes here and here respectively.

For example, this tutorial is itself within a repository. And that repository includes a PITCHME.md file. So you can view the GitPitch slideshow presentation associated with this tutorial at the following URL:

https://gitpitch.com/gitpitch/in-60-seconds/master

Note how $USER has been replaced with my GitHub account name ( gitpitch ) and $REPO has been replaced with the name of my repository ( in-60-seconds ).
60 Seconds Later!

That wraps things up for this very short tutorial. I hope you followed along and enjoyed creating your own GitPitch presentation using nothing more than Markdown and some basic Git commands.

GitPitch is without doubt, the fastest way from idea to presentation!

Before I wrap up, I do have a small favor to ask. If you enjoyed this post today, please show your appreciation by clapping 👏 for this article.

Your claps help boost the article on
Medium
. And that helps others to find and read this article too.

If you have any questions or feedback you can reach me in the comments sections below, on Twitter or by email. More details on the website.

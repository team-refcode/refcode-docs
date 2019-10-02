---
layout: default
title: Sprint 4
parent: Level 2 Course
nav_order: 5
permalink: /curriculum/level-2/04-sprint-plan
---

# Sprint 4
SASS for CSS, Github Pages, and Jekyll

## In-class Assignments
### Using Jekyll and Github Pages
In our last class we learned to build websites from scratch, this a useful skill but not always practical. It was a lot of work right? Making all of your pages look the same? Making navigation work the same on all of your pages so users don't get lost?

When we're building websites (and eventually web applications) there are a lot of little things that need to be consistent but a lot of little things can add up to a lot of work. That's why we use frameworks. Frameworks take care of all those little things (and a couple of larger things too).

#### Jekyll
The framework we'll set up today is called Jekyll. Jekyll was originally created to help build blogs but it can be applicable for many uses. What are some of those uses?

Jekyll provides a lot of benefits but we're interested in these two specifically:
* lets us create pages in markdown which Jekyll compiles into HTML
* lets us easily create pages that look and behave consistently

#### Installing Jekyll and Dependencies

Sounds great! How do we get started? We have to install a lot of stuff! Follow these steps:
1. [Install Command Line Tools](https://jekyllrb.com/docs/installation/macos/#install-command-line-tools)
2. [Install Ruby Using Homebrew](https://jekyllrb.com/docs/installation/macos/#brew)
3. [Install Jekyll Locally](https://jekyllrb.com/docs/installation/macos/#local-install)

#### Creating Your New Blog, Generating HTML from Markdown and Serving Your New Blog
1. Create your blog by running this command in the terminal:
`jekyll new myblog`
2. Change into your new directory:
`cd myblog`
Open your editor and look around, what do you see?
3. Run the command that builds html files from the markdown files:
`jekyll build`
Open your editor and look around again, what do you see now?
4. Run the command that serves your site:
`jekyll serve`
What does the terminal say now?
5. Take the server address that the serve command output:
[http://127.0.0.1:4000/](http://127.0.0.1:4000/)
And paste it into your web browser. What do you see? Who made this site? 
6. Press ctrl+c to stop the server

### STOP! Version Control Time
We built a lot so far, and it has been exciting. Let's keep our good habit of using version control to track changes in our projects. We're going to create a GitHub pages repo for your project.

1.  [Create a new repository](https://github.com/new)  named blog on GitHub.
2. Clone the repository to your local computer using GitHub desktop. Click the "Set up in Desktop" button. When the GitHub desktop app opens, save the project.
3. Using GitHub Desktop add your blog to this repository, commit all changes and push
4. Navigate to github.com/username/blog/settings where username is you're username. Scroll all the way down to the section *GitHub Pages.* Select the master branch from the source dropdown. 
5. Your blog should now be hosted at username.github.io/blog (it might take a few seconds)

### Customizing Your Blog
Let's customize your blog by editing the `_config.yml` file
1. Read the whole file. What do you think this file does?
2. Change the Title, Email, Description and GitHub Username
3. Run the command that builds _and_ serves your site.
`jekyll serve`
Hint: jekyll serve will build and serve your site
4. Take the server address that the serve command output:
[http://127.0.0.1:4000/](http://127.0.0.1:4000/)
And paste it into your web browser. What's different?
5. Press ctrl+c to stop the server
6. Look around in your project in GitHub Desktop. What's different?
7. Add, commit and push your changes using Github Desktop.
8. Give it a minute and check your blog at username.github.io/blog to see your changes


### Creating Your First Blog Post
1. Create a markdown file with today's date in the `_posts` directory. Your file should have this name
`2019-10-01-my-first-jekyll-post.markdown`
2. Make sure you include the front matter that indicates the layout and title of your blog:
```
---
layout: post
title:  "My First Jekyll Post"
---
```
3. Add some content using markdown
4. Run the command that builds _and_ serves your site.
`jekyll serve`
5. Take the server address that the serve command output:
[http://127.0.0.1:4000/](http://127.0.0.1:4000/)
And paste it into your web browser.  What's different?
6. Press ctrl+c to stop the server
7. Add, commit and push your changes using Github Desktop.
8. Give it a minute and check your blog at username.github.io/blog to see your changes







## At-home Assignments
Up to now, we've been using Github Desktop to manage our project repositories on Github, but we haven't dug into how git as a version control program works. Next session will will go into details about commits, best practices, how to contribute to other repositories via PRs, and how to give valuable comments. Being able to give useful and concise comments on a PR is a really good skill to have when looking for a job, and, just like everything else, it takes time and practice to master.

The at-home assignments this time are to help prepare for next week discussion and get you familiarized with git and Github:
### Watch these videos
1. [Git It? How to use Git and Github](https://www.youtube.com/watch?v=HkdAHXoRtos)

### Assignments
1. Create another blog post on your jekyll blog using the in-class instructions "Creating Your First Blog Post." Make sure you give your file a name with the YEAR-MONTH-DAY-title.markdown format.

---
<< [Back to curriculum overview](../level-2)

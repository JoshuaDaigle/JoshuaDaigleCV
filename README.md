# Write and host a resume using Markdown, GitHub Pages, and Jekyll.

Purpose
--
This readme is for you to learn the software stack required to write your own resume and host it online while following Etters guidelines
for modern technical writing. To accomplish this, we will be writing your resume in markdown, generating a static website from your resume 
using Jekyll and hosting it online using GitHub Pages. 

# Prerequisites 
1. A GitHub account 
2. Ruby
3. RubyGems
4. A text editor that supports Markdown, specifically GitHub flavoured markdown

# Instructions

## Writing your resume

Etter stresses the importance of writing a technical document using a lightweight, human readable markup language. This is because it makes it
simple to maintain, publish, and collaborate with others. For these reasons we will be writing our resume in Markdown, the most popular lightweight markup
language in the world. This readme will not go into detail about how to use Markdown, but here are some resources to help you learn:
* https://www.markdownguide.org/
* https://github.github.com/gfm/

## Creating your website

We will be generating a static website from your resume. Etter recommends the using static websites because of their speed, simplicity, and security. 
The tool we will be using to make the static website is Jekyll, a popular static website generator. Making your own static website from this repository will involve 6 main steps:
1. Forking this repository to your GitHub account.
2. Cloning this repository to your local machine.
3. Making changes to the repository.
4. Generating the static website with Jekyll.
5. Updating your repository with your changes.
6. Hosting the static website with GitHub Pages.

## 1. Forking this repository
Forking lets you create a copy of a repository that you can manage on your own GitHub page.

To fork this repository: 

1. Click the `Fork` button on the top right side of the repository.
2. Click the green `Create fork` and the bottom of the page that you were re-directed to. 

You should now be re-directed to your new forked repository. 

## 2. Cloning this repository
Cloning a repository downloads it to your local machine and initializes a local git repository. You will now clone the fork you created. 

To clone your forked repository:

1. Open the terminal in the folder you wish to clone the repository into.
2. Type `git clone <URL_OF_FORKED_REPOSITORY>` into the terminal.

You should now see the contents of the repository inside of the folder you cloned into. 
These files include: 
* A folder named `_layouts`.
* A file named `_config.yaml`.
* A file named `.gitignore`.
* A file named `index.md`.
* A file named `README.md`.

## 3. Making changes to the repository

In the index.md file, you will see 2 things:
* A YAML front matter block at the top of the page.
* My Markdown formatted resume. 

The YAML front matter block at the top defines two variables:

* The `title` variable specifies the title of the page.

* The `layout` variable tells Jekyll which layout to use for the page; its what is going to add the styling for the resume. You can see the layout
being referenced in the `_layouts` folder.

On this page, make the following changes:
1. Edit the `title` variable to whatever you wish.
2. Replace my resume with your own Markdown formatted resume.

Additionally, in the `config.yaml` file, change the title variable to your desired website name. 

## 4. Generating the static website with Jekyll

First, Jekyll must be installed on your computer.

To install Jekyll we will be using the Ruby Package manager RubyGems. RubyGems is a command line tool for downloading Ruby programs, like Jekyll. 

Assuming you already have Ruby and RubyGems properly installed:

1. Open your terminal.
2. Type `gem install jekyll bundler`.

Once Jekyll has been installed: 
1. Navigate to your cloned repository in the terminal.
2. Type `jekyll build` to generate the static website.
   * This will create two new files: `_site` and `.jekyll-cache`. You don't have to worry about them.
3. Type `jekyll serve` to run your website locally. 
4. Go to `http://localhost:4000/` to view your website.

If you followed these steps and see your resume properly formatted when visiting the URL, move onto the next step. 

## 5. Updating the repository with your changes
Once you are happy with your local changes, it's time to push you changes back to your repository on GitHub. 

To push your changes to GitHub:
1. Open the terminal in your cloned local directory.
2. Type `git add .` to stage your changes.
3. Type `git commit -m"<A_COMMIT_MESSAGE>"` to commit your changes.   
4. Type `git push` to push your changes to your GitHub repository.

If you followed these steps successfully you should see your changes on your GitHub repository. 

## 6. Hosting the static website with GitHub Pages
Once your changes have been successfully pushed to your repository, it's finally time to host your resume. 

To host your resume on GitHub Pages:
1. Navigate to your forked GitHub repository.
2. Click the `Settings` button.
3. Click the `Pages` option under the `Code and automation` section
4. Select `main` from the `Branch` dropdown
5. Hit save. 

After a few minutes, your resume should hosted on GitHub pages.

You can see your hosted resume by visiting `https://<GITHUB_USERNAME>.github.io/<GITHUB_REPOSITORY>/`, or by clicking the link
at the top of the GitHub pages section. 

![GitHub Pages Navigation](https://user-images.githubusercontent.com/56177903/199147008-d16ae0cf-4cbc-4fc6-898b-414ad7f32f6a.gif)

# Authors and Acknowledgments: 
Joshua Daigle

Group Members

# FAQs

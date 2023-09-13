---
title:  "Week 1: Setting up the static website"
permalink: /documentation/week_1/
last_modified_at: 13-9-2023
---

This article will take you step by step through the process of building your own static website. 

To build our website we use Jekyll. Jekyll is a popular static site generator used for building and managing websites and blogs. It's an open-source tool written in Ruby and often used by developers, bloggers, and content creators. Jekyll takes plain text files, often written in Markdown or HTML, and converts them into static websites or blogs. Combined with Github Pages we can host our website for free and could even deploy it with our own custom domain name.

The process had been done on a laptop with windows 11 installed. To simplify the process we will install ubuntu via the Microsoft store using WSL (Windows Subsystem for Linux). It is a compatibility layer in the Windows operating system that allows you to run a full-fledged Linux kernel and user-space environment alongside the Windows kernel. This technology is primarily aimed at developers and users who want to use Linux tools and utilities on their Windows machines without the need for dual-booting or using a virtual machine.
Let’s get started: 

## Step 1: Create a Github account

- Create a GitHub account on [`Github`](https://github.com/signup) 

## Step 2: Create your local and remote GitHub repository

- On your home screen click on the "New repository" sign 
- Provide a name for your repository. This name will also determine the URL for your repository.
- Add a description that briefly explains the purpose or content of your repository.
- Ensure that the repository visibility is set to "Public" so that it can be accessed by anyone.
- Check the option to "Add a README file" to include an initial `README.md` file in your repository.
- For the `.gitignore` file, select "Jekyll" to automatically include a Gitignore file tailored for Jekyll projects.
- Under "License," choose the MIT License, which is a permissive open-source license.
- Finally, click the "Create repository" button to create your repository with these specified settings.

## Step 3: Enabling WSL

- In the windows search bar search `Turn Windows features on or off`
- Scroll down to "Windows Subsystem for Linux" and make sure its checked

## Step 4: Download ubuntu via the Microsoft Store 

- Open application
- Set up your Linux username and password
- Update and upgrade packages with:

```ruby
sudo apt update && sudo apt upgrade
```

- More detailed information on [`Learn.Microsoft`](https://learn.microsoft.com/nl-nl/windows/wsl/setup/environment) 

## Step 5: Install Jekyll on Ubuntu

- Install Ruby and other prerequisites:

```ruby
sudo apt-get install ruby-full build-essential zlib1g-dev
```

- Avoid installing RubyGems packages (called gems) as the root user. Instead, set up a gem installation directory for your user account. The following commands will add environment variables to your `~/.bashrc` file to configure the gem installation path:

```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

- Finally, install Jekyll and Bundler: 

```
gem install jekyll bundler
```

## Step 6: Create directory 

- To create a directory in Linux, you can use the `mkdir` command followed by the name of the directory you want to create. Here's the basic syntax: 

```
mkdir directory_name
```

for example 

```
mkdir website
```

- In file explorer search for the folder you just created. It would something like `\\wsl.localhost\Ubuntu\home\username\directory_name` Change `username` for your own username and `directory_name` with the name of the directory you just created
- Pin this directory in `Quick access`

## Step 7: Download Gitub desktop

- Link your remote repository to your local repository by going to the GitHub Desktop
- Go to file - Clone repository – select the repository that you just created and save it in the directory you pinned in Quick access.

## Step 8: Download a theme

- You can browse and discover various templates on websites like [`Jekyll Themes`](https://jekyllthemes.io/github-pages-themes) . This website offers a curated list of themes for GitHub Pages. 
- Navigate to its GitHub repository by clicking the `Get [theme] on GitHub` link provided on the theme's page.
- Look for the green "Code" button located near the top right of the repository's main page. In the dropdown menu, click on the "Download ZIP" option.
- Extract the zip file and paste them inside your local GitHub repository (the folder you just created)
- Give yourself full permision using `sudo chown -R username path` for example `sudo chown -R sven_dekker /home/sven_dekker/`

## Step 9: Download Visual Studio Code (VSC)
- Can be downloaded from the Microsoft store

Install Extensions

- In the top left corner, click on the "Extensions" icon
* In the Extensions sidebar, search for and install the following extensions:
  * `Ruby` (by Peng Lv): Install the first result that appears in the search
  * `Code Runner` (by Jun Han): Install the first result that appears in the search
  * `GitHub Pull Requests and Issues` (by GitHub.com): Install the first result that appears in the search
  * `Remote Repositories` (by Microsoft): This extension is often pre-installed

* Open Remote Github Repository in VSC:
  * To access various commands in VSC, open the Command Palette by pressing Shift + Enter + P. It will display a menu for executing commands
  * In the Command Palette, type "Open Remote Repository" and select it from the suggestions
* Open local Github repository in VSC
  * Click on "File," then select "Open Folder."
  * Choose the option to "Show Local" and locate your local GitHub repository
  * Open the local repository folder

---
When working with a new theme and navigating its files and folders, like `navigation.yml`, `_config.yml`, `_layouts`, `_pages`, and `_posts`, it's common to feel a bit lost. My advice is to start by reading the documentation thoroughly to understand the theme's concept. Additionally, you can benefit from exploring the theme's demo site. This allows you to identify elements you'd like to replicate and examine the code in the GitHub repository. These steps can significantly ease your understanding and usage of the theme.

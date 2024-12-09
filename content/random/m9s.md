+++
date = '2024-12-10T00:24:26+06:00'
draft = false
title = 'mylearnings init: How I setup hugo for my knowledge base'
tags = ["Hugo", "Tutorial", "Static Site Generator"]
categories = ["random"]
+++
## How I setup Hugo for my knowledge base

### Basic Setup
1. Follow Hugo getting started [Quick Start](https://gohugo.io/getting-started/quick-start/) to get Hugo installed and running.
2. Clone the [hugo-paper](https://github.com/nanxiaobei/hugo-paper) theme. Follow the [Quick Start](https://gohugo.io/getting-started/quick-start/) Page for reference.
3. Create a new Hugo site using the theme.
4. Modify the hugo.toml file for [hugo-paper](https://github.com/nanxiaobei/hugo-paper).  
5. Run `hugo server` to start the server.

### Creating a new post
Markdown Cheatshee: [markdown-guide](https://www.markdownguide.org/cheat-sheet/)
1. Run `hugo new post/my-post.md` to create a new post. Where `my-post.md` is the name of the post.
    - The post will be created in the `content/post` directory.
2. Edit the post file.
    - Update the content of the front matter.
    - Add content below the front matter.
3. Set the `draft` parameter to `false` to publish the post.

### Adding a menu
Reference : [hugo-menus](https://gohugo.io/content-management/menus/)
1. Add `sectionPagesMenu = 'main'` to the `hugo.toml` file.
2. Edit hugo.toml file and add the following to the `[menus]` section.
```toml
[[menus.main]]
  name = 'Home'
  pageRef = '/'
  weight = 10
[[menus.main]]
  name = 'K12e'
  pageRef = '/knowledge-base'
  weight = 20
```
- name: Display name of the menu item.
- url: URL of the menu item.
- weight: Determines the order (lower weights appear first).


### Deploy to GitHub Pages
Reference: [Host-on-Github-Pages](https://gohugo.io/hosting-and-deployment/hosting-on-github/)

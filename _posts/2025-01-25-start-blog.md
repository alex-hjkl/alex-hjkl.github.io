---
layout: post
title: "How to Start the Simplest Blog with Markdown"
date: 2025-01-25
---

# How to Start the Simplest Blog with Markdown

Do you want a very simple way to keep notes about projects?  
GitHub Pages is great for that because it has built-in support for Jekyll.  
You won't need to generate pages manually - just write Markdown files, push them to Git, and you're done.  
As simple as Kalashnikov rifle!  

Below are a few steps to get started.  

---

## Create a New Repository on GitHub
Create a new repository named `<yourUsername>.github.io`.   
This name is important.  
GitHub will automatically turn this repository into a personal site.  

---

## Enable GitHub Pages
1. Go to your repository **Settings**.  
2. Select **Pages** in the sidebar.  
3. Pick the main branch as the source.  
4. Click **Save**.  

After a minute or two, your site will be live at `https://<yourUsername>.github.io`.  

---

## Create a Simple Home Page
In the root of your repository, add a file called `index.md`:  

```markdown
---
layout: home
title: "Home"
permalink: /
---
```

---

## Create a Simple About Page
Also, create a file called `about.md`:
```markdown
---
layout: page
title: "About"
permalink: /about/
---

This is a page about me.
```

I'm gonna fill it out someday. (Ha ha)  

---

## Create a Configuration File
Jekyll reads from `_config.yml` in the root of your repository.  
Here’s a simple example:  

```yaml
title: "Alex hjkl"
author: "Alexey Yashin"
description: "Notes about some tech stuff"
theme: minima 
links:
  - title: "Home"
    url: /
  - title: "About"
    url: /about/
```
Fill in your own title, author, and description.  
This keeps your site info consistent and replaces default placeholders.  

---

## Push Everything to Git
Push `index.md`, `about.md`, and `_config.yml` to your repository.  
After a few minutes, your changes will be live on GitHub Pages.  


But what about articles? Let's move on  

---

## Create a _posts Folder for Articles 
To publish articles, add a folder named _posts in the root of your repo.  
Place Markdown files inside it.  
Use the naming format YYYY-MM-DD-post-title.md  

Example `_posts/2025-01-25-start-blog.md`:
```markdown
---
layout: post
title: "How to Start the Simplest Blog with Markdown"
date: 2025-01-25
---

# How to Start the Simplest Blog with Markdown

Some text here...
```

Each time you push a new file to _posts, Jekyll generates a new blog post.  
Remember to push your changes so they’re available on your live site.  

---

That’s it!  
You now have a functional blog on GitHub Pages using Jekyll and Markdown.  

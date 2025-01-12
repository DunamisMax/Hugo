+++
title = "Hosting a Hugo blog on Ubuntu"
date = "2024-12-18T12:00:00Z"
draft = false
+++

I recently put together a Hugo blog on an Ubuntu server and learned a lot in the process. After installing Hugo Extended via apt, I created a new site and used `hugo server -D` to preview any changes. I picked the hugo-paper theme, updated `theme = "hugo-paper"` in `hugo.toml`, and customized fonts and icons in the `static/` folder. A few template tweaks gave the blog a personal touch.

For content, I set up `_index.md` for the homepage, added posts under `content/blog/`, and created a contact page with a Formspree HTML form (requiring `unsafe = true` in Goldmark). A few hiccups popped up—like having to switch off draft settings and adjust URLs—but everything eventually came together. Once I was happy, I ran `hugo` to generate the `public/` folder, uploaded it, and configured a Caddy reverse proxy. It’s been fun experimenting with Hugo and refining each detail, and I’m excited to keep improving my site.
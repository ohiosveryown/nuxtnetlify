---
title: Second Post
date: 2020-12-27T16:38:23.223Z
description: This is the second post excerpt
---
# Blog Post Title

By adding nuxt content module you get `$content` injected into your whole app which you can use to fetch content from your content folder using `simple fetch api` or `nuxt asyncData` option. \
This also gives a `<nuxt-content>` component which helps you display markdown content with ease and also gives option of live editing in dev mode.

### Example Blog Post

To generate blog posts create a `_slug.vue` file in the pages folder. By using `$content` you would get a json which you can use to display. But if you are using `markdown` to write and store your posts you can use `<nuxt-content>`module which gives you option to edit content on page in dev mode and many more [features](https://content.nuxtjs.org/).
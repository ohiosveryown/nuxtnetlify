<template>
  <div>
    <!-- blog post page content / style -->
    <h2>{{ post.title }}</h2>
    <h6>Blog post style / content</h6>
    <nuxt-content :document="post" />
    <!-- <small>Hello</small> -->
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params, error }) {
    let post;
    try {
      post = await $content("blog", params.slug).fetch();
      // OR const article = await $content(`articles/${params.slug}`).fetch()
    } catch (e) {
      error({ message: "Blog Post not found" });
    }

    return {
      post,
    };
  },
};
</script>
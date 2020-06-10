<template>
  <section>
    <client-only><div v-html="posts" /></client-only>
  </section>
</template>
<script>
import { mapState } from "vuex";
export default {
  head() {
    return {
      title: "Trang quản trị"
    };
  },
  asyncData() {
    return {
      posts: "<p>So, before I start with the details on how I overcame the SEO problem, I would like to mention that there are some projects that did something similar and ultimately inspired me for the approach I ended up using, one such project is prerender-spa-plugin, however, in my opinion most of these projects took an approach that was much more complex to implement. What these projects did was to integrate pre-rendering engines like Puppeteer and rendred all possible routes of their static website with it and then hosted these pre-rendered pages on the web host instead of the actual single-page application.</p><p>This approach works great with SEO and reduces load times as well for your website, however you lose that fluid experience of single-page apps that I personally admire. The pre-rendered pages lose the no-refresh navigation among different pages on your sites and you lose the route-navigation animations that work so well on SPA.</p>"
    };
  }
};
</script>

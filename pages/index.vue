<template>
  <div>
    <logo />
    <h1 class="title">Nuxt.js & Netlify CMS Starter</h1>
    <h2 class="subtitle">Truly fantastic. Sometimes I astound even myself.</h2>
    <a href="https://github.com/xdesro/nuxt-netlify-cms-starter">GitHub</a>
    <a href="http://i.ncredibly.online">Twitter</a>
    <nuxt-link to="/blog">Blog</nuxt-link>
    <div class="deploy-button">
      <a
        href="https://app.netlify.com/start/deploy?repository=https://github.com/xdesro/nuxt-netlify-cms-starter"
      >
        <img src="https://www.netlify.com/img/deploy/button.svg" alt="Deploy to Netlify" />
      </a>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  head() {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }
      ]
    }
  }
}
</script>

<style scoped>
.deploy-button {
  margin-top: 1rem;
}
</style>

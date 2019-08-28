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

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
    'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: bold;
  font-size: 3.2rem;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 2rem;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
a {
  font-weight: bold;
  color: #526488;
}
.deploy-button {
  margin-top: 1rem;
}
</style>

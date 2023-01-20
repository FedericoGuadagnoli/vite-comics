<script>
import AppLogo from './components/AppLogo.vue';
import AppLink from './components/AppLink.vue';
import AppActions from './components/AppActions.vue';
import AppFooterTop from './components/AppFooterTop.vue';
import AppFooterBottom from './components/AppFooterBottom.vue';
export default {
  name: 'Vite DC Comiccs',
  components: { AppLogo, AppLink, AppActions, AppFooterTop, AppFooterBottom }


};

</script>

<template>
  <!-- Header -->
  <header>
    <div class="container">
      <div class="navbar">
        <App-Logo></App-Logo>
        <App-Link></App-Link>

      </div>
    </div>
  </header>

  <!-- Main -->
  <main>

    <!-- Section Content goes here -->
    <section id="Content-Goes-Here">
      <div class="container">
        <h1> -- Content goes here -- </h1>
      </div>
    </section>

    <!-- Section Actions -->
    <section id="actions">
      <div class="container">
        <App-Actions></App-Actions>
      </div>
    </section>
  </main>
  <footer>
    <App-FooterTop></App-FooterTop>
    <App-FooterBottom></App-FooterBottom>
  </footer>

</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>

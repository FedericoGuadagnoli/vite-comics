<script>
import AppLogo from './components/AppLogo.vue';
export default {
  name: 'Vite DC Comiccs',
  components: { AppLogo }
};

</script>

<template>
  <!-- Header -->
  <header>
    <div class="container">
      <div class="navbar">
        <App-Logo></App-Logo>

      </div>
    </div>
  </header>
  <main></main>
  <footer></footer>

</template>

<style>
/* RESET */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* GENERICS */
.container {
  width: 80%;
  margin: 0 auto;
  height: 100%;
}


/* HEADER */
header {
  height: 150px;
}

.navbar {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>

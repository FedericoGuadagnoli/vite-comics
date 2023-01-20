<script>
import AppLogo from './components/AppLogo.vue';
import AppLink from './components/AppLink.vue';
export default {
  name: 'Vite DC Comiccs',
  components: { AppLogo, AppLink }


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

a {
  text-decoration: none;
  color: black;
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

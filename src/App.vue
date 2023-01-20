<script>
import AppLogo from './components/AppLogo.vue';
import AppLink from './components/AppLink.vue';
import AppActions from './components/AppActions.vue';
export default {
  name: 'Vite DC Comiccs',
  components: { AppLogo, AppLink, AppActions }


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
    <div class="container">

    </div>
  </footer>

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

/* MAIN */
#Content-Goes-Here {
  height: 150px;
  background-color: black;
  color: white;
  line-height: 150px;
  vertical-align: middle;
  margin-top: 3px;
}

#actions {
  height: 180px;
  background-color: dodgerblue;
  color: white;
}

/* FOOTER */
footer {
  height: 600px;
}
</style>

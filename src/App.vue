<!-- **************************
SCRIPT
************************** -->
<script>
// 1. importare il componente
import AppTitle from "./components/AppTitle.vue";

export default {
  components: {
    // 2. registrare il componente che abbiamo importato
    AppTitle,
  },
  data() {
    return {
      message: "Ciao mondo sono io!",
    };
  },
  methods: {
    sayHello() {
      console.log("Ciao!");
    },
  },
};
</script>

<!-- **************************
TEMPLATE
************************** -->

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <AppTitle />
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>

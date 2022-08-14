<template>
  <div>
    <NavBar></NavBar>
    <TheConteudo></TheConteudo>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import NavBar from './components/NavBar.vue';
import TheConteudo from './components/TheConteudo.vue';



export default defineComponent({
  name: 'App',
  components: {
    NavBar,
    TheConteudo
  }
});
</script>

<style scoped>

</style>

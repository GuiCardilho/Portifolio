<template>
  <div>
    <TheHeader></TheHeader>
    <TheConteudo></TheConteudo>
    <NavBar></NavBar>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import NavBar from './components/NavBar.vue';
import TheConteudo from './components/TheConteudo.vue';
import TheHeader from './components/TheHeader.vue';



export default defineComponent({
  name: 'App',
  components: {
    NavBar,
    TheConteudo,
    TheHeader
}
});
</script>

<style scoped>

</style>

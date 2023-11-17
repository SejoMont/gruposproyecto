<template>
  <MusicaComponent/>
  <home-alumnos-vue></home-alumnos-vue>
</template>

<script>
import HomeAlumnosVue from './components/HomeAlumnos.vue'
import MusicaComponent from './components/MusicaComponent.vue'
HomeAlumnosVue

export default {
  name: 'App',
  components: {
    MusicaComponent,
    HomeAlumnosVue
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

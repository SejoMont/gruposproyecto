<template>
  <div class="container-fluid">
    <h2 class="text-center mt-5">NUMERO DE ALUMNOS: </h2>
    <div class="d-flex flex-row">
      <!-- Contenedor izquierdo (col-md-3) -->
      <div class="col-md-3 p-4" style="background-color: #3498db; color: white; border-radius: 8px;">
        <h2 class="mb-3">Contenedor Izquierdo</h2>
        <p>Este es el contenido del contenedor izquierdo.</p>
        <musica-component/>
        <button class="btn btn-info">GENERAR INFORME</button>
      </div>

      <!-- Contenedor derecho (col-md-9) -->
      <div class="col-md-9 p-4 " style="background-color: #9b59b6; color: white; border-radius: 8px;">
        <h2 class="mb-3">Contenedor Derecho</h2>
        <p>Este es el contenido del contenedor derecho. Es más grande que el izquierdo.</p>
        <div></div>
      </div>
    </div>
  </div>
</template>

<script>
import MusicaComponent from './MusicaComponent.vue'

export default {
  components: { MusicaComponent },
  name: "HomeAlumnos",
}
</script>

<style scoped>
/* Puedes agregar estilos adicionales aquí si es necesario */
</style>

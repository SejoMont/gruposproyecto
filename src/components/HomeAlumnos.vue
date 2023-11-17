<template>
  <div>
    <div class="container-fluid">
      <div class="d-flex flex-row" style="height: 100vh">
        <!-- Contenedor izquierdo (col-md-3) -->
        <div
          class="col-md-3 p-3 "
          style="background-color: #3498db; color: white; border-radius: 8px"
        >
          <h3 class="mb-2">Alumnos</h3>
          <ul class="list-group">
            <li v-for="alumno in alumnos" :key="alumno.id" class="list-group-item">
              {{ alumno.nombre }}
            </li>
          </ul>
          <musica-component />
          <button class="btn btn-info btn-sm mt-3">Generar Informe</button>
        </div>

        <!-- Contenedor derecho (col-md-9) -->
        <div
          class="col-md-9 p-4"
          style="background-color: #9b59b6; color: white; border-radius: 8px"
        >
          <h2 class="text-center mt-5">NUMERO DE ALUMNOS:</h2>
          <h2 class="mb-3">Contenedor Derecho</h2>
          <p>
            Este es el contenido del contenedor derecho. Es más grande que el
            izquierdo.
          </p>
          <div></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import MusicaComponent from "./MusicaComponent.vue";

export default {
  components: { MusicaComponent },
  name: "HomeAlumnos",
  data() {
    return {
      alumnos: [
        { id: 1, nombre: "Alumno 1" },
        { id: 2, nombre: "Alumno 2" },
        { id: 3, nombre: "Alumno 3" },
        // Agrega más alumnos según sea necesario
      ],
    };
  },
};
</script>

<style scoped>
/* Puedes agregar estilos adicionales aquí si es necesario */
</style>

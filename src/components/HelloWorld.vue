<template>
  <div class="hello">
    <div>
      <h2>Todos los Alumnos</h2>
      <ul v-for="alumno in alumnos" :key="alumno.idAlumno">
        <!-- <img :src="alumno.imagen" alt="alumno.imagen" /> -->
          <li>{{ alumno.nombre }} {{ alumno.apellidos }}</li>
      </ul>
    </div>

    <div v-if="gruposGenerados.length > 0">
      <h2>Grupos Generados</h2>
      <div v-for="(grupo, index) in gruposGenerados" :key="index">
        <h3>Grupo {{ index + 1 }}</h3>
        <ul v-for="alumno in grupo" :key="alumno.idAlumno">
          <li>{{ alumno.nombre }} {{ alumno.apellidos }}</li>
        </ul>
      </div>
    </div>

    <button @click="generarGrupos">Generar Grupos Aleatorios</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
    alumnos: Array, // Nueva propiedad para recibir el array de alumnos
  },
  data() {
    return {
      gruposGenerados: [], // Almacena los grupos generados aleatoriamente
    };
  },
  methods: {
    generarGrupos() {
      // Copia el array de alumnos y mézclalo para formar grupos aleatorios
      const alumnosAleatorios = this.shuffleArray([...this.alumnos]);

      // Divide los alumnos en grupos de 3
      this.gruposGenerados = [];
      for (let i = 0; i < alumnosAleatorios.length; i += 3) {
        this.gruposGenerados.push(alumnosAleatorios.slice(i, i + 3));
      }
    },
    shuffleArray(array) {
      // Función para mezclar aleatoriamente un array
      for (let i = array.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [array[i], array[j]] = [array[j], array[i]];
      }
      return array;
    },
  },
};
</script>

<style scoped>
/* Puedes agregar estilos específicos para tu componente aquí */
</style>

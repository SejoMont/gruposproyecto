<template>
  <div>
    <!-- Pasa el array de alumnos al componente HelloWorld -->
    <HelloWorld :alumnos="alumnos" />
    <MusicaComponent/>
  </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue"; // Ajusta la ruta según tu estructura de archivos
import MusicaComponent from './components/MusicaComponent.vue';

export default {
  components: {
    HelloWorld,
    MusicaComponent

  },
  data() {
    return {
      alumnos: [
  {
    "idAlumno": 1,
    "nombre": "Ferrán",
    "apellidos": "Aguilar",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 2,
    "nombre": "Mauricio",
    "apellidos": "Almaraz",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 3,
    "nombre": "John",
    "apellidos": "Flores",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 4,
    "nombre": "Valentin",
    "apellidos": "Gonzalez",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 5,
    "nombre": "Cristopher",
    "apellidos": "Jimenez",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 6,
    "nombre": "Ivan",
    "apellidos": "Juarez",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 7,
    "nombre": "Rafael",
    "apellidos": "Librero",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 8,
    "nombre": "Razvan",
    "apellidos": "Lucaci",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 9,
    "nombre": "Alejandro",
    "apellidos": "Lopez",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 10,
    "nombre": "Wendemu",
    "apellidos": "Lopez",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 11,
    "nombre": "Werku",
    "apellidos": "Lopez",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 12,
    "nombre": "Marcos",
    "apellidos": "Madrid",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 13,
    "nombre": "Macarena",
    "apellidos": "Mamolar",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 14,
    "nombre": "Andrea",
    "apellidos": "Martinez",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 15,
    "nombre": "Alexia",
    "apellidos": "Molina",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 16,
    "nombre": "Sergio",
    "apellidos": "Montero",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 17,
    "nombre": "Alberto",
    "apellidos": "Ojea",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 18,
    "nombre": "Ana Maria",
    "apellidos": "Ortega",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 19,
    "nombre": "Alejandro",
    "apellidos": "Parra",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 20,
    "nombre": "Ana Maria",
    "apellidos": "Pereira",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 21,
    "nombre": "Michely",
    "apellidos": "Pinto",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 22,
    "nombre": "Samuel",
    "apellidos": "Pop",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 23,
    "nombre": "Jaime",
    "apellidos": "Reparaz",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 24,
    "nombre": "Javier",
    "apellidos": "Roca",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  },
  {
    "idAlumno": 25,
    "nombre": "Jaime",
    "apellidos": "Rodriguez",
    "imagen": "https://www.kmikze.com/1821-large_default/super-friki.jpg",
    "activo": 1,
    "idCurso": 2023
  }
],
    };
  },
};
</script>
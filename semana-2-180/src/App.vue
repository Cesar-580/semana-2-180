<template>
  <div id="app">

    <!-- Inicio -->

    <top-banner></top-banner>

    <!-- Servicios -->

    <!-- <page-services></page-services> -->

    <!-- Aplicación -->

    <div class="container-fluid">
      <section-api></section-api>
    </div>

    <!-- Miembros -->
    <div class="container-fluid">
      <div class="row justify-content-center mb-5">
        <div class="col mt-5" v-for="(item, index) of team" :key="index">
          <team-card v-bind:member="item"></team-card>
        </div>
      </div>
    </div>

    <!-- footer  -->
    <page-footer></page-footer>

    <!-- <h1>{{ titulo }}</h1> -->
  </div>
</template>

<script>
import PageFooter from "./components/PageFooter.vue";
import TeamCard from "./components/TeamCard.vue";
import SectionApi from "./components/SectionApi.vue";
import TopBanner from './components/TopBanner.vue';
// import PageServices from './components/PageServices.vue';

export default {
  name: "App",
  components: {
    PageFooter,
    TeamCard,
    SectionApi,
    TopBanner,
    // PageServices,
  },
  data() {
    return {
      titulo: "Vivo dentro de Vue",
      team: [
        {
          codigo: 1,
          nombre: "José Javier Martínez Urzola",
          descripcion:
            "30 años, estudiante de la UTP, me gusta la tecnología, hacer deporte, aprender cosas nuevas.",
          rol: "Desarrollador fronted",
          imagen: require("@/assets/jjmt.jpg"),
        },
        {
          codigo: 2,
          nombre: "Henry Guillen Ramírez",
          descripcion:
            "Director operativo en Hirai Denki Industria Electrónica S.A.S. Me gusta leer sobre tecnología, escuchar Jazz suave. Soy creyente cristiano.",
          rol: "Arquitecto de software",
          imagen: require("@/assets/hmt.jpg"),
        },
        {
          codigo: 3,
          nombre: "César A. Ospina Muñoz",
          descripcion:
            "Estudiante Universidad Nacional de Colombia, 20 años, Me gusta practicar ciclo montañismo y futbol, me apasiona aprender diferentes tipos de lenguajes de programación.",
          rol: "Desarrollador de backend",
          imagen: require("@/assets/cesar.jpg"),
        },
        {
          codigo: 4,
          nombre: "Heberley Tobon",
          descripcion:
            "Mi nombre es Heberley Tobón, Me apasiona la transferencia tecnologica y el ajedrez. ",
          rol: "Tester",
          imagen: require("@/assets/heber.jpg"),
        },
        {
          codigo: 5,
          nombre: "Jairo Arteaga",
          descripcion:
            "Me gusta aprender cada dia de los lenguajes de programción, y estoy muy feliz de estar en el curso",
          rol: "Analista",
          imagen: require("@/assets/Jairo.jpg"),
        },
      ],
    };
  },
};
</script>


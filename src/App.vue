<template>
  <div id="app">
    <header-section></header-section>
    <services></services>
    <news-section></news-section>
    <section class="row justify-content-center mb-5">
      <div class="col" v-for="(item, index) of team" :key="index">
        <team-card :member="item"></team-card>
      </div>
    </section>
    
    <footer-section></footer-section>
  </div>
</template>

<script>

import FooterSection from './components/FooterSection.vue';
import TeamCard from './components/TeamCard.vue';
import Services from './components/Services.vue';
import NewsSection from './components/NewsSection';
import HeaderSection from './components/HeaderSection.vue';


export default {
  name: 'App',
  components: {
    HeaderSection,
    Services,
    NewsSection,
    TeamCard,
    FooterSection
  },
  data(){
    return{
      team: [
        {
        codigo: 1,
        nombre: 'Andrés Manuel Prieto Álvarez',
        descripcion: 'Yo soy Andrés M. Prieto; tengo 6 años de experiencia en TI, 3 años de desarrollo Frontend, 2 años de desarrollo de bases de datos relacionales, 1 año en desarrollo de arquitecturas, 1 año de metodología Scrum; soy estudiante de ingeniería en sistemas y computación de la UTP',
        rol: '(Main Frontend Developer)',
        image: 'https://avatars3.githubusercontent.com/u/39841241?s=96&v=4'
        },
        {
        codigo: 2,
        nombre: 'Carlos Sneider Soto Sogamoso',
        descripcion: 'Soy Carlos Sneider Soto, estudiante de Ingeniería electrónica y telecomunicaciones  en la Universidad del Cauca, puedo comentar que en mi carrera he manejado algunos temas que se verán en el ciclo 3, además he manejado la metodología Scrum para desarrollar un sitio web usando php, http, javaScript y css.',
        rol: '(Main Backend Developer)',
        image: 'https://avatars3.githubusercontent.com/u/75052415?s=96&v=4'
        },
        {
        codigo: 3,
        nombre: 'Harold Alejandro Caicedo',
        descripcion: 'Mi nombre es Alejandro Caicedo, soy estudiante de último semestre de ingeniería electrónica, durante mi carrera he tenido experiencia en el desarrollo y diseño de interfaces para aplicaciones móviles y páginas web. Tengo habilidades para la comunicación escrita y en cuanto al entorno de desarrollo del ciclo 3 tengo conocimientos de javascript. Finalmente tengo conocimiento en la gestión de proyectos para la innovación en perfiles educativos.',
        rol: '(Frontend Developer)',
        image: 'https://avatars0.githubusercontent.com/u/75107873?s=96&v=4'
        },
        {
        codigo: 4,
        nombre: 'Juan Sebastian Orduz',
        descripcion: 'Soy Ingeniero Electronico y Telecomunicaciones, me gradue el año pasado. Este 2020 estuve trabajando como desarrollador backend utilizando Django y DRF.',
        rol: '(Backnd Developer)',
        image: 'https://avatars2.githubusercontent.com/u/75085664?s=96&v=4'
        }
      ]
    }
  }
}
</script>

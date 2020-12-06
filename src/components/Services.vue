<template>
  <div class="container-fluid" id="services">
    <div class="row justify-content-center mb-5">
      <div
        v-for="(service, index) of services"
        :key="index"
        class="col-sm-6 col-xs-12 col-lg-4 mt-5"
      >
        <div class="card h-100">
          <div class="d-flex justify-content-center p-2">
            <img :src="service.img" :alt="service" class="img-fluid" />
          </div>
          <div class="card-body">
            <h3 class="card-title">{{ service.title }}</h3>
            <p class="card-text text-justify">
              {{ service.description }}
            </p>
            <a :href="service.url">Ver mas...</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import imagen_servicio1 from "../assets/imgs/servicio1 (1).jpg";
import imagen_servicio2 from "../assets/imgs/servicio2 (1).png";
import imagen_servicio3 from "../assets/imgs/servicio3 (1).jpg";

export default {
  name: "Services",
  data() {
    return {
      services: [
        {
          title: "TutoTIC",
          img: imagen_servicio1,
          description:
            "Servicio para brindar tutorías academicas y clases en vivo gratuitas a estudiantes, que podrán realizarse en grupos de máximo 3 estudiantes a través de videollamadas, llamadas telefónicas, correo o vía Chat.",
          url: "https://tutotic.gov.co/",
        },
        {
          title: "Marketing a emprendedores",
          img: imagen_servicio2,
          description:
            "Posiciona tu emprendimiento recibiendo 1 dominio gratuito por un año, alojamiento de 1GB, plantilla web para la creación de tu sitio web.",
          url: "https://innpulsacolombia.com/dominio-co",
        },
        {
          title: "Talentos en primera fila",
          img: imagen_servicio3,
          description:
            "Empresas de cualquier sector podrán postular retos y posteriormente, en una siguiente etapa, los estudiantes de Misión TIC plantearán soluciones a través de la programación. Interacpedia seleccionará los mejores talentos y se ofrecerán a las empresas que participen.",
          url: "https://interacpedia.com/",
        },
      ],
    };
  },
  props: ["member"],
};
</script>

<style scoped>
</style>

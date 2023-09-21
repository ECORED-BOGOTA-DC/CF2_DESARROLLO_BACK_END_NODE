<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
  
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción
    .row.bg-c1
      .col-12
        .px-5.pt-5
          .row.align-items-center.mb-5(data-aos="fade-right")
            .col-md-auto.mb-4.mb-md-0
              figure
                img(src='@/assets/curso/intro/img1.png', style="width: 80px" ,alt='Texto que describa la imagen').m-auto
            .col
              p.mb-0 Le damos la bienvenida a este componente formativo en el que se estudiará la construcción de API RESTful con Node.js; para conocer la importancia del tema y los diferentes componentes que se incluirán, le invitamos a ver el siguiente video:
          figure(data-aos="fade-left")
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/GEgsJSgEPAk?si=JY9qzgPPd-YH0Tzi" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    
</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass"></style>

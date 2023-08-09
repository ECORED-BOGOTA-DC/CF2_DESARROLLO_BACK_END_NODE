<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p.mb-5 El Node.js se considera un entorno de código abierto para JavaScript; asíncrono, diseñado para crear aplicaciones #[i network] escalables, por lo que se hace necesario conocer a profundidad sus generalidades, dependencias, comandos, herramientas y direccionamiento básico, entre otras cosas. De igual manera se debe conocer de construcción API con el fin de poder crear una API RESTful que logre una comunicación con MongoDB. Por esta razón este componente formativo profundizó estos temas, los cuales se resumen a través del siguiente esquema:
    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="alt")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>

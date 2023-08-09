<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 1
      h1 Definiciones
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema1/img1.png', style="width: 370px" ,alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p.mb-0 Como hemos mencionado, la mayoría de los sistemas de información requieren la gestión y transformación de datos, que, generalmente, se almacenan y protegen en sistemas gestores de bases de datos; sin embargo, se pueden presentar diferentes situaciones en las que se necesite refactorizar las funcionalidades ya establecidas, por lo que el uso de API RESTful es la respuesta para efectuar tales actualizaciones sin afectar el desempeño normal del sistema.
    .row.align-items-center.mb-5(data-aos="fade-left")
      .col-lg-4.bg-c2.mb-4.mb-lg-0
        .p-4
          p.ms-5.fs-4.mb-0 #[b Entonces,]
          p.ms-5.fs-4.mb-0 #[b ¿qué es una API?]
      .col-lg-8
        .cajon.color-primario.p-4
          .row.align-items-center
            .col-auto
              figure
                img(src='@/assets/curso/tema1/img2.svg', style="width: 70px" ,alt='').m-auto
            .col
              p.mb-0 #[i Application Programming Interfaces (API)], que traducido literalmente al español significa Interfaz de programación de aplicaciones; es esencialmente un conjunto de especificaciones, reglas y/o mecanismos que se definen para establecer la comunicación entre dos componentes de #[i software].
    p(data-aos="fade-right") Así, una API de REST o conocida también como API RESTful es una interfaz que permite la comunicación entre dos componentes de #[i software], usualmente, entre un sistema gestor de base de datos y una aplicación de #[i software] que la consume.
    p.mb-5(data-aos="fade-right") Hasta aquí hemos agregado otro término, REST,
    .row.align-items-center.mb-3
      .col-lg-8.mb-4.mb-lg-0(data-aos="fade-right")
        figure.mb-4
          img(src='@/assets/curso/tema1/img3.svg', style="width: 850px" ,alt='').m-auto
        p Una de las características de REST consiste en el no almacenamiento del estado; es decir, cada vez que se realiza una solicitud de transmisión, el emisor se debe identificar por medio de credenciales o tokens, ya que esta información no se almacena de ninguna forma. Aunque esto parece una desventaja, se encuentra que, al no tratar con el manejo de memoria, se disminuyen los procesos requeridos para el procesamiento de los datos y lo hace altamente compatible para ser utilizado por cualquier tecnología y para entornos con necesidades de escalamiento horizontal.
        p.mb-0 Por medio de una API REST se pueden implementar los HTTPVerbs o los métodos HTTP, por medio de los cuales se especifica el tipo de solicitud que se realiza al servidor y así este puede dar el tratamiento adecuado y ofrecer respuestas correctas.
      .col-lg-4(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema1/img2.png', style="width: 370px" ,alt='').m-auto
    p.mb-5 Veamos cada uno de los métodos HTTP y su función o uso:
    .tarjeta.tarjeta--amarilla.mb-5(data-aos="fade-left")
      .p-4
        SlyderA(tipo="b")
          .row.justify-content-center.align-items-center
            .col-lg-4.mb-4.mb-lg-0
              p.mb-0 #[b GET]
              p Consulta de información al servidor, equivale a una solicitud #[i find()] en NOSQL o SELECT en SQL.
            .col-lg-6
              figure
                img(src='@/assets/curso/tema1/img3.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
          .row.justify-content-center.align-items-center
            .col-lg-4.mb-4.mb-lg-0
              p.mb-0 #[b POST]
              p Este método se usa para el envío de información al servidor generalmente para realizar un proceso de registro de datos, obligatoriamente implica el envío de datos adicionales en la solicitud. Es equivalente a un comando tipo #[i InsertOne()] o #[i InsertMany()] en NoSQL o la sentencia INSERT en SQL.
            .col-lg-6
              figure
                img(src='@/assets/curso/tema1/img4.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
          .row.justify-content-center.align-items-center
            .col-lg-4.mb-4.mb-lg-0
              p.mb-0 #[b PUT]
              p Este método es similar al anterior, pero se utiliza para la actualización de datos del lado del servidor. Es equivalente a un comando #[i updateOne()] o #[i updateMany()] en NOSQL o una sentencia UPDATE en SQL.
            .col-lg-6
              figure
                img(src='@/assets/curso/tema1/img5.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
          .row.justify-content-center.align-items-center
            .col-lg-4.mb-4.mb-lg-0
              p.mb-0 #[b PATCH]
              p Este método también se utiliza para la actualización de registros en la base de datos, pero solo cuando la actualización es parcial y no del registro completo.
            .col-lg-6
              figure
                img(src='@/assets/curso/tema1/img6.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
          .row.justify-content-center.align-items-center
            .col-lg-4.mb-4.mb-lg-0
              p.mb-0 #[b DELETE]
              p Método utilizado para la eliminación de registro en el servidor. Es equivalente al comando #[i deleteOne()] o #[i deleteMany()] en NoSQL y a la sentencia DELETE de SQL.
            .col-lg-6
              figure
                img(src='@/assets/curso/tema1/img7.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
          .row.justify-content-center.align-items-center
            .col-lg-4.mb-4.mb-lg-0
              p.mb-0 #[b HEAD]
              p Método que sirve para obtener información general de los recursos del servidor como, por ejemplo, validar la accesibilidad. No sirve para la gestión directa de registros propios del servidor.
            .col-lg-6
              figure
                img(src='@/assets/curso/tema1/img8.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
    p.mb-5(data-aos="fade-right") Ahora bien, según Red Hat (2020) una API RESTful debe cumplir con los siguientes criterios:
    SlyderF(columnas="col-lg-6 col-xl-4")(data-aos="fade-left")
      .tarjeta.color-primario.p-4
        .row.justify-content-center.mb-3
          .col-12
            img(src='@/assets/curso/tema1/img9.png' alt='AvatarTop')
        p.mb-0 Debe usar arquitectura tipo cliente servidor con manejo de solicitudes por medio del protocolo HTTP.
      .tarjeta.color-primario.p-4
        .row.justify-content-center.mb-3
          .col-12
            img(src='@/assets/curso/tema1/img10.png' alt='AvatarTop')
        p.mb-0 Manejo de comunicaciones entre cliente y el servidor sin almacenar el estado.
      .tarjeta.color-primario.p-4
        .row.justify-content-center.mb-3
          .col-12
            img(src='@/assets/curso/tema1/img11.png' alt='AvatarTop')
        p.mb-0 Los datos pueden almacenarse en caché para operaciones clave y así eliminar interacciones entre el cliente y el servidor.
      .tarjeta.color-primario.p-4
        .row.justify-content-center.mb-3
          .col-12
            img(src='@/assets/curso/tema1/img12.png' alt='AvatarTop')
        p.mb-0 Arquitectura en capas que separe las solicitudes de los clientes y las respuestas del servidor.
      .tarjeta.color-primario.p-4
        .row.justify-content-center.mb-3
          .col-12
            img(src='@/assets/curso/tema1/img13.png' alt='AvatarTop')
        p.mb-0 Debe existir una interfaz uniforme de comunicación.
      
</template>

<script>
export default {
  name: 'Tema1',
  components: {},
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

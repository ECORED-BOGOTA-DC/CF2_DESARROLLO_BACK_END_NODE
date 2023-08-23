<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 2
      h1 Generalidades de Node.js
    .row.align-items-center.mb-3
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema2/img1.png', style="width: 370px" ,alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p JavaScript es, tal vez, uno de los lenguajes más comunes en el desarrollo de aplicaciones web; generalmente, este lenguaje permite enriquecer el contenido que se muestra a los clientes por medio de un navegador web y junto a HTML y CSS completan el paquete completo de elementos que se debe combinar para ofrecer una buena experiencia de navegación por sitios WEB.
        p Así, es importante que conozcamos a qué hace referencia los términos HTML, CSS y JavaScript.
        p.mb-0 Como observamos, JavaScript se ejecuta del lado del cliente, esto significa que utiliza los recursos del equipo de cómputo del usuario que usa el navegador web, para controlar muchos de los procesos de validaciones y de gestión de datos. En este sentido, se podría decir que Node.js es la versión de JavaScript que puede gestionar la ejecución de código del lado del servidor como lo hacen los lenguajes PHP, ASP.NET, JSP, entre otros.
    p.mb-5 Conozcamos algunas de las características de Node.js y JavaScript:
    .row.bg-c3.mb-5(data-aos="fade-down")
      .col-12
        .p-4.p-lg-5
          ImagenInfografica.color-acento-botones
            template(v-slot:imagen)
              figure
                img(src='@/assets/curso/tema2/img1.svg', alt='')
            .tarjeta.color-secundario.shadow-lg.p-3(x="13%" y="22%" numero="+")
              p.mb-0 #[b Tiene código abierto]
              p.mb-0 Node.js en un entorno de ejecución #[i Open Source] (código abierto), multiplataforma.
            .tarjeta.color-secundario.shadow-lg.p-3(x="53%" y="18%" numero="+")
              p.mb-0 #[b Orientado a eventos asincrónicos]
              p.mb-0 Se orienta a eventos asíncronos que puede ejecutar código JavaScript por fuera de los entornos de un navegador web.
            .tarjeta.color-secundario.shadow-lg.p-3(x="55%" y="57%" numero="+")
              p.mb-0 #[b Es tendencia]
              p.mb-0 Actualmente, Node.js se posiciona como una tendencia muy importante en el mundo laboral relacionado con estas tecnologías web.
    .row.justify-content-center(data-aos="fade-right")
      .col-lg-7
        .cajon.color-primario.p-4
          p.mb-0 Según la encuesta Stack Overflow (2021), desde hace nueve años, JavaScript es el lenguaje de programación más utilizado por desarrolladores profesionales; asimismo, Node.js se ubica en la sexta posición de uso en esta misma encuesta, con lo cual se marca una tendencia.
    Separador
    #t_2_1
    .titulo-segundo.color-acento-contenido
      h2 2.1 Instalación de herramientas
    p(data-aos="fade-right") Para la instalación de Node.js se recomienda acceder a su página oficial de descargas ubicada en la dirección: 
      |
      a(href="https://nodejs.org/es/download/" target="_blank") https://nodejs.org/es/download/
      |, en donde se presentan distribuciones para los sistemas operativos Windows y MacOS e incluso con el código fuente, recordemos que esta es una plataforma #[i open source].
    p(data-aos="fade-down") En la siguiente figura se observan las diferentes posibilidades de instalación habilitadas actualmente:
    .row.bg-c4(data-aos="fade-right")
      .col-12
        .p-4.p-lg-5
          .titulo-sexto.color-acento-contenido.mb-5
            p.mb-0 #[b Figura 1]. Visiones instaladores Node.js
          .row.justify-content-center
            .col-lg-10
              figure
                img(src='@/assets/curso/tema2/img2.png', style="width: 1200px" ,alt='').m-auto
                figcaption.mt-3 Nota. 
                  | 
                  a(href="https://nodejs.org/es/download/" target="_blank") #[u https://nodejs.org/es/download/]
    p.mb-5(data-aos="fade-down") Como se observa en dicha figura, la página oficial recomienda la descarga de versiones LTS (#[i Long Term Support]), lo que significa que estas versiones tienen soporte de largo plazo y un funcionamiento estable, altamente validado y con gran cantidad de documentación asociada.
    .row.justify-content-center.mb-5(data-aos="fade-down")
      .col-lg-8
        .tarjeta-avatar-b.mb-4.mb-lg-0
          .tarjeta-avatar-b__img
            img(src='@/assets/curso/tema2/img3.svg' alt='AvatarTop')
          .tarjeta.tarjeta--azul2
            .p-4
              p.mb-0.my-4 Es importante anotar que este campo del desarrollo #[i software] es muy dinámico, con permanentes actualizaciones que generan diferentes versiones; así, la última versión LTS de Node.js es la 16.15.0 y la de Node.js corresponde a la 18.1.0. Sin embargo, aunque estas herramientas son tan activas, presentan algunas generalidades que son esenciales conocer, con las cuales se garantiza su funcionamiento independiente de la versión que se descargue.
    .row.align-items-center.mb-4
      .col-lg-8.mb-4.mb-lg-0(data-aos="fade-right")
        p Adicionalmente, se requiere de un IDE de programación que permita el cargue y la ejecución de los paquetes de Node.js. En este punto, puede hacer uso de cualquier IDE que utilice normalmente para el desarrollo de aplicaciones afines a la web, particularmente se recomienda el uso de Visual Studio Code.
        p Este es un editor de código fuente que puede ser utilizado para el desarrollo de lenguajes como Python, Java, PHP, HTML/CSS, TypeScript, YAML y, por supuesto, JavaScript; tiene la posibilidad de ampliar sus funciones con plugins y buscadores de otros plugins, lo que permite una mayor personalización, según las necesidades de los usuarios, sin afectar su condición de código muy potente y liviano.
        .row
          .col-12.bg-c5
            .p-4
              p Las siguientes son algunas de las características importantes de este editor de código:
              ul.lista-ul.mb-0
                li.d-flex
                  i.fas.fa-check(style="color: #FFC202")
                  |
                  p.mb-0 Soporte para depuración.
                li.d-flex
                  i.fas.fa-check(style="color: #FFC202")
                  |
                  p.mb-0 Integración con sistemas de versionamiento como GIT.
                li.d-flex
                  i.fas.fa-check(style="color: #FFC202")
                  |
                  p.mb-0 Verificación de sintaxis.
                li.d-flex
                  i.fas.fa-check(style="color: #FFC202")
                  |
                  p.mb-0 Ayudas de finalización de código inteligente.
                li.d-flex
                  i.fas.fa-check(style="color: #FFC202")
                  |
                  p.mb-0 Opciones de refactorización de código.
      .col-lg-4(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema2/img3.png', style="width: 410px" ,alt='').m-auto
    p.mb-5(data-aos="fade-right") Visual Studio Code puede ser descargado de forma gratuita directamente desde su página oficial: 
      |
      a(href="https://code.visualstudio.com/Download" target="_blank") https://code.visualstudio.com/Download
      |, está disponible para sistemas operativos Windows, versiones de Linux Debian, Ubuntu, Red Hat, Fedora y SUSE y sistema operativo MacOS.
    .row.bg-c4.mb-5(data-aos="fade-down")
      .col-12
        .p-4.p-lg-5
          .titulo-sexto.color-acento-contenido.mb-5
            p.mb-0 #[b Figura 2]. Versiones instaladores Visual Studio Code
          .row.justify-content-center
            .col-lg-10
              figure
                img(src='@/assets/curso/tema2/img4.png', style="width: 1200px" ,alt='').m-auto
                figcaption.mt-3 Nota. 
                  | 
                  a(href="https://code.visualstudio.com/Download" target="_blank") #[u https://code.visualstudio.com/Download]
    p(data-aos="fade-right") Por último, se requiere de un sistema que nos permita hacer uso de la API REST para verificar su funcionamiento; recordemos que la API RESTful es un intermediario entre un sistema de base de datos y una aplicación que hace uso de estos servicios. Si bien las solicitudes que se realizan a la API se hacen por medio de HTTP, solo las solicitudes de tipo GET pueden ser verificadas por medio de un navegador web.
    .row.align-items-center.mb-3
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema2/img5.svg', style="width: 410px" ,alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p Recordemos que hay otros tipos de métodos que requieren de un mecanismo que permita identificar los parámetros y el tipo de método para ser procesado en el servidor.
        p.mb-0 Para suplir esta necesidad, se recomienda instalar Postman, plataforma que facilita la construcción y prueba de APIS con una versión libre, con las funcionalidades necesarias para la verificación del funcionamiento de todos los métodos HTTP de nuestras API RESTFul.
    p.mb-5(data-aos="fade-right") Puede utilizar esta plataforma de dos formas:
    ol.lista-ol--cuadro(data-aos="fade-right")
      li.d-flex
        .lista-ol--cuadro__vineta
          span #[b 1.]
        | 
        p.mb-0 Descargue la versión #[i desktop] desde la página oficial disponible en: 
          |
          a(href="https://www.postman.com/downloads/" target="_blank") https://www.postman.com/downloads/
    .row.bg-c4.mb-5(data-aos="fade-down")
      .col-12
        .p-4.p-lg-5
          .titulo-sexto.color-acento-contenido.mb-5
            p.mb-0 #[b Figura 3]. Interfaz principal de Postman
          .row.justify-content-center
            .col-lg-10
              figure
                img(src='@/assets/curso/tema2/img5.png', style="width: 1200px" ,alt='').m-auto
                figcaption.mt-3 Nota. 
                  | 
                  a(href="https://www.postman.com" target="_blank") #[u https://www.postman.com]
    .row.bg-c1
      .col-12
        .px-5.pt-5
          ol.lista-ol--cuadro.mb-5(data-aos="fade-right")
            li.d-flex
              .lista-ol--cuadro__vineta
                span #[b 2.]
              | 
              p.mb-0 Realice el registro en línea, ingresando a la página oficial disponible en: 
                |
                a(href="https://www.postman.com/downloads/" target="_blank") https://www.postman.com
                |, en este caso, le invitamos a observar el siguiente video, en el que se presenta el proceso para la instalación y configuración de Postman:
          figure(data-aos="fade-left")
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    Separador
    #t_2_2
    .titulo-segundo.color-acento-contenido
      h2 2.2 Dependencias
    .row.align-items-center.mb-4
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema2/img6.png', style="width: 370px" ,alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p Una de las grandes potencialidades de Node.js es precisamente la facilidad de acoplar y reutilizar paquetes de JavaScript públicos que agilizan y disminuyen el tiempo requerido para la creación de servicios de alta calidad en muy poco tiempo. Node.js utiliza NPM para lograr estos resultados.
        .row
          .col-lg-4.bg-c6.mb-4.mb-lg-0
            .p-4
              p.ms-4.fs-4.mb-0 #[b ¿Qué significa y cómo opera NPM?]
          .col-lg-8
            .cajon.color-primario.p-4
              p #[b #[i Node Package Manager] (NPM) es el administrador de paquetes de Node y es el encargado de realizar las tres actividades fundamentales (npm, Inc):]
              ul.lista-ul.mb-0
                li.d-flex
                  i.fas.fa-circle(style="color: #FFC202")
                  |
                  p.mb-0 Ayuda a los desarrolladores JavaScript a compartir fácilmente módulos de código empaquetados.
                li.d-flex
                  i.fas.fa-circle(style="color: #FFC202")
                  |
                  p.mb-0 Sirve de colección pública de paquetes de código fuente abierto para Node.js.
                li.d-flex
                  i.fas.fa-circle(style="color: #FFC202")
                  |
                  p.mb-0 Sirve como interfaz de línea de comandos que permite instalar y publicar esos paquetes.
    p(data-aos="fade-right") A continuación, se detallan algunos de estos paquetes que serán usados en la construcción de la API RestFul:
    .row.justify-content-center.mb-0.mb-lg-4(data-aos="fade-up")
      .col-md-7.col-xl-4.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img7.png')})`}")
            .tarjeta-flip__contenido.p-4
              figure.mb-4
                img(src='@/assets/curso/tema2/img12.png', style="width: 60px" ,alt='').m-auto
              p.text-center.mb-0 Se considera un #[i framework] de Node.js minimalista y flexible que facilita las operaciones requeridas para la construcción de una aplicación como son el enrutamiento de URL, gestión de sesiones, cookies.
      .col-md-7.col-xl-4.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img8.png')})`}")
            .tarjeta-flip__contenido.p-4
              figure.mb-4
                img(src='@/assets/curso/tema2/img12.png', style="width: 60px" ,alt='').m-auto
              p.text-center.mb-0 Librería Node.js basada en modelado de datos orientados a objetos para MongoDB muy similar a un ORM en sistemas de bases de datos relacionales. Mongoose permite la aplicación de un esquema específico desde la capa de aplicación y facilita la ejecución de operaciones en bases de datos NOSQL como establecer la conexión y la ejecución de comando.
      .col-md-7.col-xl-4.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img9.png')})`}")
            .tarjeta-flip__contenido.p-4
              figure.mb-4
                img(src='@/assets/curso/tema2/img12.png', style="width: 60px" ,alt='').m-auto
              p.text-center.mb-0 Es común intentar hacer lecturas sobre la información alojada en las solicitudes HTTP transferidas y recibidas desde el servidor, como, por ejemplo, examinar los parámetros enviados en una solicitud de tipo POST, PUT o DELETE. Este paquete de Node.js se encarga de la lógica necesaria para acceder a la información de los cuerpos en las solicitudes.
    .row.justify-content-center(data-aos="fade-up")
      .col-md-7.col-xl-4.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img10.png')})`}")
            .tarjeta-flip__contenido.p-4
              figure.mb-4
                img(src='@/assets/curso/tema2/img12.png', style="width: 60px" ,alt='').m-auto
              p.text-center.mb-0 Paquete de Node.js que funciona como Middleware de registro de las solicitudes y errores HTTP.
      .col-md-7.col-xl-4.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img11.png')})`}")
            .tarjeta-flip__contenido.p-4
              figure.mb-4
                img(src='@/assets/curso/tema2/img12.png', style="width: 60px" ,alt='').m-auto
              p.text-center.mb-0 Herramienta que se encarga de detectar cualquier cambio en el código del servidor para relanzar la ejecución de los servicios aplicando los cambios detectados.
    Separador
    #t_2_3
    .titulo-segundo.color-acento-contenido
      h2 2.3 Comandos y direccionamiento básico
    p.mb-5(data-aos="fade-right") A continuación se especifican algunos de los comandos que se ejecutan en una terminal tipo Shell y son utilizados durante la creación y gestión de una aplicación desarrollada con Node.js junto a su función:
    .row.mb-5
      .col-lg-7.mb-4.mb-lg-0(data-aos="fade-right")
        AcordionA(tipo="a" clase-tarjeta="tarjeta tarjeta--azul")
          .row(titulo="npm init")
            .col-auto
              figure
                img(src='@/assets/curso/tema2/img13.png', style="width: 60px" ,alt='').m-auto
            .col
              p.mb-0 Comando usado para configurar un paquete npm nuevo o existente. Crea el archivo package.json.
          .row(titulo="npm start")
            .col-auto
              figure
                img(src='@/assets/curso/tema2/img13.png', style="width: 60px" ,alt='').m-auto
            .col
              p.mb-0 Ejecuta el comando predefinido en la propiedad “start” del objeto Script de un paquete (package.json).
          .row(titulo="npm install express")
            .col-auto
              figure
                img(src='@/assets/curso/tema2/img13.png', style="width: 60px" ,alt='').m-auto
            .col
              p.mb-0 Instala el paquete de Express en el proyecto y toda aquella dependencia adicional requerida por Express.
          .row(titulo="npm install express")
            .col-auto
              figure
                img(src='@/assets/curso/tema2/img13.png', style="width: 60px" ,alt='').m-auto
            .col
              p.mb-0 Instala el paquete de Mongoose en el proyecto y toda aquella dependencia adicional requerida por Mongoose.
          .row(titulo="npm install morgan")
            .col-auto
              figure
                img(src='@/assets/curso/tema2/img13.png', style="width: 60px" ,alt='').m-auto
            .col
              p.mb-0 Instala el paquete de Morgan en el proyecto y toda aquella dependencia adicional requerida por Morgan.
          .row(titulo="npm install body-parser")
            .col-auto
              figure
                img(src='@/assets/curso/tema2/img13.png', style="width: 60px" ,alt='').m-auto
            .col
              p.mb-0 Instala el paquete de Body-parser en el proyecto y toda aquella dependencia adicional requerida por Body-parser.
          .row(titulo="npm install nodemon")
            .col-auto
              figure
                img(src='@/assets/curso/tema2/img13.png', style="width: 60px" ,alt='').m-auto
            .col
              p.mb-0 Instala el paquete de Nodemon en el proyecto y toda aquella dependencia adicional requerida por Nodemon. Es necesario indicar el uso de Nodemon en el script start del paquete Json.
      .col-lg-5(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema2/img6.svg', style="width: 470px" ,alt='').m-auto
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0.d-none.d-lg-block(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema2/img14.png', style="width: 370px" ,alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p Recuerde que las Rutas o #[i Routes] son el concepto usado en Node.js para referirse a los componentes que permiten gestionar el direccionamiento dentro de una aplicación. Estas permiten asociar los métodos HTTP (GET, POST, PUT, DELETE, etc.) un patrón o camino URL (URL path) y con la función que será ejecutada para controlar dicho patrón.
        p.mb-0 En Node.js se utiliza el paquete de Express para la gestión de las rutas y tendrá una estructura similar a la que se visualiza en la siguiente figura:
    .row.bg-c7(data-aos="fade-down")
      .col-12
        .p-4.p-lg-5
          .titulo-sexto.color-acento-contenido.mb-5
            p.mb-0 #[b Figura 4]. Esquema general de manejo de rutas en Node.
          .row.justify-content-center
            .col-lg-10
              figure
                img(src='@/assets/curso/tema2/img15.png', style="width: 1200px" ,alt='').m-auto
    p.mb-0(data-aos="fade-right") Como se puede observar en la imagen se necesita de una instancia de la clase Router() de express; luego, se debe instanciar el controlador que tiene definidas las acciones para un modelo específico y finalmente, con la instancia de la clase #[i router] definimos el método HTTP, la ruta relativa por donde será accedido desde una solicitud web a la API publicada por el servicio junto a la función específica en el controlador encargado de darle respuesta.

</template>

<script>
export default {
  name: 'Tema2',
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

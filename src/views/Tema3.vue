<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 3
      h1 Construcción API
    p.mb-0(data-aos="fade-right") En este momento ya disponemos de las herramientas de #[i software] necesarias y los conceptos involucrados en la construcción de la APi RestFull, ahora veamos los siguientes aspectos a tener en cuenta:
    Separador
    #t_3_1
    .titulo-segundo.color-acento-contenido
      h2 3.1. Conexión Node.js y MongoDB
    p(data-aos="fade-right") Lo primero que se debe realizar es la construcción de una aplicación Node.js que se pueda ejecutar satisfactoriamente y luego tratar de establecer una conexión con el servidor MongoDB que previamente ha sido configurado como sistema gestor de base de datos.
    p.mb-5(data-aos="fade-left") Se recomienda realizar los siguientes pasos:
    .row.mb-4(data-aos="fade-down")
      .col-12
        .p-4.p-lg-5
          ImagenInfografica.color-acento-botones
            template(v-slot:imagen)
              figure
                img(src='@/assets/curso/tema3/img1.svg', alt='')
            .tarjeta.color-secundario2.shadow-lg.p-3(x="6.4%" y="100%" numero="+")
              p.mb-0 Crear una carpeta en la que se almacenará el código fuente de la aplicación.
            .tarjeta.color-secundario2.shadow-lg.p-3(x="28.2%" y="100%" numero="+")
              p.mb-0 Utilizar el IDE Visual Studio Code para cargar esta carpeta e iniciar con la configuración del espacio de trabajo con la ejecución del comando npm int.
            .tarjeta.color-secundario2.shadow-lg.p-3(x="50%" y="100%" numero="+")
              p.mb-0 Incluir todas las dependencias a ser usadas por el proyecto por medio del comando npm install paquete.
            .tarjeta.color-secundario2.shadow-lg.p-3(x="72%" y="100%" numero="+")
              p.mb-0 Una vez definidas las dependencias se debe crear un archivo de extensión js donde se importarán todas las dependencias, la lógica de conexión a la base de datos utilizando Mongoose.
            .tarjeta.color-secundario2.shadow-lg.p-3(x="93.7%" y="100%" numero="+")
              p.mb-0 Finalmente, el puerto por donde el servidor escucha las solicitudes una vez se ejecuta el comando npm start.
    .row.bg-c1.mb-5(data-aos="fade-right")
      .col-12
        .px-5.pt-5
          figure(data-aos="fade-left")
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    p.mb-5(data-aos="fade-down") Basado en la explicación anterior, en la siguiente figura se visualiza el resultado final esperado luego de realizar el proceso de creación y configuración inicial del servidor:
    .row.bg-c7(data-aos="fade-left")
      .col-12
        .px-5
          .titulo-sexto.color-acento-contenido.mb-5
            p.mb-0 #[b Figura 5]. Ejecución del servidor Node.js por medio de la terminal de Visual Studio Code.
          .row.justify-content-center
            .col-lg-10
              figure
                img(src='@/assets/curso/tema3/img1.png', style="width: 1200px" ,alt='').m-auto
    Separador
    #t_3_2
    .titulo-segundo.color-acento-contenido
      h2 3.2. Construcción de consultas con Node
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema3/img2.png', style="width: 370px" ,alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p Para la construcción del servicio RESTful se recomienda utilizar algún patrón arquitectónico que facilite la disminución de dependencias, la actualización rápida de componentes y facilidades para el escalamiento y pruebas. Tenga en cuenta que esta API es la responsable de definir el esquema de base de datos y la forma en que será manipulado por los clientes.
        p Para controlar el esquema de la base de datos deberá hacer uso de una instancia de la clase Schema de la librería mongoose.js, con el cual definirá un modelo o estructura general de los documentos que serán almacenados en MongoDB, especificando como mínimo cada uno de los campos con su correspondiente tipo de dato.
        .tarjeta.color-secundario.p-4.p-md-5
          .row.justify-content-around.align-items-center
            .col-8.col-sm-6.col-md-4.mb-4.mb-md-0
              img(src="@/assets/curso/tema3/img2.svg")
            .col-md.col-lg-6
              h3(style="color: #12263F") Para tener más detalles puede consultar el siguiente enlace:
              a.boton.color-acento-botones.texto-blanco(href="https://mongoosejs.com/docs/guide.html" target="_blank" type="application/pdf")
                span(style="color: #12263F !important") Descargar
                i.fas.fa-file-download(style="color: #12263F !important")
    p.mb-5 Veamos entonces a través de la siguiente figura la estructura general requerida para crear un nuevo modelo:
    .row.bg-c7.mb-5(data-aos="fade-right")
      .col-12
        .px-5
          .titulo-sexto.color-acento-contenido.mb-5
            p.mb-0 #[b Figura 6]. Esquema general de un modelo.
          .row.justify-content-center
            .col-lg-10
              figure
                img(src='@/assets/curso/tema3/img3.png', style="width: 1200px" ,alt='').m-auto
    p.mb-5(data-aos="fade-down") Una vez definidos los modelos se deben crear los controladores que determinan las operaciones a realizar en dicho modelo, entre las más comunes se encuentran:
    .row.justify-content-center.mb-5(data-aos="fade-right")
      .col-10.col-md-7.col-lg-3.mb-4.mb-lg-0
        .row.align-items-center
          .col-auto(style="z-index: 2")
            figure
              img(src='@/assets/curso/tema3/img3.svg', style="width: 80px" ,alt='').m-auto
          .col.bg-c8(style="z-index: 1")
            .ps-4.py-2
              p.mb-0 #[b Buscar un documento específico.]
      .col-10.col-md-7.col-lg-3.mb-4.mb-lg-0
        .row.align-items-center
          .col-auto(style="z-index: 2")
            figure
              img(src='@/assets/curso/tema3/img4.svg', style="width: 80px" ,alt='').m-auto
          .col.bg-c8(style="z-index: 1")
            .ps-4.py-2
              p.mb-0 #[b Buscar un documento específico.]
      .col-10.col-md-7.col-lg-3
        .row.align-items-center
          .col-auto(style="z-index: 2")
            figure
              img(src='@/assets/curso/tema3/img5.svg', style="width: 80px" ,alt='').m-auto
          .col.bg-c8(style="z-index: 1")
            .ps-4.py-2
              p.mb-0 #[b Buscar un documento específico.]
    p.mb-5(data-aos="fade-right") Los controladores harán uso de los métodos que serán emparejados con los comandos que se ejecutan del lado de MongoDB.
    .tarjeta.color-secundario.p-4.p-md-5.mb-5(data-aos="fade-down")
      .row.justify-content-around.align-items-center
        .col-8.col-sm-6.col-md-3.mb-4.mb-md-0
          img(src="@/assets/curso/tema3/img2.svg")
        .col-md.col-lg-6
          h3(style="color: #12263F") Si desea profundizar en la funciones disponibles para los modelos de mongoose, consulte la documentación oficial disponible en:
        .col-auto
          a.boton.color-acento-botones.texto-blanco(href="https://mongoosejs.com/docs/models.html" target="_blank" type="application/pdf")
            span(style="color: #12263F !important") Ver Enlace
            i.fas.fa-file-download(style="color: #12263F !important")
    .row.bg-c1.mb-5(data-aos="fade-left")
      .col-12
        .px-5.pt-5
          figure(data-aos="fade-left")
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.align-items-center.mb-5
      .col-lg-8.mb-4.mb-lg-0(data-aos="fade-right")
        p El último paso para completar la API RESTful es la construcción de las rutas. Tenga en cuenta que estas deben ser importadas en la clase de servidor. Se recomienda tener direcciones de rutas por cada modelo del esquema de la base de datos e implementar como mínimo en el controlador todos los métodos tipo CRUD que serán utilizados por los clientes externos.
        p.mb-0 Es por ello, que en el siguiente video se muestra un ejemplo, en el que se realiza el proceso para crear las rutas de cada uno de los métodos definidos en el controlador y la forma de adecuar el servicio para hacer uso de estas rutas; también se indica cómo utilizar la herramienta Postman para hacer las pruebas manuales de cada una de las rutas definidas.
      .col-lg-4(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema3/img4.png', style="width: 370px" ,alt='').m-auto
    .row.bg-c1.mb-5(data-aos="fade-down")
      .col-12
        .px-5.pt-5
          figure(data-aos="fade-left")
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema3/img5.png', style="width: 370px" ,alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p En el ejemplo anterior solo se implementaron las solicitudes HTTP de tipo GET y POST, la implementación de los otros métodos HTTP que complementan el CRUD siguen la misma dinámica; por ende, con los conocimientos adquiridos es posible completar el ejercicio sin ningún problema.
        p.mb-0 Recordemos que las operaciones que se pueden realizar sobre los documentos están establecidas en la clase controlador que importa el modelo particular sobre el que se realizarán las opciones. Así, se presentan algunas de estas funciones de Mongoose que pueden ejecutar acciones del lado de la base de datos MongoDB, conózcanoslas:
    .row.align-items-end.mb-5
      .col-lg-7.mb-4.mb-lg-0(data-aos="fade-right")
        AcordionA(tipo="a" clase-tarjeta="tarjeta tarjeta--verde")(data-aos="fade-down")
          .row(titulo="findByIdAndUpdate()")
            .col-12
              p Recibe como parámetro el Id del documento a buscar para la actualización  y el objeto con la información a ser utilizada en la actualización.
              p Si encuentra el registro, le aplica los cambios determinados en el objeto enviado y retorna el registro encontrado como respuesta.
              p.mb-0 Ejecuta el comando #[b.txt-c1 findOneAndUpdate] en mongoDB
          .row(titulo="findByIdAndDelete()")
            .col-12
              p Recibe como parámetro el id del documento a buscar, que será eliminado.
              p.mb-0 Ejecuta el comando #[b.txt-c1 findOneAndDelete()] en mongoDB
          .row(titulo="Save()")
            .col-12
              p Inserta un nuevo documento a la colección.
              p Debe crear un objeto del modelo que quiere registrar, llenar los campos e invocar a la función save()
              p Esta función retorna un valor indefinido, si hay error o el documento registrado, si el proceso es exitoso.
          .row(titulo="find()")
            .col-12
              p Recibe como parámetro un filtro que se utiliza para encontrar documentos en el esquema. Si el parámetro recibido es un filtro vacío quiere decir que se buscan todos los documentos del esquema.
              p Algunos ejemplo de la utilización del find podrían ser los siguientes:
              .row
                .col-12.bg-c9
                  .p-4
                    p.mb-0.txt-c2 //Encuentra todos los documentos de la colección MyModel
                    p MyModel.find({})
                    p.mb-0.txt-c2 //Encuentra todos los documentos de la colección MyModel cuyo campo name sea igual a ‘john’ y la edad sea igual o superior a 18.
                    p.mb-0 MyModel.find({ name: 'john', age: { $gte: 18 } })
          .row(titulo="findById()")
            .col-12
              p Recibe como parámetro el Id del documento a buscar en la colección.
              p Retorna como resultado un único documento si es que dicho Id existe.
              p Este método es equivalente al comando #[b.txt-c1 findOne()] de MongoDB, en el que solo se busca por el campo de identificación del documento.
      .col-lg-5(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema3/img6.svg', style="width: 460px" ,alt='').m-auto
    p(data-aos="fade-right") En la siguiente figura se muestra un borrador de la estructura que tendría una función en el controlador para actualizar una colección de tipo Modelo X, se puede observar que en el controlador se debe importar primero el modelo para poder invocar la función findByIDAndUpdate(), la cual recibirá como parámetro el id del documento a actualizar y el documento con toda su estructura de cómo debería quedar luego de la actualización. El método findByIDAndUpdate() asocia a la palabra reservada $set los valores a actualizar. Tenga en cuenta que cualquier campo de la colección puede ser actualizado excepto el identificador.
    p.mb-5(data-aos="fade-down") Los parámetros utilizados en la consulta son obtenidos desde el body del objeto de tipo request, es decir, que en el momento de hacer la solicitud del servicio se deberá hacer uso de un método de tipo POST o similar que acepte el envío de parámetros. Observe dicha figura:
    .row.bg-c7.mb-5(data-aos="fade-right")
      .col-12
        .px-5
          .titulo-sexto.color-acento-contenido.mb-5
            p.mb-0 #[b Figura 7]. Esquema general para la actualización de un documento de un modelo específico.
          .row.justify-content-center
            .col-lg-10
              figure
                img(src='@/assets/curso/tema3/img6.png', style="width: 1200px" ,alt='').m-auto
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema3/img7.png', style="width: 370px" ,alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p Por último, en la siguiente figura, se muestra un borrador de la estructura de una función que permite la eliminación de un documento, de acuerdo con un número de identificador dado. Al igual que las demás operaciones vistas, se requiere la importación del modelo sobre el que se va a realizar el proceso de eliminación y la invocación de la función findByIDAndRemove()
        p.mb-0 El parámetro del identificador debe ser capturado desde el body del objeto request, lo que implica que la invocación de este servicio se realizará por medio de un método POST o similar que acepte el envío de parámetros en el cuerpo de la solicitud enviada al servidor. Dicha figura es:
    .row.bg-c7.mb-5(data-aos="fade-right")
      .col-12
        .px-5
          .titulo-sexto.color-acento-contenido.mb-5
            p.mb-0 #[b Figura 8]. Esquema general para la eliminación de un documento de un modelo específico.
          .row.justify-content-center
            .col-lg-10
              figure
                img(src='@/assets/curso/tema3/img8.png', style="width: 1200px" ,alt='').m-auto
    .row.align-items-center.mb-5
      .col-lg-6.mb-4.mb-lg-0(data-aos="fade-right")
        p.mb-0 Finalmente, recuerde que cada función del controlador debe ser explotada al módulo por medio del comando:
      .col-lg-6(data-aos="fade-left")
        .row
          .col-12.bg-c10
            .p-4
              p.text-center.mb-0 #[b.txt-c1 module.exports = {fun1, fun2, … fun n}]
    p(data-aos="fade-right") En el que fun1, fun2 y fun n corresponden a las funciones implementadas para la gestión de operaciones sobre los modelos construidos y que, adicionalmente, cada una de estas funciones deberán tener su respectiva representación en el archivo de rutas.
    p.mb-0(data-aos="fade-left") Se recomienda usar las indicaciones del video #[b “Pruebas y rutas con Postman”] para completar el ejercicio de habilitar las operaciones de actualización y eliminación de colecciones y así completar todas las operaciones CRUD del Backend de Ejemplo.

</template>

<script>
export default {
  name: 'Tema3',
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

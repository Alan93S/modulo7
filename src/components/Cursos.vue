<template>
  
    <div class="row justify-content-center">

        <div class="card col-6 col-sm-3 m-3 p-0" v-for="{nombre, codigo, img, url} in cursos" :key="nombre" style="width: 18rem;">
  <img v-bind:src="(img)"  class="card-img-top" alt="imagen">
  <div class="card-body">
    <h5 class="card-title">{{nombre}}</h5>
    <p class="card-text">{{codigo}}</p>

    <a :href="(url)" class="btn btn-primary">Conoce más</a>
  </div>
</div>


    </div>

    <footer>
        <footer class="bg-light text-center text-dark">
  <div class="container p-4 pb-0">
    <section class="">
      <form action="">
        <div class="row d-flex justify-content-center">
          <div class="col-auto">
            <p class="pt-2">
              <strong>Sign up for our newsletter</strong>
            </p>
          </div>

          <div class="col-md-5 col-12">
            <div class="form-outline form-white mb-4">
              <input type="email" id="form5Example29" class="form-control" />
              <label class="form-label" for="form5Example29">Email address</label>
            </div>
          </div>

          <div class="col-auto">
            <button type="submit" class="btn btn-outline-light mb-4">
              Subscribe
            </button>
          </div>
        </div>
      </form>
    </section>
  </div>

  <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2);">
    © 2020 Copyright:
    <p class="text-white" href="https://mdbootstrap.com/">Modulo 7 - Alan - Elizabeth - Rodrigo - Guillermo - Daniel</p>
  </div>
</footer>
    </footer>

</template>

<script>
export default {

    name: 'Cursos',

    data: () => ({

       cursos: [

                    {
                        "codigo": "0001",
                        "nombre": "HTML",
                        "estado": true,
                        "precio": "30000",
                        "duracion":"1 mes",
                        "descripcion": "curso html",
                        "cupos": 10,
                        "inscritos": 0,
                        "img": "https://www.w3.org/html/logo/downloads/HTML5_Logo_512.png",
                        "url": "https://www.udemy.com/course/universidad-html-aprende-html-desde-cero-hasta-experto-css-html5/"
                        },
                        {
                        "codigo": "0002",
                        "nombre": "CSS",
                        "estado": false,
                        "precio": "20000",
                        "duracion":"1 mes",
                        "descripcion": "curso css",
                        "cupos": 20,
                        "inscritos": 0,
                        "img": "https://lineadecodigo.com/wp-content/uploads/2014/04/css.png",
                        "url": "https://www.udemy.com/es/topic/css/"

                        },
                        {
                        "codigo": "0003",
                        "nombre": "SASS",
                        "estado": true,
                        "precio": "40000",
                        "duracion":"2 mes",
                        "descripcion": "curso sass",
                        "cupos": 30,
                        "inscritos": 0,
                        "img": "https://miro.medium.com/max/512/1*9U1toerFxB8aiFRreLxEUQ.png",
                        "url": "https://www.udemy.com/course/sass-curso/"
                        },
                        {
                        "codigo": "0004",
                        "nombre": "VUE",
                        "estado": false,
                        "precio": "50000",
                        "duracion":"3 mes",
                        "descripcion": "curso vue",
                        "cupos": 15,
                        "inscritos": 0,
                        "img": "https://thumbs.gfycat.com/PinkPiercingBull-size_restricted.gif",
                        "url": "https://www.udemy.com/course/vuejs-fh/"
                        }


                            ]


                            })
                            


}

</script>

<style>

</style>
<template>
  <div class="container">
    <header>
      <div class="slider">
        <div class="topnav">
          <div class="text-center" id="div-logo">
            <img id="logo" src="../assets/img/logo.png" alt="logo nuvola pinsa">
          </div>
          <!-- Navigation links (hidden by default) -->
          <div id="nav-links">
            <ul class="mt-4">
              <li v-for="elm in nav" :key="elm.id">
                <a class="text-capitalize" :href="elm.url">{{elm.name}}</a>
                <hr>
              </li>
            </ul>
          </div>
          <!-- "Hamburger menu" / "Bar icon" to toggle the navigation links -->
          <a href="javascript:void(0);" class="icon" @click="myFunction()">
            <i class="fa fa-bars"></i>
          </a>
        </div>

      </div>
    </header>
    <main>
      <div class="d-xl-flex flex-wrap">
        <div class="w-70 my-2">
          <div class="text-center w-90">
            <img class="mt-4" src="../assets/img/bakery.png">
            <h2 class="fs-20 my-2 text-similblack text-center">Una Nuvola di Bontà</h2>
          </div>
          <div class="text-justify text-lightgray">
            <p class="fs-13">La Pinsa Nuvola nasce da un’idea di Corrado Di Marco che, da tre generazioni, attraverso l’azienda di famiglia continua a fare ricerca su farine e metodi di lievitazione. Con la base pronta Nuvola, Di Marco intende portare nelle case la sua più fortunata invenzione del 2001, la Pinsa Romana (fino ad oggi disponibile solo nelle Pinserie certificate), realizzando così un prodotto leggero e digeribile, pronto da condire con gli ingredienti preferiti, mettendo d’accordo tutti… anche chi preferisce una dieta vegetariana.</p>
          </div>
        </div>
        <div class="mt-4 d-xl-flex">
          <div id="bakery" class="col-xl-6 d-xl-flex ai-center jc-center">
            <div class="mb-4">
              <div>
                <div class="w-xl-80">
                  <div class="w-80 mt-4">
                    <h2 class="fs-20 my-2 text-similblack">Nuvola ambient<br>La fragranza a portata di mano, ora anche fuori frigo</h2>
                    <p class="text-justify text-lightgray fs-12">Tutte le caratteristiche di leggerezza, digeribilità, sapore antico, versatilità e facilità di preparazione, sono ora disponibili anche “fuori frigo”. Nuvola infatti, nella sua versione ambient, viene commercializzata al di fuori della catena del freddo della Classica e della Multicereali, senza però rinunciare alle famose caratteristiche della Pinsa Romana originale. Una bella comodità, sia in fase di acquisto sia per la conservazione a casa.Anche con ambient sono sufficienti 5 minuti di forno.</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="pinsa1 col-xl-6">
          </div>
        </div>
      </div>
      <div class="d-xl-flex">
        <div class="pinsa2 col-xl-6" id="romana">
        </div>
        <div class="w-80 col-xl-6 d-xl-flex ai-center jc-center">
          <div class="w-xl-80">
            <h2 class="fs-20 my-2 text-similblack">Nuvola classica<br>La pinsa romana originale</h2>
            <p class="text-justify text-lightgray fs-13">Un mix di farine segreto e una lunga lievitazione per garantire digeribilità, leggerezza e croccantezza: tutto questo è la Pinsa Romana che grazie a NUVOLA può essere preparata in casa. Nuvola è la base pronta di Pinsa, stesa a mano e confezionata in atmosfera modificata per mantenere la freschezza e le caratteristiche di una Pinsa appena sfornata.</p>
          </div>
        </div>
      </div>
      <div class="d-xl-flex">
        <div class="w-80 col-xl-6 d-xl-flex ai-center jc-center">
          <div class="w-xl-80">
            <h2 class="fs-20 my-2 text-similblack">Nuvola multicereali<br>Gusto rustico e leggerezza</h2>
            <p class="text-justify text-lightgray fs-12">Al famoso mix della classica Pinsa Romana sono stati aggiunti farina integrale di segale, semi di girasole, semi di zucca, semi di lino, farina di avena, malto d’orzo e farina d’ orzo, per un impasto integrale ancora più saporito, digeribile e salutare. Bastano 5 minuti di forno con i condimenti preferiti.</p>
          </div>
        </div>
        <div class="pinsa3 mt-4 col-xl-6">
        </div>
      </div>
      <div class="d-xl-flex">
        <div class="impasto col-xl-6">
        </div>
        <div class="w-80 col-xl-6 d-xl-flex ai-center jc-center">
          <div class="w-xl-80">
            <h2 class="fs-20 my-2 text-similblack">Croccante fuori e morbida dentro</h2>
            <p class="text-justify text-lightgray fs-13">L’impasto della Pinsa Nuvola è preparato con Farina di frumento 0, acqua, pasta acida di frumento, farina di riso, farina di soia, olio extra vergine di oliva, sale, lievito, senza alcun conservante aggiunto. Viene fatto lievitare per 72 ore per ottenere in cottura una base croccante fuori e morbida dentro, con un caratteristico profumo di pane antico e con la metà delle calorie (kcal) rispetto ad una normale base per pizza.Incredibilmente soffice e con la caratteristica forma ovale lavorata a mano, la Pinsa Nuvola è perfetta da portare in tavola in ogni occasione, da soli, in famiglia o con gli amici.</p>
          </div>
        </div>
      </div>
      <div class="d-xl-flex">
        <div class="w-80 mb-4 col-xl-6 d-xl-flex ai-center jc-center">
          <div class="w-xl-80">
            <h2 class="fs-20 my-2 text-similblack">Condisci Pinsa Nuvola</h2>
            <p class="text-justify text-lightgray fs-12">Preparare la Pinsa Nuvola è molto semplice, sono sufficienti 5 minuti in forno a 250°C. I tempi di cottura sono indicativi, possono variare a seconda del tipo di forno e del grado di cottura desiderato. Se la desideri più crispy lasciala in forno un minuto in più! In base agli ingredienti scelti il condimento può essere aggiunto prima o dopo il passaggio in forno. La Pinsa Nuvola è disponibile in confezioni singole o da due. Si conserva in frigorifero tra 0°C e 4°C e va aperta qualche minuto prima dell’uso.</p>
          </div>
        </div>
        <div class="pinsa4 col-xl-6">
        </div>
      </div>
      <!-- GALLERY -->
      <div class="text-center w-90 my-2" id="gallery">
        <img class="mt-4 mb-2" src="../assets/img/icon-gallery.png">
        <h2 class="fs-20 text-similblack text-center">Gallery</h2>
      </div>
      <div class="d-flex flex-wrap">
        <div v-for="elm in gallery" :key="elm.id" class="gallery col-12 col-xl-4">
          <img :src="elm.img">
        </div>
      </div>
      <!-- VIDEO -->
      <div class="video d-flex jc-center ai-center" id="video">
        <div class="text-center w-90 my-2">
          <img class="mt-4 mb-2" src="../assets/img/icon-video.png">
          <h2 class="fs-20 text-similblack text-center">Video</h2>
          <span>Watch the Nuvola Pinsa videos! Great tips for topping Nuvola and much more...</span>
          <div class="btn-youtube">
            <span class="text-uppercase"><a href="https://www.youtube.com/channel/UCbGEAjUpX5tjoIfcfhIBg3Q" target="_blank">discover our youtube channel</a></span>
          </div>
        </div>
      </div>
      <!-- ACQUISTA -->
      <div class="acquista d-flex jc-center ai-center" id="acquista">
        <div class="text-center w-90 my-2">
          <img class="mt-4 mb-2" src="../assets/img/logo-white.png">
          <h2 class="fs-20 text-similblack text-center">Where to buy</h2>
          <span>Coming soon...</span>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
name: 'MainComp',
components : {
},
data(){
  return{
    nav : [
      {
        name : 'home',
        url : '#'
      },
      {
        name : 'a cloud of goodness',
        url : '#bakery'
      },
      {
        name : "to whet your appetite",
        url : '#romana'
      },
      {
        name : 'gallery',
        url : '#gallery'
      },
      {
        name : 'video',
        url : '#video'
      },
      {
        name : 'where to buy',
        url : '#acquista'
      },
    ],
    gallery : [
      {
        img : require('../assets/img/gallery-1.jpg')
      },
      {
        img : require('../assets/img/gallery-2.jpg')
      },
      {
        img : require('../assets/img/gallery-3.jpg')
      },
      {
        img : require('../assets/img/gallery-4.jpg')
      },
      {
        img : require('../assets/img/gallery-5.jpg')
      },
      {
        img : require('../assets/img/gallery-6.jpg')
      },
      {
        img : require('../assets/img/gallery-7.jpg')
      },
      {
        img : require('../assets/img/gallery-8.jpg')
      },
      {
        img : require('../assets/img/gallery-9.jpg')
      },
    ]
  }
},
methods : {
  myFunction() {
    var x = document.getElementById("nav-links");
    if (x.style.display === "block") {
      x.style.display = "none";
    } else {
      x.style.display = "block";
    }
  } 
}
}
</script>

<style scoped lang='scss'>
.container{
  header{
    padding: 2em 0;
    .topnav {
      overflow: hidden;
      position: relative;
      background-color: transparent;
      #logo{
        max-width: 100%;
        height: auto;
        width: 10%;
      }
      .fa-bars{
        cursor: pointer;
        font-size: 1.3rem;
        color: #000;
      }
      #nav-links{
        display: none;
        a{
          color: #fff;
          padding: 0.6em 0em;
          text-decoration: none;
          display: block;
          width: 65%;
          margin: 0 auto;
          font-size: 0.9rem;
          font-weight: 700;
        }
        hr{
          color: lightgray;
          width: 70%;
          margin: 0 auto;
        }
      }
      a.icon{
        display: block;
        position: absolute;
        left: 30px;
        top: 12px;
      }
    }
  }
  main{
    #bakery{
      width: 80%;
      margin: 0 auto;
    }
    .pinsa1{
      background-image: url('https://www.nuvolapinsa.com/wp-content/uploads/2022/04/cover-nuvola-ambient.jpg');
      background-position: left;
      background-repeat: no-repeat;
      background-size: auto;
      height: 80vh;
    }
    .pinsa2{
      background-image: url('https://www.nuvolapinsa.com/wp-content/uploads/2021/10/nuvola-classica.jpg');
      background-position: left;
      background-repeat: no-repeat;
      background-size: auto;
      height: 80vh;
    }
    .pinsa3{
      background-image: url('https://www.nuvolapinsa.com/wp-content/uploads/2021/10/nuvola-multicereali-02.jpg');
      background-position: left;
      background-repeat: no-repeat;
      background-size: auto;
      height: 80vh;
    }
    .impasto{
      background-image: url('https://www.nuvolapinsa.com/wp-content/uploads/2021/10/img-01.jpg');
      background-position: left;
      background-repeat: no-repeat;
      background-size: auto;
      height: 80vh;
    }
    .pinsa4{
      background-image: url('https://www.nuvolapinsa.com/wp-content/uploads/2021/10/img-02.jpg');
      background-position: left;
      background-repeat: no-repeat;
      background-size: auto;
      height: 80vh;
    }
    .video{
        background-image: url('../assets/img/banner-video.jpg');
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        height: 55vh;
        width: 100%;
        margin: 1em 0;
        h2{
          color: #fff;
          margin-bottom: 0.7em;
          font-size: 2.2rem;
        }
        span{
          color: #fff;
          font-size: 1.2rem;
        }
        .btn-youtube{
          background-color: #b6191d;
          width: 55%;
          margin: 1em auto;
          padding: 1em 0em;
          a{
            color: #fff;
            font-size: 0.9rem;
            font-weight: 700;
            text-decoration: none;
          }
        }
      }
      .acquista{
        background-image: url('../assets/img/banner-acquisto.jpg');
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        height: 55vh;
        width: 100%;
        h2{
          color: #fff;
          margin-bottom: 0.7em;
          font-size: 2.2rem;
        }
        span{
          color: #fff;
          font-size: 1.2rem;
        }
      }
  }
}

// lg
@media screen and (min-width: 1050px) {
  .container{
    header{
      padding: 0em 0em;
      .topnav {
        padding: 1em 1em;
        display: flex;
        justify-content: space-between;
        align-items: center;
        #div-logo{
          margin-left: 1em;
          #logo{
            width: 100%;
          }
        }
        .fa-bars{
          display: none;
        }
        #nav-links{
          display: unset;
          ul{
            display: flex;
            margin-top: 0;
            padding-left: 2em;
            li{
              padding: 0 1em;
            }
          }
          a{
            padding: 0em 0em;
            width: unset;
            margin: 0 auto;
            font-size: 1rem;
          }
          hr{
            display: none;
          }
        }
      }
      .slider{
        background-image: url('../assets/img/banner-eng.jpeg');
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        height: 110vh;
        width: 100%;
      }
    }
    main{
      .pinsa1{
        background-size: cover;
      }
      .pinsa2{
        background-size: cover;
      }
      .pinsa3{
        background-size: cover;
      }
      .impasto{
        background-size: cover;
      }
      .pinsa4{
        background-size: cover;
      }
      .gallery{
        img{
          max-width: 100%;
          height: auto;
          padding: 0.5em;
        }
      }
      .video{
        .btn-youtube{
          width: 22%;
        }
      }
    }
  }
}


@media screen and (min-width: 1200px){

  main{
    .pinsa1{
      width: 95%;
      margin: 0 auto;
    }
    .pinsa2{
      width: 95%;
      margin: 0 auto;
    }
    .pinsa3{
      width: 95%;
      margin: 0 auto;
    }
    .impasto{
      width: 95%;
      margin: 0 auto;
    }
    .pinsa4{
      width: 95%;
      margin: 0 auto;
    }
  }
}

</style>
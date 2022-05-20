<template>
  <div id="app">
    <MainComp/>
  </div>
</template>

<script>
import MainComp from "./components/MainComp.vue"

export default {
  name: 'App',
  components: {
    MainComp
  }
}
</script>

<style lang="scss">
*{padding: 0; margin: 0; box-sizing: border-box; font-family: sans-serif; scroll-behavior: smooth;}
li{list-style-type: none;}

@for $i from 1 through 12{
  .col-#{$i}{width: calc(100% / 12) * $i; flex-basis: calc(100% / 12) * $i;}
}


@for $i from 1 through 12{
  .offright-#{$i}{margin-right: calc(100% / 12) * $i;}
}

.w-70{width: 70%; margin: 0 auto;}
.w-80{width: 80%; margin: 0 auto;}
.w-90{width: 90%; margin: 0 auto;}

.d-none{display: none;}
.d-block{display: block;}
.d-flex{display: flex;}
.flex-wrap{flex-wrap: wrap;}
.jc-center{justify-content: center;}
.ai-center{align-items: center;}

.text-uppercase{text-transform: uppercase;}
.text-capitalize{text-transform: capitalize;}
.text-center{text-align: center;}
.text-justify{text-align: justify;}

.text-lightgray{color: #808285;}
.text-similblack{color: #3a3a3a;}

.fs-20{font-size: 2rem;}
.fs-17{font-size: 1.7rem;}
.fs-13{font-size: 1.3rem;}
.fs-12{font-size: 1.2rem;}

.mt-4{margin-top: 2em;}
.mb-2{margin-bottom: 1em;}
.mb-4{margin-bottom: 2em;}
.my-2{margin-bottom: 1em; margin-top: 1em;}
.my-4{margin-bottom: 2em; margin-top: 2em;}

@media screen and (min-width: 1200px) {

  @for $i from 1 through 12{
    .col-xl-#{$i}{width: calc(100% / 12) * $i; flex-basis: calc(100% / 12) * $i;}
  }

  .d-xl-flex{display: flex;}

  .w-xl-80{width: 80%; margin: 0 auto;}
}
</style>

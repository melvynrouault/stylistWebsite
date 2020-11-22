<template>
  <div class="container">
    <div>
      <header>
        <img src="~/assets/logo.png" alt="" id="logo">
        <h1 class="title">
          A fashion website for fashion victims
        </h1>
      </header>

      <body>
        <test-card />
        
      </body>

    </div>
  </div>
</template>

<script>

  import Vue from 'vue'
  import Vuesax from 'vuesax'
  import 'vuesax/dist/vuesax.css' //Vuesax styles
  
  import testCard from '../components/testCard.vue'

  Vue.use(Vuesax, {
    // options here
  })

  export default {
    components: { testCard },
  }
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  /* align-items: center; */
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 50px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

#logo {
  width: auto;
  height: auto;
}

body {
  max-width: 100%;
  height: auto;
  /* background-image: url('../assets/apparel.jpg'); */
  /* background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover; */
}

.testDiv {
  display: block;
  width: 100%;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 300px;
  margin-bottom: 20px;
  content: '';
}

.testDivImage1 {
  background-image: url('~assets/masques/hiboux.jpg');
}

.testDivImage2 {
  background-image: url('~assets/paniers/panier.jpg');
}

.testDivImage3 {
  background-image: url('~assets/tissus/tissus.jpg');
}

.testDiv img {
  display: block;
  width: 100%;
}

.card-body {
  padding: 0 !important;
}


vs-card-group {
  width: 100%;
  height: auto;
}
</style>

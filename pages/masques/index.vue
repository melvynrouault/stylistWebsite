<template>
  <div>
    <div>
      <div class="center examplex">
      <vs-navbar target-scroll="#padding-scroll-content" padding-scroll center-collapsed v-model="active" class="navbar">

        <template #left>
          <NuxtLink to="/">
            <img src="~assets/logo.png" alt="">
          </NuxtLink>
        </template>

        <vs-navbar-item :active="active == 'masques'" id="masques">
          <NuxtLink to="/masques">
            Masques
          </NuxtLink>
        </vs-navbar-item>
        
        <vs-navbar-item :active="active == 'paniers'" id="paniers">
          <NuxtLink to="/paniers">
            Paniers
          </NuxtLink>
        </vs-navbar-item>

        <vs-navbar-item :active="active == 'cotons'" id="cotons">
          <NuxtLink to="/cotons">
            Cotons
          </NuxtLink>
        </vs-navbar-item>

        <vs-navbar-item :active="active == 'tissus'" id="tissus">
          <NuxtLink to="/tissus">
            Tissus
          </NuxtLink>
        </vs-navbar-item>

        <template #right>
          <vs-button flat >Se connecter</vs-button>
          <vs-button>S'inscrire</vs-button>
        </template>

      </vs-navbar>
    </div>
    </div>

    <div class="masqueContent">
      <h1>Masques</h1>
      <div id="padding-scroll-content">

        <test-card />

        <test-card />

        <test-card />

        <test-card />

        <test-card />

        <test-card />
      </div>
    </div>


  </div>
</template>

<style>

.navbar {
  position: fixed;
}

.masqueContent {
  position: relative;
  top: 200px;
}

.masqueContent h1 {
  text-align: center;
}

</style>

<script>

  import Vue from 'vue'
  import Vuesax from 'vuesax'
  import 'vuesax/dist/vuesax.css' //Vuesax styles
  

  Vue.use(Vuesax, {
    // options here
  })

  export default {
    // layout : 'page_layout',
  }
</script>
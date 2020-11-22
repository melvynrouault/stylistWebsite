
<template>
    <div class="center examplex">
      <vs-navbar target-scroll="#padding-scroll-content" padding-scroll center-collapsed v-model="active">

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
      <div id="padding-scroll-content" class="square">
        <div class="child">
          child 1
        </div>
        <div class="child">
          child 2
        </div>
        <div class="child">
          child 3
        </div>
      </div>
    </div>
  </template>
<script>
  export default {
    data:() => ({
      active: 'guide'
    })
  }
  </script>

        
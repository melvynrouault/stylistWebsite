 <template>
  <vs-card-group>
     <NuxtLink to="/masques">
      <vs-card>
        <template #title>
          <h3>Des masques de qualités, lavables et personnalisables !</h3>
        </template>
        <template #img>
          <img src="~assets/masques/hiboux.jpg" alt="">
        </template>
        <template #text>
          <p>
            Fabriqué en 2 semaines
          </p>
        </template>
      </vs-card>
     </NuxtLink>

     <NuxtLink to="/paniers">
      <vs-card>
        <template #title>
          <h3>Un panier pour ranger tout plein de choses !</h3>
        </template>
        <template #img>
          <img src="~assets/paniers/panier.jpg" alt="">
        </template>
        <template #text>
          <p>
            Fabriqué en 3 semaines
          </p>
        </template>
      </vs-card>
     </NuxtLink>

     <NuxtLink to="/cotons">
      <vs-card>
        <template #title>
          <h3>Des lingettes démaquillantes réutilisables !</h3>
        </template>
        <template #img>
          <img src="~assets/tissus/tissus.jpg" alt="">
        </template>
        <template #text>
          <p>
            Fabriqué en 2 semaines
          </p>
        </template>
      </vs-card>
     </NuxtLink>

      </vs-card-group>

</template>

<style scoped>

</style>


<script>
export default {
  
}
</script>


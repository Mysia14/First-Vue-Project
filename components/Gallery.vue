<template>
  <v-container class="flex justify-center align-center  m-20">
    <v-main class=" flex justify-center align-center  m-20">
       <h1 class="font-bold">{{ galleryPage.title }}</h1>
    <ul>
      <li class="text-red-900 font-bold flex justify-center align-center" v-text="galleryPage.name"></li>
      <li class="text-red-500 font-italic flex justify-center align-center" v-text="galleryPage.ingredients"></li>
      <nuxt-img class="max-w-screen-md mx-8" v-if="galleryPage.image" :src="galleryPage.image"  sizes="sm:50vw md:300px lg:758px" />
       

    </ul>
    </v-main>
      
  </v-container>
</template>

<script>
export default {
  props: ['galleryPage']
}
</script>
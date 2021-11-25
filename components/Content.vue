<template>
  <v-container class="flex justify-center align-center flex-col text-center pt-5 m-auto">
    <h1 class="text-3xl p-2 text-red-900" >{{ contentPage.food }}</h1>
    <p class="text-2xl pb-8 text-pink-300 italic"> {{ contentPage.country }}</p>
  </v-container>
</template>
<script>
export default {
  props: ['contentPage']
}
</script>
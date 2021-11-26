<template>
  <v-container class="flex justify-center align-center flex-col text-center text-red-900 bg-red-300">
    <h1 class="p-10 text-5xl font-sans md:font-serif">{{ headerPage.title }}</h1>
    <Navigation />
  </v-container>
</template>

<script>
export default {
  props: ['headerPage']
}
</script>
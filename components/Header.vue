<template>
  <v-container class="flex justify-center align-center flex-col text-center p-3 bg-red-300">
    <h1 class="p-10 text-5xl font-bold font-sans md:font-serif">{{ headerPage.title }}</h1>
    <Navigation />
  </v-container>
</template>

<script>
export default {
  props: ['headerPage']
}
</script>
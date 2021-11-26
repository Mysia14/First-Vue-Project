<template>
<footer>
  <v-container class="flex justify-center align-center flex-col text-center bg-red-200">
    <p class="text-md text-gray-600">&copy;Mysia2021 {{ footerPage.license }}</p>
  </v-container>
  </footer>
</template>
<script>
export default {
  props: ['footerPage']
}
</script>
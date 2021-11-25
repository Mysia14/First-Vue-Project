<template>
  <v-container>
    <Header :headerPage="info" />
    <h1 class="text-7xl p-7 text-center text-red-300"> International Food list </h1>
    <Content v-for="food in foods" :key="food.id" :contentPage="food" />
    <Footer :footerPage="info" />
  </v-container>
</template>

<script>
export default {
  data () {
    return {
      info: {
        title: 'Excentric Cuisine',
        description: 'Some uniques international food',
        author: 'Mysia Santana',
        license: 'MIT License'
      },
      contents: [
        {
          country: 'Indian',
          name: 'Gabriela Palai',
          ingredients: 'https://www.pexels.com/@gabriela-palai-129458',
          url: 'uk.jpg'
        },
        {
          country: 'Indian',
          name: 'Gabriela Palai',
          ingredients: 'https://www.pexels.com/@gabriela-palai-129458',
          url: 'uk.jpg'
        },
        {
          country: 'Indian',
          name: 'Gabriela Palai',
          ingredients: 'https://www.pexels.com/@gabriela-palai-129458',
          url: 'uk.jpg'
        },
        {
          country: 'Indian',
          name: 'Gabriela Palai',
          ingredients: 'https://www.pexels.com/@gabriela-palai-129458',
          url: 'uk.jpg'
        }
      ],
      foods: [
        {
          food: 'Pizza',
          country: 'Italy'
        },
        {
          food: 'Sushi',
          country: 'Japan'
        },
        {
          food: 'Tacos',
          country: 'Mexico'
        },
        {
          food: ' Greek Salada',
          country: 'Greece'
        }
      ]
    }
  },
  head () {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }
      ]
    }
  }
}
</script>
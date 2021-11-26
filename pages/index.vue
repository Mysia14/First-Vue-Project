<template>
  <v-container>
    <Header :headerPage="info" />
    <h1 class="text-4xl p-12 text-center text-red-600"> Favourites International Foods </h1>
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
          ingredients: "tomato sauce, cheese and basil",
          image:"assets/images/mexican.jpg",
          food:"tacos",
        },
        {
          ingredients: "tomato sauce, cheese and basil",
          image:"assets/images/mexican.jpg",
          food:"pizza",
        },
        {
          ingredients: "tomato sauce, cheese and basil",
          image:"assets/images/mexican.jpg",
          food:"pizza",
        },
        {
          ingredients: "tomato sauce, cheese and basil",
          image:"assets/images/mexican.jpg",
          food:"pizza",
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
          country: 'Mexico',
          image:"images/mexican.jpg",
        },
        {
          food: 'Greek Salad',
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
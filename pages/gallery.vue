<template>
  <v-container> 
    <Header :headerPage="info" />
      <v-main>
        <Gallery v-for="content in contents" :key="content.id" :galleryPage="content" />
      </v-main>
    <Footer :footerPage="info" />
  </v-container>
</template>
<script>
export default {
  data () {
    return {
      info: {
        title: ' Some Delicious Meals',
        description: 'We eat wiht the our eyes too',
        author: 'Mysia Santana',
        license: 'MIT License'
      },
      contents: [
        {
          ingredients: "Tomato sauce, cheese and basil.",
          image:"assets/images/italian.jpg",
          name:"Pizza",
         
        },
        {
          ingredients: "Tomatoes, onion, feta cheese and peppers.",
          image:"assets/images/greek.jpg",
          name:"Greek salad",
          
        },
        {
          ingredients: "Grounded beef, spices and cilantro.",
          image:"assets/images/mexican.jpg",
          name:"Tacos",
        },
        {
          ingredients: "Fresh Fish.",
          image:"assets/images/japanese.jpg",
          name:"Sushi",
        }
      ]
    }
  }
}
</script>
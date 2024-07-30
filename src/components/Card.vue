<template>
    <div class="card">
        <img class="card__image" :src="require(`@/assets/img/${image}`)" alt="Icono de la carta">
        <h2 class="card__title">{{title}}</h2>
        <span class="card__line"></span>
        <p class="card__paragraph">{{paragraph}}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'CardComponent',
    props: {
        image: String,
        title: String,
        paragraph: String
    }
  }
  </script>
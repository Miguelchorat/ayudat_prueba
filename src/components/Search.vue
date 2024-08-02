<template>
    <form class="search">
        <input class="search__input" type="email" placeholder="Your email" :value="search">
        <a class="search__button" href="#">Suscribe</a>
    </form>
  </template>
  
  <script>
  export default {
    name: 'SearchComponent',
    data() {
        return {
            search: ''
        }
    },
  }
  </script>
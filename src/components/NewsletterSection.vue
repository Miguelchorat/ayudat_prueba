<template>
    <section class="newsletter">
      <article class="newsletter__content">
        <InfoTitle subtitle="Newsletter" title="Get Quality Education" paragraph="Problems trying to resolve the conflict between 
the two major realms of Classical physics: Newtonian mechanics "/>
        <Search />
      </article>
      <article class="newsletter__footer">
        <Footer />
      </article>      

    </section>
  </template>
  
  <script>
  import InfoTitle from './InfoTitle.vue';
  import Footer from './Footer.vue';
  import Search from './Search.vue';

  export default {
    components: {
      InfoTitle,
      Footer,
      Search
    },
    data() {
      return {
        
      }
    }
  }
  </script>
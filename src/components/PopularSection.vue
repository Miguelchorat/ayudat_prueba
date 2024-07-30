<template>
  <section class="popular">
    <InfoTitle subtitle="Practice Advice" title="Most Popular Courses" paragraph="Problems trying to resolve the conflict between 
    the two major realms of Classical physics: Newtonian mechanics"/>

    <div class="popular__content">
      <Card v-for="(card, index) in cards" :key="index" :image="card.image" :title="card.title" :paragraph="card.paragraph"/>
    </div>
  </section>
</template>

<script>
import InfoTitle from './InfoTitle.vue';
import Card from './Card.vue';

export default {
  components: {
    InfoTitle,
    Card
  },
  data() {
    return {
      cards: [
        { image: 'school.svg', title: 'Expert instruction', paragraph: 'The gradual accumulation and small-scale..' },
        { image: 'book.svg', title: '2,769 online courses', paragraph: 'The gradual accumulation and small-scale..' }
      ]
    }
  }
}
</script>
<template>
    <section class="package">
      <InfoTitle subtitle="Practice Advice" title="Approdable Packages" paragraph="Problems trying to resolve the conflict between 
the two major realms of Classical physics: Newtonian mechanics "/>
  
      <div class="package__content">
        <CardSale v-for="(card, index) in cards" :key="index" :image="card.image" :subtitle="card.subtitle" :title="card.title" :paragraph="card.paragraph"
        :countSales="card.countSales" :oldPrice="card.oldPrice" :newPrice="card.newPrice" :score="card.score" :learn="card.learn" :favorite="card.favorite" :eye="card.eye" :buy="card.buy"/>
      </div>
    </section>
  </template>
  
  <script>
  import InfoTitle from './InfoTitle.vue';
  import CardSale from './CardSale.vue';
  
  export default {
    components: {
      InfoTitle,
      CardSale
    },
    data() {
      return {
        cards: [
          { image: 'background_card1.png', subtitle: 'Welcome', title: 'Training Courses', paragraph: 'We focus on ergonomics and meeting you where you work. It is only a keystroke away.' 
            , countSales: 15, oldPrice: 16.48, newPrice: 6.48, score: 4.9, learn: '#', favorite: '#', eye: '#',buy: '#'
          },
          { image: 'background_card2.png', subtitle: 'Welcome', title: 'Lifetime access', paragraph: 'We focus on ergonomics and meeting you where you work. It is only a keystroke away.' 
            , countSales: 15, oldPrice: 16.48, newPrice: 6.48, score: 4.9, learn: '#', favorite: '#', eye: '#',buy: '#'
          }
        ]
      }
    }
  }
  </script>
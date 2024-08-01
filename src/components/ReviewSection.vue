<template>
    <section class="reviewSection">
      <InfoTitle subtitle="Practice Advice" title="Most Popular Courses" paragraph="Problems trying to resolve the conflict between 
the two major realms of Classical physics: Newtonian mechanics "/>
  
      <div class="reviewSection__content">
        <Review v-for="(review, index) in reviews" :key="index" :image="review.image" :name="review.name" :paragraph="review.paragraph"
        :score="review.score" :job="review.job" />
      </div>
    </section>
  </template>
  
  <script>
  import InfoTitle from './InfoTitle.vue';
  import Review from './Review.vue';

  export default {
    components: {
      InfoTitle,
      Review
    },
    data() {
      return {
        reviews: [
          { image: 'user1.png', paragraph: 'We focus on ergonomics and meeting you where you work. It is only a keystroke away.' 
            , score: 4, name: 'Regina Miles', job: 'Designer'
          },
          { image: 'user2.png', paragraph: 'We focus on ergonomics and meeting you where you work. It is only a keystroke away.' 
            , score: 3, name: 'Regina Miles', job: 'Designer'
          }
        ]
      }
    }
  }
  </script>
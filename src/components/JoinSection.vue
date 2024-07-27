<template>
  <section class="join">
    <img class="join__figure join__figure--1" src="../assets/img/figure_1.svg" alt="figure background" />
    <img class="join__figure join__figure--2" src="../assets/img/figure_2.svg" alt="figure background" />
    <Header />
    <div class="join__content">
      <article class="join__content__info">
        <h3>Join Us</h3>
        <h1>25k+ STUDENTS TRUST US</h1>
        <p>Every day brings with it a fresh set of learning possibilities</p>
        <div>
          <button>
            Join us
          </button>
          <button>
            Learn More
          </button>
        </div>
      </article>
      <article class="join__content__image">

      </article>
    </div>
  </section>
</template>


<script>
import Header from '@/components/Header.vue';

export default {
  components: {
    Header
  }
}
</script>
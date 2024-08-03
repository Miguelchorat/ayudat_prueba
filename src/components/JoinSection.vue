<template>
  <section class="join">
    <div class="join__content">
      <article class="join__content__info">
        <h3 class="join__content__info__subtitle">Join Us</h3>
        <h1 class="join__content__info__title">25k+ STUDENTS <br>TRUST US</h1>
        <p class="join__content__info__paragraph">Every day brings with it a fresh set of<br> learning possibilities</p>
        <div class="join__content__info__buttons">
          <Button button-text="Join us" link="#"/>
          <Button button-text="Learn More" fill="true" link="#"/>
        </div>
      </article>
      <article class="join__content__image">
        <img class="join__content__image__photo" src="../assets/img/image_woman.png" alt="Imagen de una mujer">
        <img class="join__content__image__bigellipse" src="../assets/img/ellipse_1.svg" alt="">
        <img class="join__content__image__graphic1" src="../assets/img/graphic_1.svg" alt="">
        <img class="join__content__image__graphic2" src="../assets/img/graphic_2.png" alt="">
        <img class="join__content__image__graphic3" src="../assets/img/graphic_3.png" alt="">
        <img class="join__content__image__ellipse" src="../assets/img/ellipse_2.svg" alt="">
        <img class="join__content__image__wave" src="../assets/img/wave.svg" alt="">
      </article>
    </div>
  </section>
</template>


<script>
import Button from '@/components/Button.vue';

export default {
  components: {
    Button
  }
}
</script>
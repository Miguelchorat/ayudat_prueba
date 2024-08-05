<template>
  <section class="join">
    <div class="join__content">
      <article class="join__content__info">
        <h3 class="join__content__info__subtitle">Join Us</h3>
        <h1 class="join__content__info__title">25k+ STUDENTS <br>TRUST US</h1>
        <p class="join__content__info__paragraph">Every day brings with it a fresh set of<br> learning possibilities</p>
        <div class="join__content__info__buttons">
          <Button button-text="Join us" link="#"/>
          <Button button-text="Learn More" :fill="true" link="#"/>
        </div>
      </article>
      <article class="join__content__image">
        <img class="join__content__image__photo" src="../assets/img/woman1.svg" alt="Imagen de una mujer">
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
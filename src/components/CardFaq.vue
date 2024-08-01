<template>
    <div class="cardFaq">
        <img class="cardFaq__icon" src="../assets/img/arrow.svg" alt="arrow">
        <h2 class="cardFaq__title">{{ title }}</h2>
        <p class="cardFaq__paragraph">{{ paragraph }}</p>
    </div>
</template>

<script>
export default {
    name: 'CardFaqComponent',
    props: {
        title: String,
        paragraph: String
    }
}
</script>
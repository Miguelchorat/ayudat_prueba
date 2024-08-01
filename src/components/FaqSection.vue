<template>
    <section class="faq">
        <InfoTitle subtitle="" title="FAQ" paragraph="Problems trying to resolve the conflict between 
the two major realms of Classical physics: Newtonian mechanics " />

        <div class="faq__content">
            <CardFaq v-for="(card, index) in cards" :key="index" :title="card.title" :paragraph="card.paragraph" />
        </div>
    </section>
</template>

<script>
import InfoTitle from './InfoTitle.vue';
import CardFaq from './CardFaq.vue';

export default {
    components: {
        InfoTitle,
        CardFaq
    },
    data() {
        return {
            cards: [
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                },
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                },
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                },
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                },
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                },
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                },
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                },
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                },
                {
                    title: 'the quick fox jumps over the lazy dog', paragraph: 'Things on a very small scale behave like nothing'
                }
            ]
        }
    }
}
</script>
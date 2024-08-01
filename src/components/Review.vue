<template>
    <div class="review">
        <img class=" review__image" :src="require(`@/assets/img/${image}`)" alt="Imagen de la review">
        <p class="review__paragraph">{{ paragraph }}</p>
        <div class="review__score">
            <img v-for="star in stars" :key="star" :src="starImage(star)" alt="star" class="review__score__icon" />
        </div>
        <h3 class="review__name">{{ name }}</h3>
        <p class="review__job">{{ job }}</p>

    </div>
</template>

<script>
export default {
    name: 'ReviewComponent',
    props: {
        image: String,
        paragraph: String,
        job: String,
        name: String,
        score: Number
    },
    computed: {
        stars() {
            // Limitar la puntuación entre 1 y 5
            const limitedScore = Math.min(Math.max(this.score, 1), 5);
            // Convertir la puntuación a un número entero
            const roundedScore = Math.floor(limitedScore);
            // Crear un array con el número de estrellas llenas y vacías
            return Array.from({ length: 5 }, (_, index) => index < roundedScore ? 'star1' : 'star2');
        }
    },
    methods: {
        starImage(star) {
            return require(`@/assets/img/${star}.svg`);
        }
    }
}
</script>
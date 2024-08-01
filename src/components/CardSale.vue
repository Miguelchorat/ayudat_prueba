<template>
    <div class="cardSale">
        <img class=" cardSale__image" :src="require(`@/assets/img/${image}`)" alt="Icono de la carta">
        <p class="cardSale__label">Sale</p>
        <h2 class="cardSale__subtitle">{{ subtitle }}</h2>
        <h2 class="cardSale__title">{{ title }}</h2>
        <p class="cardSale__paragraph">{{ paragraph }}</p>
        <div class="cardSale__score">
            <img class="cardSale__score__icon" src="../assets/img/star.svg" alt="">
            <p class="cardSale__score__text">{{ score }}</p>
        </div>
        <div class="cardSale__sales">
            <img class="cardSale__sales__icon" src="../assets/img/sale.svg" alt="">
            <p class="cardSale__sales__text">{{ countSales }} Sales</p>
        </div>
        <div class="cardSale__price">
            <p class="cardSale__price__old">${{ oldPrice }}</p>
            <p class="cardSale__price__new">${{ newPrice }}</p>
        </div>
        <div class="cardSale__link">
            <a class="cardSale__favorite" :href="favorite"><img class="cardSale__favorite__icon" src="../assets/img/favorite.svg" alt=""></a>
            <a class="cardSale__buy" :href="buy"><img class="cardSale__buy__icon" src="../assets/img/buy.svg" alt=""></a>
            <a class="cardSale__eye" :href="eye"><img class="cardSale__eye__icon" src="../assets/img/eye.svg" alt=""></a>            
        </div>
        <a class="cardSale__learn">Learn More ❯</a>
    </div>
</template>

<script>
export default {
    props: {
        image: String,
        title: String,
        paragraph: String,
        subtitle: String,
        countSales: Number,
        oldPrice: Number,
        newPrice: Number,
        learn: String,
        favorite: String,
        buy: String,
        eye: String,
        score: Number
    }
}
</script>
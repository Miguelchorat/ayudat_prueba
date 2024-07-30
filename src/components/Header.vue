<template>
    <header class="header">
        <div class="header__nav">
            <h2 class="header__nav__title">BrandName</h2>
            <ul class="header__nav__list">
                <li class="header__nav__list__item"><a class="header__nav__list__item__link" href="#">Home</a></li>
                <li class="header__nav__list__item"><a class="header__nav__list__item__link" href="#">Product</a></li>
                <li class="header__nav__list__item"><a class="header__nav__list__item__link" href="#">Pricing</a></li>
                <li class="header__nav__list__item"><a class="header__nav__list__item__link" href="#">Contact</a></li>
            </ul>
        </div>
        <div class="header__access">
            <a class="header__access__login" href="#">Login</a>
            <Button button-text="JOIN US &nbsp; 🡢" link="#"/>
        </div>
    </header>
</template>

<script>
import Button from '@/components/Button.vue';

export default {
    name: 'HeaderComponent',
    components: {
        Button
    }
}
</script>
<template>
    <div class="menu" :class="{ 'menu__open': menu, 'menu__close': !menu }">              
        <div class="menu__header">
            <img class="menu__header__close" src="../assets/img/close.svg" alt="#" @click="listenMenu">
        </div>  
        <div class="menu__nav">
            <ul class="menu__nav__list">
                <li class="menu__nav__list__item"><a class="menu__nav__list__item__link" href="#">Home</a></li>
                <li class="menu__nav__list__item"><a class="menu__nav__list__item__link" href="#">Product</a></li>
                <li class="menu__nav__list__item"><a class="menu__nav__list__item__link" href="#">Pricing</a></li>
                <li class="menu__nav__list__item"><a class="menu__nav__list__item__link" href="#">Contact</a></li>
            </ul>
        </div>
        <div class="menu__access">
            <a class="menu__access__login" href="#">Login</a>
            <Button button-text="JOIN US &nbsp; 🡢" link="#" />
        </div>        
    </div>
</template>

<script>
import Button from '@/components/Button.vue';

export default {
    name: 'MenuComponent',
    components: {
        Button
    },
    props: {
        menu: Boolean
    },
    data() {
        return {
        }
    },
    methods: {
        listenMenu(){
            this.$emit('listenMenu')
        }
    }
}
</script>
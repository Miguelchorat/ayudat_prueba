<template>
    <header class="header" :class="{ header__scroll: isScrolled }" ref="header">
        <div class="header__nav">
            <h2 class="header__nav__title" @click="scrollToTop()">BrandName</h2>
            <ul class="header__nav__list">
                <li class="header__nav__list__item"><a class="header__nav__list__item__link" href="#">Home</a></li>
                <li class="header__nav__list__item"><a class="header__nav__list__item__link" href="#">Product</a></li>
                <li class="header__nav__list__item"><a class="header__nav__list__item__link" href="#">Pricing</a></li>
                <li class="header__nav__list__item"><a class="header__nav__list__item__link" href="#">Contact</a></li>
            </ul>
        </div>
        <div class="header__access">
            <a class="header__access__login" href="#">Login</a>
            <Button button-text="JOIN US &nbsp; 🡢" link="#" />
        </div>
    </header>
</template>

<script>
import Button from '@/components/Button.vue';

export default {
    name: 'HeaderComponent',
    components: {
        Button
    },
    props: {
        scroll: Number,
        container: Object
    },
    data() {
        return {
            isScrolled: false,
            container2: this.container
        }
    },
    watch: {
        scroll(newScroll) {
            this.handleScroll(newScroll);
        }
    },
    methods: {
        handleScroll(newScroll) {
            this.isScrolled = newScroll > this.$refs.header.offsetHeight * 8;
        },
        scrollToTop() {
            this.container2 = this.container
            if (this.container2 && typeof this.container2.scrollTo === 'function') {
                this.container2.scrollTo({
                    top: 0,
                    behavior: 'smooth'
                });
            }
        }
    }
}
</script>
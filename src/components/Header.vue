<template>
    <header class="header">
        <div class="header__nav">
            <h2 class="header__nav__title">BrandName</h2>
            <ul class="header__nav__list">
                <li class="header__nav__list__item">Home</li>
                <li class="header__nav__list__item">Product</li>
                <li class="header__nav__list__item">Pricing</li>
                <li class="header__nav__list__item">Contact</li>
            </ul>
        </div>
        <div class="header__access">
            <a class="header__access__login" href="#">Login</a>
            <a class="header__access__joinus" href="#">Join Us</a>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderComponent'
}
</script>
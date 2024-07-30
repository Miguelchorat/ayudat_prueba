<template>
    <a class="button" :class="{ 'button--fill': fill }" :href="link">
        <p class="button__text">{{ buttonText }}</p>
    </a>
</template>

<script>
export default {
    name: 'ButtonComponent',
    props: {
        buttonText: String,
        fill: Boolean,
        link: String
    }
}
</script>
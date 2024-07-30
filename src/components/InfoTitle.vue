<template>
    <div class="info">
        <h3 class="info__subtitle">{{ subtitle }}</h3>
        <h2 class="info__title">{{ title }}</h2>
        <p class="info__paragraph" >{{ paragraph }}</p>
    </div>
</template>

<script>
export default {
    props: {
        subtitle: String,
        title: String,
        paragraph: String
    }
}
</script>
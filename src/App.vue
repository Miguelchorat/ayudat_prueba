<template>
  <div class="container" ref="container">    
    <Header :scroll="scroll" :container="this.$refs.container"/>
    <router-view />
  </div>
</template>

<script>

import Header from '@/components/Header.vue';

export default {
  components: {
    Header
  },
  data() {
    return {
      scroll: 0,
    };
  },
  mounted() {
    const container = this.$refs.container
    container.addEventListener('scroll', this.onScroll)
  },
  beforeUnmount() {
    this.$refs.container.removeEventListener('scroll', this.onScroll);
  },
  methods: {
    onScroll() {
      const container = this.$refs.container
      this.scroll = container.scrollTop
    },
  },
}
</script>

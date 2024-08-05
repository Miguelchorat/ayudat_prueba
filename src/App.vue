<template>
  <div class="container" ref="container">    
    <Header :scroll="scroll" :container="this.$refs.container" :menu="menu" @listenMenu="listenMenu"/>
    <router-view />
    <Menu :menu="menu" @listenMenu="listenMenu"/>
  </div>
</template>

<script>

import Header from '@/components/Header.vue';
import Menu from '@/components/Menu.vue';

export default {
  components: {
    Header,
    Menu
  },
  data() {
    return {
      scroll: 0,
      menu: false
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
    listenMenu(){
      this.menu = !this.menu
    }
  },
}
</script>

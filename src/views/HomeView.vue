<template>
  <main class="home">
    <JoinSection />
    <PopularSection />
  </main>
</template>
<script>

import JoinSection from '@/components/JoinSection.vue';
import PopularSection from '@/components/PopularSection.vue';

export default {
  components: {
    JoinSection,
    PopularSection
  }
}
</script>
